<script>
  import InboxCards from '../utils/InboxCards.svelte';
</script>

<style lang="scss">
  .content {
    margin-top: 1rem;
    flex: 1;
    margin-left: 5rem;
    h1 {
      color: #d2202d;
      font-size: 2rem;
    }
    .info {
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: 1.4rem;
    }
    label {
      margin-right: 1rem;
    }
  }
</style>

<section class="content">
  <h1>Inbox</h1>
  <div class="info">
    <p>
      You have
      <strong>470 new messages</strong>
      out of 472 total in your inbox
    </p>
    <div>
      <label for="sort">Sort by:</label>
      <select name="sort" id="sort">
        <option>New Replies First</option>
        <option>Date (descending)</option>
        <option>Date (ascending)</option>
        <option>Name (descending)</option>
        <option>Name (ascending)</option>
        <option>City (descending)</option>
        <option>City (ascending)</option>
        <option>Age (descending)</option>
        <option>Age (ascending)</option>
      </select>
    </div>
  </div>
  <InboxCards />
</section>
