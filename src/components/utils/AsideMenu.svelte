<style lang="scss">
  aside {
    padding-top: 3rem;
    margin-left: 1rem;
    .btn-subscribe {
      background-color: #9bcb1b;
      color: white;
      font-size: 1.7rem;
      padding: 0.2rem 4rem;
      box-shadow: 0px 5px 15px -5px rgba(0, 0, 0, 0.5);
      border-radius: 8px;
    }
    .menu {
      .option {
        margin-top: 3rem;
        h2 {
          color: #d2202d;
        }
        li {
          display: flex;
          align-items: center;
          justify-content: space-between;
          color: #1b4f72;
          margin-top: 0.7rem;
          a {
            color: #1b4f72;
            position: relative;
            font-size: 1.5rem;
          }
          p {
            font-weight: 700;
            background-color: #f0f3f4;
            padding: 0.1rem 0.5rem;
          }
        }

        .hover-border-blue {
          &::after {
            content: '';
            width: 0%;
            height: 2px;
            background-color: #1b4f72;
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

      figure {
        margin-top: 2rem;
      }
    }
  }
</style>

<aside>
  <button class="btn-subscribe">Subscribe</button>
  <div class="menu">
    <div class="option">
      <h2>Emails</h2>
      <ul>
        <li>
          <a href="#" class="hover-border-blue">Inbox</a>
          <p>470</p>
        </li>
        <li>
          <a href="#" class="hover-border-blue">Sent Mail</a>
        </li>
        <li>
          <a href="#" class="hover-border-blue">Deleted Mail</a>
        </li>
        <li>
          <a href="#" class="hover-border-blue">Compose New
            Mail</a>
        </li>
      </ul>
    </div>
    <div class="option">
      <h2>Ladies</h2>
      <ul>
        <li>
          <a href="#" class="hover-border-blue">Online
            Ladies</a>
          <p>2979</p>
        </li>
        <li>
          <a href="#" class="hover-border-blue">My Contact
            List</a>
        </li>
        <li>
          <a href="#" class="hover-border-blue">Search</a>
        </li>
      </ul>
    </div>
    <div class="option">
      <h2>Services</h2>
      <ul>
        <li>
          <a href="#" class="hover-border-blue">Live Chat</a>
        </li>
        <li>
          <a href="#" class="hover-border-blue">CamShare</a>
        </li>
        <li>
          <a href="#" class="hover-border-blue">Virtual
            Gifts</a>
        </li>
        <li>
          <a href="#" class="hover-border-blue">Flowers &
            Presents</a>
        </li>
        <li>
          <a href="#" class="hover-border-blue">Call Me</a>
        </li>
      </ul>
    </div>
    <figure>
      <img
        src="https://44ad.itocd.net/www/extBanners/431f819a433945248d408a8b82239f57.jpg"
        alt="" />
    </figure>
  </div>
</aside>
