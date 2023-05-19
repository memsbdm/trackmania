<script lang="ts">
    import Download from "$lib/components/Download.svelte";
    import Documentation from "./Documentation.svelte";
    import ScriptCards from "./ScriptCards.svelte";

    export let unlimiterDetails;
    $: scriptPage = 0;
    const numberOfPages = unlimiterDetails.scripts.length / 3 - 1;
</script>

<div class="unlimiter__container" style="background-image: {unlimiterDetails.background}">
    <div class="unlimiter__header">
        <img src="/images/folder.svg" alt="icône de dossier">
        <h1>UNLIMITER {unlimiterDetails.version}</h1>
        <Download />
    </div>
</div>

<div class="unlimiter__documentation">
    <h3>Documentation</h3>
    <div class="documentation">
        {#each unlimiterDetails.documentation as documentationDetails}
            <Documentation {documentationDetails}/>
        {/each}
    </div>
</div>

<div class="unlimiter__scripts">
    <div class="scripts__header">
        <h3>Scripts</h3>
        <div class="buttons">
            <button on:click={()=>scriptPage>=numberOfPages?scriptPage--:''} ><i class="fa-solid fa-chevron-left"></i> Previous</button>
            <span>Page {scriptPage+1}</span>
            <button on:click={()=>scriptPage<numberOfPages?scriptPage++:''}>Next <i class="fa-solid fa-chevron-right"></i></button>
        </div>
    </div>
    <div class="scripts">
        <ScriptCards {scriptPage} scripts={unlimiterDetails.scripts}  />
    </div>
</div>

<style lang="scss">
  h3{
    color: var(--white-text);
    opacity: .8;
  }
  span{
    margin: 0 1.5rem;
    color: var(--white-text);
    opacity: .8;
  }
    .unlimiter__container{
      width: calc(90% - 6rem);
      border-radius: 20px;
      padding: 2rem 3rem;
      background-size: cover;
      background-position: center;
      position: relative;
    }

    .unlimiter__header {
      img{
        width: 4rem;
        filter: invert(100%);
      }
      h1{
        margin: 1rem 0 2rem 0;
        color: var(--white-text);
      }
    }

    .unlimiter__documentation {
      h3{
        margin: 2rem 0 1rem 0;
      }
      width: 90%;
      .documentation{
        overflow: hidden;
        border-radius: 20px;
        border: 1px solid var(--light-gray-bg);
        background-color: var(--content-bg);
      }
    }

    .unlimiter__scripts {
      width: 90%;
      .scripts__header{
        display: flex;
        justify-content: space-between;
        margin: 2rem 0 1rem 0;
        button{
          outline: none;
          border: none;
          background-color: transparent;
          opacity: .4;
          cursor: pointer;
          font-size: 1rem;
          color: var(--white-text);
        }
      }
      .scripts{
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
      }
      @media screen and (max-width: 900px){
        .scripts{
          gap: 1rem;
          padding-bottom: 2rem;
        }
      }
    }
</style>