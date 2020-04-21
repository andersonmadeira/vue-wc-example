<template>
  <button class="button" @click="emitAlert">Show Alert</button>
</template>

<script>
export default {
  name: 'AlertButton',
  props: {
    name: {
      type: String,
      default: 'Someone',
    },
  },
  methods: {
    emitAlert() {
      alert('Hey ' + this.name)
      this.$emit('alert', this.name)
    },
  },
}
</script>

<style scoped>
.button {
  font-size: 1.2em;

  color: #fff;
  font-weight: 700;

  border: none;
  border-radius: 2px;
  height: 40px;
  padding-left: 20px;
  padding-right: 20px;
  display: inline-block;

  box-shadow: 0 6px 16px 0 rgba(67, 184, 201, 0.2);
  background: #27b98c;
  border-color: #27b98c;

  outline: none;
  cursor: pointer;

  transition: all 0.5s ease;
}

.button:hover {
  background: #2cd39f;
}
</style>
