<script>
  import { link } from 'svelte-routing';
</script>

<style lang="scss">
  .header {
    padding-top: 2rem;
    figure {
      width: 30rem;
    }
    .navigation {
      background-color: tomato;
      margin-top: 2rem;
      padding: 1rem;
      .nav-items {
        display: flex;
        justify-content: flex-end;
        color: white;
        font-size: 1.5rem;
        font-weight: 500;
        li {
          margin-right: 1.2rem;
          span {
            margin-left: 1rem;
          }
        }
      }
    }
  }
</style>

<header class="header container">
  <figure class="logo">
    <img src="/img/logo.png" alt="" />
  </figure>
  <nav class="navigation">
    <ul class="nav-items">
      <li>
        <a href="/" use:link>My account</a>
        <span>|</span>
      </li>
      <li>
        <a href="/" use:link>Broadcasts</a>
        <span>|</span>
      </li>
      <li>
        <a href="/" use:link>Search </a>
        <span>|</span>
      </li>
      <li><a href="/" use:link>My Profile</a></li>
    </ul>
  </nav>
</header>
