<template>
  <div>
    <h1>Hello welcome components</h1>
    <!-- V-slots -->
    <slot name="demo"></slot>
    <slot name="firstName" :middleName="leon" :lastName="woo"> </slot>
  </div>
</template>

<script>
export default {
  setup() {
    const leon = "leon";
    const woo = "woo";
    return {
      leon,
      woo,
    };
  },
};
</script>
