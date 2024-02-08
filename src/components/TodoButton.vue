<script setup>

</script>

<template>
    <button>
        <slot></slot>
    </button>
</template>

<style lang="scss" scoped>
  button {
    padding: 8px 16px;
    border: none;
    cursor: pointer;
  }

  button:hover {
    background-color: #41b080;
    color: white;
  }
</style>