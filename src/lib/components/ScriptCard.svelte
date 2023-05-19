<script lang="ts">
    import Download from "$lib/components/Download.svelte";

    export let scriptDetails;
</script>

<div class="card">
    <h4><img src="/images/code-file.svg" alt="">{scriptDetails.name}</h4>
    <p>{scriptDetails.description}</p>
    <div class="line"></div>
    <div class="download__div">
        <Download path={scriptDetails.path} />
    </div>
</div>

<style lang="scss">
    .card{
      width: calc(32% - 2rem);
      padding: 1rem;
      border: 1px solid var(--light-gray-bg);
      border-radius: 20px;
      background-color: var(--content-bg);
      color: var(--white-text);
      font-weight: 300;
      transition: all 200ms;
      &:hover{
        background: var(--hover-menu-bg);
      }
      img{
        width: 3rem;
        margin-right: 1rem;
      }
      h4{
        display: flex;
        align-items: center;
      }
      p{
        margin-top: 1rem;
      }
      .line{
        height: 2px;
        width: 100%;
        margin-top: 1.5rem;
        background-color: var(--border-color);
        margin-bottom: 1rem;
      }
      .download__div{
        width: 100%;
        display: flex;
        justify-content: flex-end;
      }
    }
    @media screen and (max-width: 900px){
      .card{
        width: 100%;
      }
    }
</style>