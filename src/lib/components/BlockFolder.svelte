<script lang="ts">
    export let folders;
    export let download = false;

</script>
{#if download}
<a href="/" download=""><img src={folders.img} alt=""></a>
    {:else}
    <img src={folders.img} alt="">
{/if}
<style lang="scss">
    img{
      cursor: pointer;
      width: 6rem;
    }
</style>
