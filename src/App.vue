<template>
  <div>
    <AlertButton class="block" @alert="displayAlert" />
    <AlertButton class="block" name="Anderson" @alert="displayAlert" />
    <Dummy class="block" />
  </div>
</template>

<script>
import AlertButton from './components/AlertButton.vue'
import Dummy from './components/Dummy.vue'

export default {
  name: 'App',
  components: {
    AlertButton,
    Dummy,
  },
  methods: {
    displayAlert(name) {
      console.log('Received greetings to:', name)
    },
  },
}
</script>

<style>
.block {
  display: block;
}
</style>
