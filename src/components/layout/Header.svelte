<script>
  import { link } from 'svelte-routing';
</script>

<style lang="scss">
  .header {
    background-image: url('//51ad.itocd.net/www/img/header.jpg?6010&v0688a30a');
    background-position: center right;
    background-repeat: no-repeat;
    background-size: cover;
    padding-top: 2rem;
    figure {
      width: 30rem;
      padding-left: 2rem;
    }
    .nav-container {
      background-color: tomato;
      padding: 0.2rem 0;
      margin-top: 1rem;
      .navigation {
        background-image: url('/img/border_horizontal.png'),
          url('/img/border_horizontal.png');
        background-repeat: repeat-x;
        background-position: 0px top, 0px bottom;
        padding: 1rem;
        .nav-items {
          display: flex;
          justify-content: flex-end;
          align-items: center;
          color: white;
          font-size: 1.5rem;
          font-weight: 500;
          li {
            margin-right: 1.2rem;
            a {
              position: relative;
            }
            span {
              margin-left: 1rem;
            }

            &:last-of-type {
              i {
                font-size: 1.6rem;
                border: 1px solid #d0d3d4;
                padding: 0.5rem;
                background-color: #d0d3d4;
                border-radius: 6px;
              }
            }
          }
        }
      }
    }
  }
</style>

<header class="header container" id="header">
  <figure class="logo">
    <img
      src="//7ad.itocd.net/www/Specials/img/logo-anastasia-global.png"
      alt="" />
  </figure>
  <div class="nav-container">
    <nav class="navigation">
      <ul class="nav-items">
        <li>
          <a href="/" class="hover-border" use:link>Home</a>
          <span>|</span>
        </li>
        <li>
          <a
            href="broadcasts"
            class="hover-border"
            use:link>Broadcasts</a>
          <span>|</span>
        </li>
        <li>
          <a
            href="inbox"
            class="hover-border"
            use:link>Inbox</a>
          <span>|</span>
        </li>
        <li>
          <i class="fas fa-user" />
          <a href="/" class="hover-border" use:link>My
            Profile</a>
        </li>
      </ul>
    </nav>
  </div>
</header>
