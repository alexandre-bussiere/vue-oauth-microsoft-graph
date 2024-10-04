<template>
  <button 
    class="base-button" 
    :disabled="disabled" 
    @click="$emit('click')"
  >
    <slot></slot> <!-- This allows dynamic content inside the button -->
  </button>
</template>

<script>
export default {
  name: 'BaseButton',
  props: {
    disabled: {
      type: Boolean,
      default: false,
    }
  }
};
</script>

<style scoped>
.base-button {
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  background-color: #3498db;
  color: white;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s ease, transform 0.2s ease;
}

.base-button:hover,
.base-button:focus {
  background-color: #2980b9;
  transform: scale(1.05);
}

.base-button:disabled {
  background-color: #bdc3c7;
  cursor: not-allowed;
}

.base-button:disabled:hover,
.base-button:disabled:focus {
  transform: none;
}
</style>
