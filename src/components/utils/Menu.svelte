<style lang="scss">
  .menu {
    display: flex;
    justify-content: space-between;
    align-items: center;

    .options {
      display: flex;
      flex-direction: column;
      border: 1px solid #d0d3d4;
      .title {
        font-size: 2.5rem;
        text-align: center;
        padding: 2rem 0;
      }

      .group {
        display: flex;
        align-items: center;
        justify-content: center;
        .option {
          display: flex;
          flex-direction: column;
          align-items: center;
          padding: 1.5rem 1.5rem 0.5rem 1.5rem;
          text-align: center;
          color: black;
          width: 7.4rem;
          height: 9.4rem;
          border: 1px solid #d0d3d4;
          i {
            font-size: 3rem;
            margin-bottom: 1rem;
          }
          span {
            font-size: 1.5rem;
          }
        }
      }
    }
  }
</style>

<div class="menu">
  <div class="options">
    <h1 class="title">At the moment <br /> you have</h1>
    <div class="group">
      <a href="/" class="option">
        <i class="far fa-envelope" />
        <span>New <br /> Emails</span>
      </a>
      <a href="/" class="option">
        <i class="fas fa-user-friends" />
        <span>Online <br /> Members</span>
      </a>
      <a href="/" class="option">
        <i class="far fa-star" />
        <span>Contact <br /> List</span>
      </a>
    </div>
    <div class="group">
      <a href="/" class="option">
        <i class="fas fa-phone" />
        <span>Phone <br /> Calls</span>
      </a>
      <a href="/" class="option">
        <i class="fas fa-gift" />
        <span>Virtual <br /> Gifts</span>
      </a>
      <a href="/" class="option">
        <i class="fas fa-glass-cheers" />
        <span>Delivered <br /> Orders</span>
      </a>
    </div>
    <div class="group">
      <a href="/" class="option">
        <i class="far fa-question-circle" />
        <span>Help <br /> Center</span>
      </a>
      <a href="/" class="option">
        <i class="far fa-check-circle" />
        <span>Bonus <br /> Points</span>
      </a>
      <a href="/" class="option">
        <i class="fas fa-fire" />
        <span>Subscribe</span>
      </a>
    </div>
  </div>
</div>
