<template>
  <section class="home">
    <nav class="home__nav">
      <h4>Site in Development</h4>
      <p>Instagram, Twitter, Awwwards</p>
    </nav>
    <main class="home__content">
      <div class="home__content__text">
        <h3>Panthone studio © 2023</h3>
        <span>
          <p>Web Design</p>
          <p>Interaction + Animation</p>
          <p>Front + Backend Development</p>
          <p>E-commerce Websites</p>
          <p>Art Direction</p>
        </span>
      </div>
    </main>
    <footer class="home__footer">
      <p>Booking Starts by March 2023</p>
      <p>
        For enquiries, contact us at
        <a href="https://panthone.design/" target="_blank"
          >https://panthone.design</a
        >
      </p>
    </footer>
  </section>
</template>

<script lang="ts" setup></script>

<style scoped lang="scss">
.home {
  &__nav {
    @extend %flex-ac-jb;
    height: 6vh;
    padding: 0 1.5rem;
    @include respondMax("mobile2x") {
      flex-direction: column;
      justify-content: flex-start;
      align-items: flex-start;
      padding: 1rem 1.5rem;
      p {
        margin-top: 1rem;
      }
    }
    h4 {
      font-family: "PP Neue Montreal", sans-serif;
      font-style: normal;
      font-weight: 450;
      font-size: Max(1rem, 16px);
      line-height: Max(1.5rem, 20px);
      letter-spacing: 0.02em;
      font-feature-settings: "ss06" on, "ss07" on;
      color: $text;
    }
    p {
      font-family: "PP Neue Montreal", sans-serif;
      font-style: normal;
      font-weight: 450;
      font-size: Max(1rem, 16px);
      line-height: Max(1.5rem, 20px);
      text-align: right;
      letter-spacing: 0.02em;
      text-decoration-line: underline;
      font-feature-settings: "ss06" on, "ss07" on;
      color: $text;
    }
  }
  &__content {
    height: calc(100vh - 13vh);
    @extend %center;
    padding: 0 1.5rem;
    &__text {
      width: Min(949px, 100%);
      text-align: center;
      h3 {
        font-family: "PP Neue Montreal", sans-serif;
        font-style: normal;
        font-weight: 450;
        font-size: Max(6rem, 30px);
        line-height: Max(6.1rem, 30px);
        letter-spacing: -0.04em;
        font-feature-settings: "ss06" on, "ss07" on;
        color: $text;
        @media screen and (max-width: 500px) {
          font-size: 40px;
        }
      }
      span {
        @extend %flex-ac-jb;
        margin-top: 0.5rem;
        flex-wrap: wrap;
        @media screen and (max-width: 900px) {
          flex-direction: column;
          gap: 1rem;
          justify-content: center;
        }
        p {
          font-family: "PP Neue Montreal", sans-serif;
          font-style: normal;
          font-weight: 450;
          font-size: Max(1rem, 16px);
          line-height: Max(1.5rem, 20px);
          letter-spacing: 0.02em;
          font-feature-settings: "ss06" on, "ss07" on;
          color: $text;
        }
      }
    }
  }
  &__footer {
    height: 7vh;
    text-align: center;
    width: 100vw;
    margin: 0 auto;
    padding: 0 1.5rem;
    p {
      font-family: "PP Neue Montreal", sans-serif;
      font-style: normal;
      font-weight: 450;
      font-size: Max(1rem, 16px);
      line-height: Max(1.5rem, 20px);
      letter-spacing: 0.02em;
      font-feature-settings: "ss06" on, "ss07" on;
      color: $text;
    }
  }
}
</style>
