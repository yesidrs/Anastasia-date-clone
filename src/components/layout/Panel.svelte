<script>
  import AsideMenu from '../utils/AsideMenu.svelte';
  import PanelContent from '../web/PanelContent.svelte';
</script>

<style>
  .panel {
    display: flex;
    justify-content: space-between;
  }
</style>

<section class="panel">
  <AsideMenu />
  <PanelContent />
</section>
