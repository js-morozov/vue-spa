<template>
  <div class="counter">
    <base-button @click="subNumber">-</base-button>
    <input type="text" class="counter__input" v-model.number="number" />
    <base-button @click="addNumber">+</base-button>
  </div>
</template>

<script>
import BaseButton from "./controls/BaseButton";

export default {
  components: { BaseButton },
  props: {
    defaultValue: {
      type: Number,
      default: 10,
    },
  },
  data() {
    return {
      number: this.defaultValue,
    };
  },
  methods: {
    addNumber() {
      this.number = this.number + 1;
    },
    subNumber() {
      this.number = this.number - 1;
    },
  },
};
</script>

<style lang="scss">
.counter {
  display: flex;
  &__button {
    margin: 0 5px;
  }
}
</style>