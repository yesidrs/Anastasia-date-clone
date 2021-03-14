<script lang="ts">
  import LiveCards from '../utils/LiveCards.svelte';

  let selected: boolean = true;

  const toggle = (select: boolean): void => {
    selected = select;
  };
</script>

<style lang="scss">
  .options {
    display: flex;
    align-items: center;
    margin: 2rem;
    p {
      font-size: 1.5rem;
    }

    button {
      position: relative;
      margin-left: 1rem;
      background-color: white;
      font-size: 1.6rem;
      &::after {
        content: '';
        width: 0%;
        height: 2px;
        background-color: tomato;
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
</style>

<section>
  <div class="options">
    <p>Show:</p>
    <button on:click={() => toggle(true)}>All</button>
    <button
      on:click={() => toggle(false)}>Following</button>
  </div>
  <LiveCards {selected} />
</section>
