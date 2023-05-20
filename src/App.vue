<script>
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'
import AppFooter from './components/AppFooter.vue'
import AppBlueBar from './components/AppBlueBar.vue'


export default {
  components: {
    AppHeader,
    AppContent,
    AppFooter,
    AppBlueBar
  }
}

</script>

<template>
  <header class="w-100">
    <AppHeader />
  </header>
  <main>
    <AppContent />
    <AppBlueBar />
  </main>
  <AppFooter />
</template>


