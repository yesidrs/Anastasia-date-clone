<script lang="ts">
  import Menu from '../utils/Menu.svelte';
  import { users } from '../../services/users';
</script>

<style lang="scss">
  .match {
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
    padding: 1rem 1rem;
    border: 1px solid #d0d3d4;
    box-shadow: 0px 2px 15px 1px rgba(0, 0, 0, 0.5);

    figure {
      position: relative;
      img {
        width: 100%;
        height: 45.8rem;
        border: 1px solid #d0d3d4;
        margin-top: 1rem;
      }
      p {
        position: absolute;
        margin-left: 0;
        margin-right: 0;
        left: 0;
        right: 0;
        bottom: 60px;
        text-align: center;
        color: white;
        font-size: 3rem;
        text-shadow: 2px 2px 2px black;
      }
      button {
        color: white;
        font-weight: 500;
        bottom: 23px;
        padding: 0.6rem 1rem;
        border-radius: 8px;
        z-index: 1;
        i {
          margin-right: 1rem;
        }
        &:first-of-type {
          position: absolute;
          left: 20px;
          background-color: #005cc3;
        }
        &:last-of-type {
          position: absolute;
          right: 20px;
          background-color: #9ccd1b;
        }
      }

      &::after {
        content: '';
        width: 100%;
        height: 15%;
        position: absolute;
        bottom: 0;
        left: 0;
        background: linear-gradient(
          to top,
          black,
          rgba(black, 0)
        );
        opacity: 0.9;
      }
    }
  }
</style>

<section>
  <div class="match">
    <Menu />
    {#each users as user}
      <figure>
        <img src={user.img} alt="" />
        <p>{user.name}, {user.age}</p>
        <button>
          <i class="fas fa-video" />Cam Share</button>
        <button>
          <i class="fas fa-comment" />Live Chat</button>
      </figure>
    {/each}
  </div>
</section>
