<template>
  <NavBar/>
  <div class="bg-primary">
    <div class="max-w-7xl mx-auto px-2 sm:px-6 lg:px-8">
  <Body/>
    </div>
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import Body from '@/components/Body.vue'
export default {
  name: 'App',
  components: {
    NavBar,
    Body
  }
}
</script>
