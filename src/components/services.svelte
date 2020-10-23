<script>
</script>

<style>
  .services__shell {
    background-color: #f5f5f5;
  }
  .services__shell__uptitle::before {
    content: "";
    width: 17px;
    height: 21px;
    background-image: url("/assets/img/overline-mark.svg");
    position: absolute;
    left: -6px;
  }
  .services__shell__uptitle {
    position: relative;
  }
  .services__shell__uptitle__content {
    margin-left: 33px;
    font-size: 12px;
    line-height: 24px;
    text-transform: uppercase;
    letter-spacing: 2.5px;
    font-weight: 700;
    color: #4b4b4b;
  }
  .services__shell__title {
    font-size: 36px;
    color: #02133c;
    line-height: 42px;
    margin-top: 33px;
    font-weight: 900;
  }
  .services__shell__list__item__title {
      font-size: 19px;
      color: #02133C;
      font-weight: 900;
      text-align: center;
  }
  .services__shell__list__item {
      display: flex;
      flex-direction: column;
      background-color: #FFFFFF;
      width: 324px;
      box-sizing: border-box;
      padding: 50px 44px;
  }
  .services__shell__list__item:hover {
    transition: .4s;
    box-shadow: 0 14px 28px rgba(0,0,0,0.25), 0 10px 10px rgba(0,0,0,0.22);
  }
  .services__shell__list {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      row-gap: 24px;
      padding-top: 78px;
      padding-bottom: 150px;
  }
  .services__shell__list__item__title {
      font-size: 19px;
      padding-top: 33px;
      padding-bottom: 20px;
  }
  .services__shell__list__item__description {
      font-size: 16px;
      color: #4B4B4B;
  }
  @media (min-width: 1024px) and (max-width: 1439px) { 
    
  }
</style>

<section class="services__shell">
  <div class="container">
    <p class="services__shell__uptitle">
      <span class="services__shell__uptitle__content">Our services </span>
    </p>

    <p class="services__shell__title">Sed perspiciatis omnis iste natus</p>

    <div class="services__shell__list">
      <div class="services__shell__list__item">
        <img src="/assets/img/car_bay.svg" alt="" />
        <p class="services__shell__list__item__title">
          Multi Point Inspections
        </p>
        <p class="services__shell__list__item__description">
          At vero eos et accusamus et iusto odio dignissimos ducimus qui
          blanditiis praesentium corrupti quos dolores et quas.
        </p>
      </div>

      <div class="services__shell__list__item">
        <img src="/assets/img/car_engine.svg" alt="" />
        <p class="services__shell__list__item__title">
            Auto Repair
        </p>
        <p class="services__shell__list__item__description">
          At vero eos et accusamus et iusto odio dignissimos ducimus qui
          blanditiis praesentium corrupti quos dolores et quas.
        </p>
      </div>

      <div class="services__shell__list__item">
        <img src="/assets/img/car_breaks.svg" alt="" />
        <p class="services__shell__list__item__title">
            Auto Maintenance
        </p>
        <p class="services__shell__list__item__description">
          At vero eos et accusamus et iusto odio dignissimos ducimus qui
          blanditiis praesentium corrupti quos dolores et quas.
        </p>
      </div>

      <div class="services__shell__list__item">
        <img src="/assets/img/car_tires.svg" alt="" />
        <p class="services__shell__list__item__title">
            Tires 
        </p>
        <p class="services__shell__list__item__description">
          At vero eos et accusamus et iusto odio dignissimos ducimus qui
          blanditiis praesentium corrupti quos dolores et quas.
        </p>
      </div>

      <div class="services__shell__list__item">
        <img src="/assets/img/car_engine_check.svg" alt="" />
        <p class="services__shell__list__item__title">
            Service Warranty
        </p>
        <p class="services__shell__list__item__description">
          At vero eos et accusamus et iusto odio dignissimos ducimus qui
          blanditiis praesentium corrupti quos dolores et quas.
        </p>
      </div>

      <div class="services__shell__list__item">
        <img src="/assets/img/car_shopping.svg" alt="" />
        <p class="services__shell__list__item__title">
            Shop Online
        </p>
        <p class="services__shell__list__item__description">
          At vero eos et accusamus et iusto odio dignissimos ducimus qui
          blanditiis praesentium corrupti quos dolores et quas.
        </p>
      </div>
    </div>
  </div>
</section>
