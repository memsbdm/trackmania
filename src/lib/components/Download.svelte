<script lang="ts">
    export let path;

</script>

<a href={path} download>Download</a>

<style lang="scss">
    a{
      background-color: var(--btn-blue);
      color: var(--white-text);
      padding: .2rem 1.2rem;
      border-radius: 30px;
      cursor: pointer;
      font-size: .95rem;
    }
</style>