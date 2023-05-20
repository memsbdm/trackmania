<script lang="ts">
    import BlockFolder from "./BlockFolder.svelte";

    export let element;
    $: folderClicked = false;
    $: subFolderClicked = false;
    $: folderIndex = 0;
    $: subFolderIndex = 0;
    function handleFolderClick(i): void {
        folderClicked = true;
        folderIndex = i;
    }

    function handleSubFolderClick(i): void {
        subFolderClicked = true;
        subFolderIndex = i;
    }

    function handleReturnClick(): void {
        if(subFolderClicked)
            subFolderClicked = false;
        else if(folderClicked)
            folderClicked = false;
    }
</script>

<div class="card">
    <div class="header">
<!--        <button on:click={()=>handleReturnClick()} style="{folderClicked || subFolderClicked? 'visibility: unset': 'visibility:hidden'}">-->
<!--            <img src="/images/GreyArrow.png" alt="" class="return"></button>-->
        <button on:click={()=>handleReturnClick()} style="{folderClicked || subFolderClicked? 'visibility: unset': 'visibility:hidden'}">
            <div class="return__img"></div></button>
        <h3>{element.name}</h3>
    </div>

    {#key folderClicked}
    {#if !folderClicked}
        <div class="container">
    {#each element.folders as folders, index}
            <div on:click={()=>handleFolderClick(index)}>
                <BlockFolder {folders} />
            </div>
    {/each}
        </div>
        {:else if folderClicked && !subFolderClicked}
        <div class="container">
        {#each element.folders[folderIndex].subfolders as folders, index}
            <div on:click={()=>handleSubFolderClick(index)}>
                <BlockFolder {folders} />
            </div>
        {/each}
        </div>
        {:else}
        <div class="container">
            {#each element.folders[folderIndex].subfolders[subFolderIndex].items as folders, index}
                <div>
                    <BlockFolder {folders} download="true"/>
                </div>
            {/each}
        </div>
        {/if}
        {/key}
    <p>{element.description}</p>
</div>

<style lang="scss">
  .container{
    display: flex;
    flex-wrap: wrap;
  }
  .return__img{
    width: 2rem;
    height: 2rem;
    background-image: url("/images/GreyArrow.png");
    background-size: contain;
    background-position: center;
    &:hover{
      background-image: url("/images/BlueArrow.png");
    }
  }
    .card{
      background-color: var(--content-bg);
      border-radius: 10px;
      padding: 0 1rem;
      transition: all 200ms;
      p{
        color: var(--white-text);
        opacity: .6;
        padding: 1rem 0;
      }
      &:hover{
        background-color: var(--light-gray-bg);
      }
      .header{
        display: flex;
        justify-content: space-between;
        padding: 1rem 0;
        h3{
          color: var(--white-text);
        }
        button{
          cursor: pointer;
          background: transparent;
          outline: none;
          border: none;
          font-size: 1rem;
          color: var(--white-text);
        }
      }
      .container{
        display: flex;
      }
    }
</style>