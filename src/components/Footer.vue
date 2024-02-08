<template>
  <div class="footer">
    <div class="container">
      <div class="footer_top">
        <form action="">
          <input type="text" id="name" name="name" placeholder="NAME" />
          <input type="email" id="email" name="email" placeholder="EMAIL" />
          <textarea
            name="message"
            cols="40"
            rows="5"
            placeholder="MESSAGE"
          ></textarea>
          <input type="submit" value="SEND MESSAGE" />
        </form>
      </div>
      <hr />
      <div class="footer_bottom">
        <div>julianeschmidt</div>
        <div class="links">
          <a href="https://github.com/juli91" target="_blank"
            ><img src="../assets/images/github.svg" alt="Github"
          /></a>
          <a href="" target="_blank"
            ><img
              src="../assets/images/frontendmentor.svg"
              alt="Frontend Mentor"
          /></a>
          <a href="" target="_blank"
            ><img src="../assets/images/linkedin.svg" alt="LinkedIn"
          /></a>
          <a href="" target="_blank"
            ><img src="../assets/images/instagram.svg" alt="Instagram"
          /></a>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.footer {
  background-color: var(--dark-grey);
  padding-bottom: 3rem;

  &_bottom {
    display: flex;
    justify-content: space-between;
    padding-top: 1rem;

    .links {
      display: flex;
      gap: 1rem;

      img {
        width: 1.5rem;
        height: 1.5rem;
      }
    }
  }

  hr {
    color: var(--secondary);
  }

  form {
    display: flex;
    flex-direction: column;

    input,
    textarea {
      background: transparent;
      border-top: none;
      border-left: none;
      border-right: none;
      border-color: white;
    }
  }
}
</style>
