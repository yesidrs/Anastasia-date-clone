<script lang="ts">
  const date: Date = new Date();
  let actualYear: number = date.getFullYear();
</script>

<style lang="scss">
  .footer-container {
    display: flex;
    justify-content: space-between;
    background-color: #273746;
    padding: 0 2rem;
    margin-top: 2rem;

    .copy {
      display: flex;
      p {
        color: white;
        font-size: 1.2rem;
        margin-left: 0.5rem;
      }
    }

    .faq {
      display: flex;
      align-items: center;
      font-size: 1.2rem;
      p {
        color: white;
      }
      ul {
        display: flex;
        li {
          margin-left: 1rem;
          position: relative;
          span {
            color: white;
          }
        }
      }
    }
    @media (max-width: 462px) {
      flex-direction: column;
    }
  }
</style>

<footer>
  <div class="container">
    <div class="footer-container">
      <div class="copy">
        <p>Copyright AnastasiaDate 2001-{actualYear}.</p>
        <p>All rights reserved.</p>
      </div>
      <div class="faq">
        <p>General comments or question:</p>
        <ul>
          <li class="hover-border">
            <a href="#">About us</a>
            <span>|</span>
          </li>
          <li class="hover-border">
            <a href="#">Help Center</a>
            <span>|</span>
          </li>
          <li class="hover-border">
            <a href="#">Privacy Policy</a>
            <span>|</span>
          </li>
          <li class="hover-border">
            <a href="#">Terms and Conditions</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</footer>
