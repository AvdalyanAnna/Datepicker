<template>
  <div class="datepicker-block datepicker-years">
    <div class="datepicker-block-left datepicker-block-arrow"></div>
    <div class="datepicker-block-content">{{ DatepickerYear }}</div>
    <div class="datepicker-block-right datepicker-block-arrow"></div>
  </div>
</template>

<script>
export default {
  name: "DatepickerYear",
  props: {
    DatepickerYear: {
      type: Number,
      default: 2022
    }
  }
}
</script>

<style scoped>

</style>