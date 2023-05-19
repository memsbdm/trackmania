<script lang="ts">
    export let documentationDetails;
</script>

<div class="row">
    <p><img src={documentationDetails.icon} alt={documentationDetails.alt}>{documentationDetails.name}</p>
    <p class="hidden__mobile">{documentationDetails.description}</p>
    <a href={documentationDetails.link} class="open">Open</a>
</div>

<style lang="scss">
  .row, .row p{
    display: flex;
    align-items: center;
  }
  .row{
    color: var(--white-text);
    font-weight: 300;
    justify-content: space-between;
    padding: .5rem 1rem;
    border-bottom: 1px solid var(--border-color);
    transition: all 200ms;
    &:hover{
      background: var(--hover-menu-bg);
    }
    &:last-of-type{
      border-bottom: none;
    }
    img{
      width: 2rem; margin-right: 1rem;
    }
    .open{
      background-color: var(--btn-blue);
      padding: .2rem 1.25rem;
      border-radius: 30px;
      color: var(--white-text);
      font-size: .95rem;
    }
  }

  @media screen and (max-width: 900px){
    .hidden__mobile{
      display: none!important;
    }
  }
</style>