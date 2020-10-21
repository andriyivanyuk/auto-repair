<script>
  export let backdrop;
  let mobileNav;

  
  $: if (backdrop) {
    toggleNav()
  }



  const toggleNav = () => {
   mobileNav.style.display = "block";
   console.log('test2', backdrop);
  }
</script>

<style>
  .header-shell {
    background-image: url("/assets/img/header-background.png");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: right top;
  }
  .header-shell__upper-content__navigation-wrapper__info-section__title {
    font-size: 20px;
    color: #ffffff;
    align-self: center;
    margin-right: 36px;
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
    background-color: #c40b0b;
    box-sizing: border-box;
    border: none;
    color: #ffffff;
    font-size: 12px;
    text-transform: uppercase;
    padding: 9px 30px;
    line-height: 24px;
    letter-spacing: 1px;
    margin-left: 32px;
    font-weight: 700;
  }
  .header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__call-us,
  .header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__hours {
    display: flex;
    flex-direction: row;
    margin-left: 32px;
  }
  .header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__call-us__title {
    font-size: 14px;
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
    text-transform: uppercase;
    font-size: 14px;
    line-height: 1.5;
  }
  .header-shell__down-content {
    margin-top: 126px;
  }
  .header-shell__down-content__action-button {
    margin: 48px 0 250px;
    background-color: #c40b0b;
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
    color: #02133c;
  }
  .header-shell__upper-content__navigation-wrapper__main-navigation a {
    color: #02133c;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-weight: 600;
  }
  .header-shell__down-content__title {
    font-size: 56px;
    max-width: 583px;
    color: #ffffff;
    line-height: 56px;
    font-weight: 900;
  }
  .header__shell__mobile-navigation {
    display: none;
    position: fixed;
    z-index: 20;
    top: 0;
    left: 0;
    background: white;
    width: 80%;
    height: 100vh;
  }
  .toggle-button {
  width: 3rem;
  background: transparent;
  border: none;
  cursor: pointer;
  padding-top: 0;
  padding-bottom: 0;
  vertical-align: middle;
}

.toggle-button:focus {
  outline: none;
}

.toggle-button__bar {
  width: 100%;
  height: 0.2rem;
  background: white;
  display: block;
  margin: 0.6rem 0;
}


  @media (min-width: 1024px) and (max-width: 1439px) {
    .header-shell__upper-content {
      max-width: 920px;
    }
  }
  @media (min-width: 768px) and (max-width: 1023px) {
    .header-shell__upper-content {
      max-width: 720px;
    }
    .header-shell__down-content__title {
      align-self: flex-end;
      font-size: 50px;
    }
    .header-shell__down-content {
      display: flex;
      flex-direction: column;
    }
    .header-shell__down-content__action-button {
      width: 61%;
      align-self: center;
    }
    .header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__appointment-btn {
      display: none;
    }
    .header-shell__upper-content__navigation-wrapper__info-section {
      justify-content: initial;
    }
    .header-shell__upper-content__navigation-wrapper__info-section__title {
      margin-left: 16px;
    }
    .header-shell__upper-content__navigation-wrapper__main-navigation__list__item {
      font-size: 11px;
    }
  }
</style>

<header class="header-shell">
  <div class="header-shell__upper-content">
    <div class="header-shell__upper-content__navigation-wrapper">
      <div
        class="header-shell__upper-content__navigation-wrapper__info-section">
        <button
           on:click={toggleNav}
           class="toggle-button">
          <span class="toggle-button__bar" />
          <span class="toggle-button__bar" />
          <span class="toggle-button__bar" />
        </button>
        <img src="/assets/img/logo.svg" alt="" />
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
                Часы работы
              </span>
              <span
                class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__hours__duration">
                Пн - Суб: 9:00 - 20:00
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
                Свяжитесь с нами
              </span>

              <span
                class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__call-us__number">
                +38 068-228-4467
              </span>
            </div>
          </div>
          <button
            class="header-shell__upper-content__navigation-wrapper__info-section__services-wrapper__appointment-btn">
            Назначить встречу
          </button>
        </div>
      </div>
      <nav
        class="header-shell__upper-content__navigation-wrapper__main-navigation">
        <ul
          class="header-shell__upper-content__navigation-wrapper__main-navigation__list">
          <li
            class="header-shell__upper-content__navigation-wrapper__main-navigation__list__item">
            <a href="#">Главная</a>
          </li>
          <li
            class="header-shell__upper-content__navigation-wrapper__main-navigation__list__item">
            <a href="#">О Нас</a>
          </li>
          <li
            class="header-shell__upper-content__navigation-wrapper__main-navigation__list__item">
            <a href="#">Преимущества</a>
          </li>
          <li
            class="header-shell__upper-content__navigation-wrapper__main-navigation__list__item">
            <a href="#">Наши работы</a>
          </li>
          <li
            class="header-shell__upper-content__navigation-wrapper__main-navigation__list__item">
            <a href="#">Услуги</a>
          </li>
          <li
            class="header-shell__upper-content__navigation-wrapper__main-navigation__list__item">
            <a href="#">Контакт</a>
          </li>
        </ul>
      </nav>

      <nav 
         bind:this={mobileNav}
         class="header__shell__mobile-navigation">
        <ul class="header__shell__mobile-navigation__list">
          <li class="header__shell__mobile-navigation__list__item">
            <a href="#">Главная</a>
          </li>
          <li class="header__shell__mobile-navigation__list__item">
            <a href="#">О Нас</a>
          </li>
          <li class="header__shell__mobile-navigation__list__item">
            <a href="#">Преимущества</a>
          </li>
          <li class="header__shell__mobile-navigation__list__item">
            <a href="#">Наши работы</a>
          </li>
          <li class="header__shell__mobile-navigation__list__item">
            <a href="#">Услуги</a>
          </li>
          <li class="header__shell__mobile-navigation__list__item">
            <a href="#">Контакт</a>
          </li>
        </ul>
      </nav>
    </div>

    <div class="header-shell__down-content">
      <p class="header-shell__down-content__title">
        Тонировка и химчистка авто
      </p>
      <button class="header-shell__down-content__action-button">
        Назначить встречу
      </button>
    </div>
  </div>
</header>
