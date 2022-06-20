<template>
  <div class="card">
    <div class="header">
      <img src="../../assets/logo.png" alt="">
      <h1>Intern Sign Up</h1>
    </div>
    <form class="form">
      <div class="mid-form">
        <InputForm type="text" label="Full Name *" classe="primario" error="Fullname Invalid" placeholder="Name"/>
        
        <div class="email-pass">
          <InputForm type="email" label="Email *" classe="primario" error="Email Invalid" placeholder="foo@bar.com"/>
        </div>

        <div class="tel-birthday">
          <InputForm type="tel" label="Phone *" classe="primario" error="Phone Invalid" placeholder="(83) 00000-0000"/>
        </div>

        <div class="email-pass">
          <InputForm type="password" label="Password *" classe="primario" error="Password Invalid" placeholder="Enter your password"/>
        </div>

        <div class="tel-birthday">
          <InputForm type="date" label="Birthday *" classe="primario" error="Age Invalid"/>
        </div>

        
        <div class="container-register">
          <InputCheck type="checkbox" label="I accept the terms and privacy" classe="check" error="You must accept the terms"/>
          <button id="button">Register</button>
        </div>
      </div>
    </form>
  </div>
</template>

<script>
    import InputForm from "../Inputs/InputForm.vue"
    import InputCheck from "../InputCheck/InputCheck.vue"

    export default {
    name: "CardForm",
    components: {
      InputForm,
      InputCheck
    }
    }

</script>

<style src="./CardForm.scss" lang= "scss" scoped/>

