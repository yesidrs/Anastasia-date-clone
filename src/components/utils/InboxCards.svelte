<script>
  import { messages } from '../../services/inbox';
</script>

<style lang="scss">
  .inbox-card {
    margin-bottom: 1.5rem;
    .card-header {
      display: flex;
      justify-content: space-between;
      background-color: #e0ecff;
      border: 1px solid #d0d3d4;
      p {
        font-weight: 700;
        font-size: 1.4rem;
        padding: 0 2rem;
        margin: 0.5rem 0;
      }
    }
    .card-content {
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      background-color: #ffff99;
      border: 1px solid #d0d3d4;
      padding: 1rem 1rem 0 0.5rem;

      @media (max-width: 768px) {
        justify-content: space-around;
      }
      .user-image {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-left: 0.5rem;
        @media (max-width: 768px) {
          margin-left: -10px;
        }
        img {
          border: 1px solid black;
        }
        p {
          text-align: center;
          color: white;
          margin-top: 0;
          font-size: 1.3rem;
          font-weight: 500;
          width: 100%;
          border-radius: 5px;
          background: linear-gradient(
            0deg,
            #93c11a 55%,
            #a6da1d 55%
          );
        }
      }
      .user-info {
        display: flex;
        flex-direction: column;
        margin-left: 1rem;

        @media (max-width: 768px) {
          margin-left: 0;
        }
        h3 {
          text-decoration: underline;
          font-size: 1.5rem;
        }
        span {
          color: grey;
          font-size: 1.3rem;
        }
        button {
          background-color: #f5f6f6;
          color: #1b4f72;
          margin-top: 0.8rem;
          border: 1px solid #d0d3d4;
          .fa-comment {
            color: #a6da1d;
            font-size: 1.5rem;
          }
        }
        .gift {
          display: flex;
          align-items: center;
          .fa-gift {
            color: tomato;
            font-size: 2rem;
          }
          p {
            margin-left: 1rem;
            color: #1b4f72;
            font-size: 1.3rem;
            text-decoration: underline;
          }
        }
        .age {
          font-size: 1.3rem;
          margin: 0;
        }
      }
      .read-container {
        text-align: left;
        flex: 1;
        margin-left: 5rem;
        h3 {
          font-size: 1.4rem;
        }
        p {
          font-size: 1.3rem;
        }
        button {
          width: 210px;
          height: 70px;
          background: url('https://64ad.itocd.net/www/img/MailSystemEx/big-btn-free-ribbon.png?v7ab68f2a');
          background-repeat: no-repeat;
        }

        @media (max-width: 768px) {
          display: none;
        }
      }
      .actions {
        display: flex;
        flex-direction: column;
        button {
          margin-top: 1rem;
          background-color: #f5f6f6;
          color: #7b7554;
          border: 1px solid #d0d3d4;
        }
        .bg-yellow {
          background-color: #ffe870;
          border: 1px solid orange;
        }
        .bg-transparent {
          background: transparent;
          text-decoration: underline;
          color: #1b4f72;
          border: none;
        }
      }
    }
  }
</style>

{#each messages as msg}
  <div class="inbox-card">
    <div class="card-header">
      <p>{msg.name}'s First Letter</p>
      <p>Mar 14 2021</p>
    </div>
    <div class="card-content">
      <input type="checkbox" />
      <div class="user-image">
        <img src={msg.img} alt="" />
        <p>ONLINE</p>
      </div>
      <div class="user-info">
        <h3>{msg.name}</h3>
        <span>(ID: 123413698)</span>
        <button><i class="fas fa-comment" />
          Live Chat</button>
        <div class="gift">
          <i class="fas fa-gift" />
          <p>Send Virtual Gift</p>
        </div>
        <p class="age">Age: {msg.age}</p>
      </div>
      <div class="read-container">
        <h3>This letter is unread.</h3>
        <p>Click button below to read this letter.</p>
        <button>Read The Letter</button>
      </div>
      <div class="actions">
        <button>Read</button>
        <button class="bg-yellow">Reply</button>
        <button class="bg-transparent">All letters</button>
        <button class="bg-yellow">Delete</button>
      </div>
    </div>
  </div>
{/each}
