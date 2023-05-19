<script lang="ts">
    import Download from "$lib/components/Download.svelte";
    import {onMount} from "svelte";
    export let element;

    $: clicked = false;
    let numberOfImgs = element.imgs.length;
    $: currentImageIndex = 0;

    function increment():void {
        currentImageIndex<numberOfImgs-1?currentImageIndex++:currentImageIndex=0;
    }
    function decrement(): void {
        currentImageIndex>0?currentImageIndex--:currentImageIndex=numberOfImgs-1;
    }

    function minimize(): void {
        setTimeout(()=>{clicked = false},1)
    }

    $: windowWidth = 2000
    onMount(()=>{
        windowWidth = window.innerWidth;
        window.addEventListener('resize', ()=>{
            windowWidth = window.innerWidth;
        })
    })


</script>

<div class="card {clicked ? 'clicked' : ''}"  on:click={()=>{clicked = true}}>
    {#key windowWidth}
    {#if clicked || windowWidth < 1100}
    <div class="buttons">
        <button on:click={()=>decrement()}><i class="fa-solid fa-chevron-left"></i></button>
        <button on:click={()=>minimize()} style="{windowWidth<1100?'display:none':'display:flex'}"><i class="fa-solid fa-down-left-and-up-right-to-center"></i></button>
        <button on:click={()=>increment()}><i class="fa-solid fa-chevron-right"></i></button>
    </div>
    {/if}
        {/key}
    <img src={element.imgs[currentImageIndex]} alt="">
    <h3><img src="/images/code-file.svg" alt="">{element.name}</h3>
    <p>{element.description}</p>
    <div class="line"></div>
    <div class="download__div">
        <Download path={element.path}/>
    </div>
</div>



<style lang="scss">

  @media screen and (max-width: 1100px){
    .card{
      width: 100% !important;
    }
  }
  .clicked{
    width: 100%!important;
    cursor: unset!important;
  }
    .card{
      position: relative;
      cursor: pointer;
      width: calc(30% - 1rem);
      margin-bottom: 2rem;
      background-color: var(--content-bg);
      padding: 1rem;
      border-radius: 20px;
      color: var(--white-text);
      transition: background-color 200ms;
      &:hover{
        background-color: var(--light-gray-bg);
      }
      & > img{
        width: 100%;
      }
      h3{
        display: flex;
        font-size: 1.05rem;
        img{
          width: 2rem;
          margin-right: 1rem;
        }
      }
      p{
        margin-top: 1rem;
        font-size: .85rem;
      }
      .line{
        margin: 1.5rem 0;
        width: 100%;
        height: 2px;
        background-color: var(--border-color);

      }
      .download__div{
        display: flex;
        justify-content: flex-end;
      }
      .buttons{
        position: absolute;
        top: 5%;
        left: 5%;
        width: 90%;
        display: flex;
        justify-content: space-between;
        button{
          cursor: pointer;
          color: var(--white-text);
          background: transparent;
          border: none;
          outline: none;
          font-size: 2rem;
        }
      }
    }
</style>