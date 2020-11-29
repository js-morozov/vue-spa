<template>
  <div>
    <button class="button" @click="$emit('click', $event)">
      <slot></slot>
    </button>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.button {
  cursor: pointer;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 30px;
  height: 30px;
  border: none;
  outline: none;
  background: #1abc9c;
  color: #ffffff;
  border-radius: 10px;
  margin: 5px;
}
</style>