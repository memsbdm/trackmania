<script lang="ts">
    import '../global.scss';
    import '../variables.scss';
    import Navigation from "$lib/components/Navigation.svelte";
</script>

<div class="container">
    <Navigation />
    <slot></slot>
</div>

<style lang="scss">
    .container{
      background-color: var(--light-gray-bg);
      width: min(95vw, 1280px);
      height: 90vh;
      border-radius: 20px;
      backdrop-filter: blur(20px);
      -webkit-backdrop-filter: blur(20px);
      display: flex;
      overflow: hidden;
    }
</style>