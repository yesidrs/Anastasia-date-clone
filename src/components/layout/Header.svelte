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
          }
          .hover-border {
            &::after {
              content: '';
              width: 0%;
              height: 2px;
              background-color: yellow;
              position: absolute;
              bottom: 0%;
              left: 50%;
              border-radius: 10px;
              transition: all 500ms ease;
            }

            &:hover {
              &::after {
                left: 0%;
                width: 100%;
              }
            }
          }
        }
      }
    }
  }
</style>

<header class="header container">
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
            href="/"
            class="hover-border"
            use:link>Broadcasts</a>
          <span>|</span>
        </li>
        <li>
          <a
            href="/"
            class="hover-border"
            use:link>Inbox</a>
          <span>|</span>
        </li>
        <li>
          <a href="/" class="hover-border" use:link>My
            Profile</a>
        </li>
      </ul>
    </nav>
  </div>
</header>
