<script>
  
</script>

<style>
  .header-shell {
    background-image: url("/assets/img/header-background.png");
    background-size: cover;
  }
  .header-shell__upper-content__navigation-wrapper__info-section__title {
    font-size: 20px;
    color: #ffffff;
  }
  .header-shell__upper-content {
    margin: 0 auto;
    max-width: 1020px;
    padding-top: 26px;
  }
  .header-shell__upper-content__navigation-wrapper__info-section {
    display: flex;
    justify-content: space-between;
  }
  .header-shell__upper-content__navigation-wrapper__info-section__services-wrapper {
    display: flex;
  }
  .header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__appointment-btn {
    background-color: #e30b0b;
    box-sizing: border-box;
    border: none;
    color: #ffffff;
    font-size: 12px;
    text-transform: uppercase;
    padding: 9px 30px;
    line-height: 24px;
    letter-spacing: 1px;
    margin-left: 32px;
  }
  .header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__call-us,
  .header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__hours {
    display: flex;
    flex-direction: row;
    margin-left: 32px;
  }
  .header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__call-us__title {
    font-size: 14px;
    line-height: 22px;
    text-transform: uppercase;
    letter-spacing: 1px;
  }
  .header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__call-us__phone-image,
  .header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__hours__clock-image {
    padding-top: 5px;
    align-self: flex-start;
  }
  .title-number-shell,
  .hours-duration-shell {
    display: flex;
    flex-direction: column;
    margin-left: 12px;
    color: #ffffff;
  }
  .header-shell__down-content {
    margin-top: 126px;
  }
  .header-shell__down-content__action-button {
    margin: 48px 0 300px;
    background-color: #e30b0b;
    box-sizing: border-box;
    border: none;
    color: #ffffff;
    font-size: 12px;
    text-transform: uppercase;
    padding: 9px 30px;
    line-height: 24px;
    letter-spacing: 1px;
  }
  .header-shell__upper-content__navigation-wrapper__main-navigation {
    background-color: #ffffff;
    padding: 17px 0;
    margin-top: 28px;
  }
  .header-shell__upper-content__navigation-wrapper__main-navigation__list {
    display: flex;
    justify-content: space-evenly;
  }
  .header-shell__upper-content__navigation-wrapper__main-navigation__list__item {
    font-size: 14px;
    line-height: 22px;
    letter-spacing: 1px;
    color: #02133C;
  }
  .header-shell__upper-content__navigation-wrapper__main-navigation a {
    color: #02133C;
    text-transform: uppercase;
  }
  .header-shell__down-content__title {
    font-size: 56px;
    max-width: 583px;
    color: #ffffff;
    line-height: 56px;
  }
</style>

<header class="header-shell">
  <div class="header-shell__upper-content">
    <div class="header-shell__upper-content__navigation-wrapper">
      <div
        class="header-shell__upper-content__navigation-wrapper__info-section">
        <div
          class="header-shell__upper-content__navigation-wrapper__info-section__title">
          company title
        </div>

        <div
          class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper">
          <div
            class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__hours">
            <img
              class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__hours__clock-image"
              src="./assets/img/phone_24px.svg"
              alt="" />
            <div class="hours-duration-shell">
              <span
                class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__hours__title">
                Service hours
              </span>
              <span
                class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__hours__duration">
                Mon - Sat: 7:00 am - 6:00 pm
              </span>
            </div>
          </div>

          <div
            class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__call-us">
            <img
              class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__call-us__phone-image"
              src="./assets/img/phone_24px.svg"
              alt="" />
            <div class="title-number-shell">
              <span
                class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__call-us__title">
                Call us
              </span>

              <span
                class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__call-us__number">
                phone number
              </span>
            </div>
          </div>
          <button
            class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__appointment-btn">
            Make an appointment
          </button>
        </div>
      </div>
      <nav
        class="header-shell__upper-content__navigation-wrapper__main-navigation">
       <ul class="header-shell__upper-content__navigation-wrapper__main-navigation__list">
         <li class="header-shell__upper-content__navigation-wrapper__main-navigation__list__item"><a href="#">Services</a></li>
         <li class="header-shell__upper-content__navigation-wrapper__main-navigation__list__item"><a href="#">Specials</a></li>
         <li class="header-shell__upper-content__navigation-wrapper__main-navigation__list__item"><a href="#">Estimates</a></li>
         <li class="header-shell__upper-content__navigation-wrapper__main-navigation__list__item"><a href="#">Reviews</a></li>
         <li class="header-shell__upper-content__navigation-wrapper__main-navigation__list__item"><a href="#">About</a></li>
         <li class="header-shell__upper-content__navigation-wrapper__main-navigation__list__item"><a href="#">Contact</a></li>
       </ul>
      </nav>
    </div>

    <div class="header-shell__down-content">
      <p class="header-shell__down-content__title">
        Top notch service is our main auto motive
      </p>
      <button class="header-shell__down-content__action-button">
        Make an appointment
      </button>
    </div>
  </div>
</header>
