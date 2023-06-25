<template>
  <NavBar />

  <div style="display: block;">

    <div style="display: block;">
      <v-row>
        <FirstSection />
      </v-row>
    </div>

    <div style="display: block;">
      <SecondSection />
    </div>

  </div>
</template>

<script>
import NavBar from "@/components/NavBar.vue"
import FirstSection from "@/components/FirstSection.vue"
import SecondSection from "@/components/SecondSection.vue"

export default {
  name: 'HomePage',
  components: {
    NavBar,
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