<script>
  import Menu from '../utils/Menu.svelte';

  let images = [
    'https://api4.anastasiadate.com/v2/ladies/2038015/photos/cd2ca67b42913f5a8ec9f45fc15211bba0ef30cd.316x450.gallery',
    'https://api7.anastasiadate.com/v2/ladies/2000273/photos/cc4b0b795557bc41bb9e42fb43aeec08f3c01387.316x450.gallery',
    'https://api9.anastasiadate.com/v2/ladies/1922573/photos/eeeac7c430b71446ab926e94e25c8538f6bfdc52.316x450.gallery',
    'https://api8.anastasiadate.com/v2/ladies/2047662/photos/0e7255996ee5a6d393193efbe26b11178433805b.316x450.gallery',
    'https://api3.anastasiadate.com/v2/ladies/2007244/photos/01e2c52568fb476e8e420a2754055566d0c49214.316x450.gallery',
  ];
</script>

<style lang="scss">
  .match {
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
    padding: 1rem 5rem;

    figure {
      img {
        width: 100%;
        height: 45.8rem;
        border: 1px solid #d0d3d4;
        margin-top: 1rem;
      }
    }
  }
</style>

<section>
  <div class="match">
    <Menu />
    {#each images as img}
      <figure><img src={img} alt="" /></figure>
    {/each}
  </div>
</section>
