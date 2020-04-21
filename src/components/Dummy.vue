<template>
  <div class="dummy-container">
    <span>Dummy</span>
  </div>
</template>

<script>
export default {
  name: 'Dummy',
}
</script>

<style scoped>
.dummy-container {
  padding: 15px;
  background: #27b98c;
  text-align: center;
  transition: background 0.5s ease-in-out;
}
.dummy-container:hover {
  background: #2cd39f;
}
.dummy-container span {
  color: white;
  font-size: 1.2em;
  font-weight: 700;
}
</style>
