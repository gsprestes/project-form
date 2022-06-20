<template>
  <div class="form">
    <label class="label"> {{ label }}</label>
    <input :type="type" :class="classe" :placeholder="placeholder"/>
    <p class="error">{{ error }}</p>
  </div>

</template>

<script>
    export default {
    name: "InputForm",
    props: {
      type: {
        type: String
      },
      label: {
        type: String
      },
      classe : {
        type: String
      },
      error: {
        type: String
      },
      placeholder: {
        type: String
      }
    }
    }
</script>

<style src="./InputForm.scss" lang= "scss" scoped/>