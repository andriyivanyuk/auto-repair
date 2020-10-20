<script>
  let name;
  let email;
  let phoneNumber;

  const handleSubmit = () => {
    console.log(name, email, phoneNumber)
  }

</script>

<style>
  .appointment__shell {
    padding: 130px 130px;
    background-color: #02133c;
  }
  .align-form-elements {
    display: flex;
    justify-content: space-between;
  }
  .appointment__shell__main-form {
    background-color: #ffffff;
    padding: 76px 58px 154px 58px;
    width: 585px;
    box-sizing: border-box;
  }
  .appointment__shell__main-form::placeholder {
    font-size: 16px;
    color: red;
  }
  .appointment__shell__main-form__title {
    font-size: 36px;
    color: #02133c;
    padding-bottom: 48px;
    font-weight: 900;
  }
  .row {
    display: flex;
    justify-content: space-between;
    column-gap: 22px;
  }
  .appointment__name {
    width: 100%;
    padding: 15px 20px;
  }
  .appointment__email {
    width: 100%;
    padding: 15px 20px;
  }
  .appointment__number {
    width: 81%;
    padding: 15px 20px;
    margin-top: 22px;
  }
  .appointment-select {
    width: 100%;
    margin-top: 22px;
  }
  .appointment__textarea {
    margin-top: 22px;
    width: 100%;
    height: 180px;
  }
  .appointment__btn {
    margin-top: 30px;
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
  .align-appointment-btn {
    display: flex;
    justify-content: flex-end;
  }
</style>

<section class="appointment__shell">
  <div class="container align-form-elements">
    <form 
       on:submit|preventDefault={handleSubmit}
       class="appointment__shell__main-form">
      <p class="appointment__shell__main-form__title">Make an appointment</p>
      <div class="row">
        <input
          bind:value="{name}"
          class="appointment__name"
          type="text"
          name=""
          placeholder="Name" />
        <input
          bind:value="{email}"
          class="appointment__email"
          type="email"
          name=""
          placeholder="Email" />
      </div>

      <div class="row">
        <input
          bind:value="{phoneNumber}"
          class="appointment__number"
          type="number"
          placeholder="Phone Number" />

        <select class="appointment-select" name="cars" id="cars">
          <option value="volvo">Change tire</option>
          <option value="saab">Saab</option>
          <option value="mercedes">Mercedes</option>
          <option value="audi">Audi</option>
        </select>
      </div>

      <div class="row"><textarea class="appointment__textarea" /></div>

      <div class="row align-appointment-btn">
        <button class="appointment__btn">Make an appointment</button>
      </div>
    </form>

    <div class="appointment__shell__description">description</div>
  </div>
</section>
