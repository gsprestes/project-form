<template>
    <div class="container">
        <div class="terms-and-check">
            <input type="checkbox" :class="classe" :placeholder="placeholder"/>
            <label class="label"> {{ label }}</label>
        </div>
        <p class="error">{{ error }}</p>
    </div>
</template>

<script>
    export default {
    name: "InputCheck",
    props: {
      label: {
        type: String
      },
      error: {
        type: String
      },
      classe: {
        type: String
      }
    }
}
</script>

<style src="./InputCheck.scss" lang= "scss" scoped/>