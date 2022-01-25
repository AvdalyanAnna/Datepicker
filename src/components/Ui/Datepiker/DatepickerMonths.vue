<template>
  <div class="datepicker-block datepicker-months">
    <div class="datepicker-block-left datepicker-block-arrow"></div>
    <div class="datepicker-block-content">
      {{ DatepickerMonthsList[DatepickerMonths] }}
    </div>
    <div class="datepicker-block-right datepicker-block-arrow"></div>
  </div>
</template>

<script>
export default {
  name: "DatepickerMonths",
  data() {
    return {
      DatepickerMonthsList: ['Январь','Январь 1']
    }
  },
  props: {
    DatepickerMonths: {
      type: Number,
      default: 0
    }
  }
}
</script>

<style scoped>

</style>