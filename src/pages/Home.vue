<template>
  <FirstSection />

  <div id="second-section">
    <h1 style="color: white">Teste</h1>
  </div>

  <!-- <div style="display: block;">
    <SecondSection />
  </div> -->
</template>

<script>
import FirstSection from "@/components/FirstSection.vue"
import SecondSection from "@/components/SecondSection.vue"

export default {
  name: 'HomePage',
  components: {
    FirstSection,
    SecondSection
  }
}
</script>

<style>
.font-charcoal {
  font-family: 'Excluded', sans-serif;
}
</style>