<script lang="ts">
    import BlockCard from "./BlockCard.svelte";

    export let elements;
    $: currentPage = 0;
    const numberOfPages = elements.length / 4 - 1;

    function decrement(): void{
        currentPage>=numberOfPages?currentPage--:'';
    }

    function increment(): void{
        currentPage<numberOfPages?currentPage++:'';
    }
</script>


<section class="section__container">
    <div class="buttons">
        <button on:click={()=>decrement()} ><i class="fa-solid fa-chevron-left"></i> Previous</button>
        <span>Page {currentPage+1}</span>
        <button on:click={()=>increment()}>Next <i class="fa-solid fa-chevron-right"></i></button>
    </div>
    <div class="elements__container">
        {#key currentPage}
            <BlockCard element={elements[currentPage * 4]}/>
            <BlockCard element={elements[currentPage * 4 + 1]}/>
            <BlockCard element={elements[currentPage * 4 + 2]}/>
            <BlockCard element={elements[currentPage * 4 + 3]}/>
        {/key}
    </div>
</section>



<style lang="scss">
  .section__container{
    background-color: var(--light-gray-bg);
    width: calc(90% - 3rem);
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    padding-bottom: 2rem;
    .buttons{
      padding: 1rem 0;
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 1rem;
      color: var(--white-text);
      button{
        cursor: pointer;
        color: var(--white-text);
        margin: auto;
        background: transparent;
        outline: none;
        border: none;
        font-size: 1rem;
      }
    }
  }
  .elements__container{
    overflow-y: scroll;
    padding: 0 2rem;
    display: flex;
    flex-direction: column;
    //justify-content: center;
    gap: 1rem;
  }
</style>