<template>
  <div>
    <slot :questions="questions"></slot>
  </div>
</template>

<script>
export default {
  data() {
    return {
      questions: ["Item 1", "Item 2", "Item 3"],
    };
  },
};
</script>