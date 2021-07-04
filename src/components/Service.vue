<template>
  <div :class="cl">
    <div>
      <slot name="header"></slot>
    </div>
    <div>
      <h4>{{ title }}</h4>
      <p>
        {{ text }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["title", "text", "cl"],
};
</script>

<style scoped></style>
