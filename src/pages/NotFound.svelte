<style lang="scss">
  .error_404 {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: white;
    height: 100vh;

    .content {
      display: flex;
      justify-content: center;
      align-items: center;

      .title {
        h1 {
          color: #84b9ff;
          font-size: 2.8rem;
        }
        p {
          font-size: 2.4rem;
        }
      }
      @media (max-width: 425px) {
        flex-direction: column-reverse;

        .title {
          text-align: center;
        }
      }
    }
  }
</style>

<section class="error_404">
  <div class="container">
    <div class="content">
      <div class="title">
        <h1>Oops!... Al parecer te has perdido</h1>
        <p>dale click aca abajo nosotros te guiamos</p>
        <a href="/" class="btn-primary link">Pagina Principal</a>
      </div>
      <figure><img src="/img/404.jpg" alt="Pagina Error 404" /></figure>
    </div>
  </div>
</section>
