<section>
    <div class="header">
        <p class="hidden__mobile">Choose the version of Unlimiter:</p>
        <a href="/unlimiter" style="{$page.url.href.endsWith('/unlimiter')?'color:var(--btn-blue)':''}">Version 1.3</a>
        <a href="/unlimiter/1-2" style="{$page.url.href.endsWith('/unlimiter/1-2')?'color:var(--btn-blue)':''}">Version 1.2</a>
        <a href="/unlimiter/1-1" style="{$page.url.href.endsWith('/unlimiter/1-1')?'color:var(--btn-blue)':''}">Version 1.1</a>
    </div>
    <slot />
</section>

<style lang="scss">
  section{
    background: var(--light-gray-bg);
    display: flex;
    flex-direction: column;
    align-items: center;
    overflow-y: scroll;
  }
    .header{
      display: flex;
      justify-content: space-evenly;
      width: calc(min(95vw, 1280px) - 180px);
      color: var(--white-text);
      p, a{
        margin: 2rem 0;
        transition: all 200ms;
      };
    }
    @media screen and (max-width: 900px){
      .hidden__mobile{
        display: none;
      }
    }
</style>

<script lang="ts">
    import { page } from '$app/stores';
</script>