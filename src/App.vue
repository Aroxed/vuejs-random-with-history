<template>
  <div id="app">
    <Random @randomValueIsGenerated="OnRandomValueIsGenerated"> </Random>
    <History :valueList="valueList"></History>
  </div>
</template>

<script>
import Random from "@/components/random.vue"
import History from "@/components/history.vue"
export default {
  name: "App",
  components: { Random, History },
  data() {
    return {
      valueList: []
    }
  },
  methods: {
    OnRandomValueIsGenerated(value) {
      this.valueList.push(value)
    }
  }
}
</script>

<style></style>
