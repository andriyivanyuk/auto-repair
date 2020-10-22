<script>
</script>

<style>
  .footer__shell {
    padding: 90px 90px;
  }
  .footer__shell__elements {
    display: flex;
    justify-content: space-between;
  }
  .footer__shell__elements__general-content__title {
    display: flex;
    align-items: center;
  }
  .footer__shell__elements__general-content__title-content {
    font-size: 24px;
    color: #02133c;
    margin-left: 10px;
  }
  .footer__shell__elements__general-content__description {
    margin-top: 23px;
    max-width: 235px;
    font-size: 16px;
    color: #4b4b4b;
    letter-spacing: 0.5px;
  }
  .footer__shell__elements__general-content__social-links {
    margin-top: 33px;
    max-width: 150px;
    display: flex;
    justify-content: space-between;
  }
  .footer__shell__elements__explore-links__title {
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 0.15px;
    color: #4b4b4b;
    font-weight: 700;
  }
  .footer__shell__elements__explore-links__list li:nth-child(1n + 2) {
    margin-top: 11px;
  }
  .footer__shell__elements__explore-links__list li {
    font-size: 14px;
    line-height: 22px;
  }
  .footer__shell__elements__contact__list__item {
    display: flex;
  }
  .footer__shell__elements__explore-links__list li:first-child {
    margin-top: 28px;
  }
  .footer__shell__elements__explore-links__list li a {
    color: #4b4b4b;
    font-weight: 700;
  }
  .footer__shell__elements__contact__list__item-description {
    max-width: 226px;
    margin-left: 18px;
    line-height: 1.5;
    color: #4b4b4b;
  }
  .footer__shell__elements__contact__list__item:nth-child(1n + 2) {
    margin-top: 16px;
  }
  .footer__shell__elements__contact__list__item:first-child {
    margin-top: 28px;
  }
  .footer__shell__elements__contact__title {
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 0.5px;
    font-weight: 700;
  }
  .footer__copyright {
    color: #959595;
    background-color: #02133c;
    padding: 22px 22px;
  }
  .align-copyright {
    display: flex;
    justify-content: space-between;
  }
  @media (max-width: 767px) {
    .footer__shell__elements {
      flex-direction: column;
    }
  }
</style>

<footer class="footer__shell">
  <div class="container">
    <div class="footer__shell__elements">
      <div class="footer__shell__elements__general-content">
        <div class="footer__shell__elements__general-content__title">
          <img
            class="footer__shell__elements__general-content__title-image"
            src="/assets/img/logo.svg"
            alt="" />
          <span
            class="footer__shell__elements__general-content__title-content">Company
            name
          </span>
        </div>
        <p class="footer__shell__elements__general-content__description">
          This is a blurb about the company sed do eiusmod tempor incididunt ut
          labore et dolore ex magna aliqua.
        </p>
        <div class="footer__shell__elements__general-content__social-links">
          <a href="/"><img src="/assets/img/facebook-link.svg" alt="" /></a>
          <a href="/"><img src="/assets/img/twitter-link.svg" alt="" /></a>
          <a href="/"><img src="/assets/img/instagram-link.svg" alt="" /></a>
          <a href="/"><img src="/assets/img/youtube-link.svg" alt="" /></a>
        </div>
      </div>
      <div class="footer__shell__elements__explore-links">
        <p class="footer__shell__elements__explore-links__title">
          Explore links
        </p>
        <ul class="footer__shell__elements__explore-links__list">
          <li><a href="/">About</a></li>
          <li><a href="/">Services</a></li>
          <li><a href="/">Specials</a></li>
          <li><a href="/">Estimates</a></li>
        </ul>
      </div>
      <div class="footer__shell__elements__contact">
        <p class="footer__shell__elements__contact__title">Contact</p>
        <ul class="footer__shell__elements__contact__list">
          <li class="footer__shell__elements__contact__list__item">
            <img
              class="footer__shell__elements__contact__list__item-image"
              src="/assets/img/place.svg"
              alt="" />
            <p class="footer__shell__elements__contact__list__item-description">
              321 Pikes Place Parkway Seattle, WA 54321
            </p>
          </li>

          <li class="footer__shell__elements__contact__list__item">
            <img
              class="footer__shell__elements__contact__list__item-image"
              src="/assets/img/smartphone.svg"
              alt="" />
            <p class="footer__shell__elements__contact__list__item-description">
              (555) 765-4321
            </p>
          </li>

          <li class="footer__shell__elements__contact__list__item">
            <img
              class="footer__shell__elements__contact__list__item-image"
              src="/assets/img/email.svg"
              alt="" />
            <p class="footer__shell__elements__contact__list__item-description">
              Info@company.com
            </p>
          </li>

          <li class="footer__shell__elements__contact__list__item">
            <img
              class="footer__shell__elements__contact__list__item-image"
              src="/assets/img/timer.svg"
              alt="" />
            <p class="footer__shell__elements__contact__list__item-description">
              Mon - Sat: 7:000 am - 6:00 pm
            </p>
          </li>
        </ul>
      </div>
    </div>
  </div>
</footer>
<section class="footer__copyright">
  <div class="container align-copyright">
    <p class="footer__copyright__title">
      Tagline lorem ipsum dolor sit amet, consectetur adipiscing eiusmod
    </p>
    <p class="footer__copyright__privacy">
      © 2018 Company. Privacy Policy | Terms & Conditions
    </p>
  </div>
</section>
