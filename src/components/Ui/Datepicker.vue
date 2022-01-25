<template>
  <div class="datepicker">
    <span class="datepicker-back"></span>
    <div class="datepicker-container">
      <h2 class="datepicker-title"> {{ DatepickerTitle }} </h2>
      <p class="datepicker-desc"> {{ DatepickerDesc }} </p>
      <DatepickerYear :datepicker-year="DatepickerDay.getFullYear()"/>
      <DatepickerMonths :datepicker-months="DatepickerMonths"/>
      <DatepickerContents :datepicker-day="DatepickerDay"/>
      <DatepickerTimes/>
    </div>
  </div>
</template>

<script>
import DatepickerYear from "@/components/Ui/Datepiker/DatepickerYear";
import DatepickerMonths from "@/components/Ui/Datepiker/DatepickerMonths";
import DatepickerContents from "@/components/Ui/Datepiker/DatepickerContents";
import DatepickerTimes from "@/components/Ui/Datepiker/DatepickerTimes";

export default {
  name: "Datepicker",
  components: {
    DatepickerYear, DatepickerMonths, DatepickerContents, DatepickerTimes
  },
  props: {
    DatepickerTitle: {
      type: String,
      default: "Персональный график для корректировки расписания"
    },
    DatepickerDesc: {
      type: String,
      default: "Если ваши планы изменились или запись клиента потребует больше времени, то выберите окна и закройте запись для клиентов на это время"
    },
    DatepickerMonths:{
      type: Number,
      default:0
    },
    DatepickerDay:{
      default: new Date()
    }
  }
}
</script>

<style scoped>

</style>