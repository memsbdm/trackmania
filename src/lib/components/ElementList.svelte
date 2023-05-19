<script lang="ts">
    import ElementCard from "$lib/components/ElementCard.svelte";

    export let elements;
    $: currentPage = 0;
    const numberOfPages = elements.length / 6 - 1;

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
        <ElementCard element={elements[currentPage * 6]}/>
        <ElementCard element={elements[currentPage * 6 + 1]}/>
        <ElementCard element={elements[currentPage * 6 + 2]}/>
        <ElementCard element={elements[currentPage * 6 + 3]}/>
        <ElementCard element={elements[currentPage * 6 + 4]}/>
        <ElementCard element={elements[currentPage * 6 + 5]}/>
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
      justify-content: center;
      gap: 1rem;
      flex-wrap: wrap;
    }
</style>