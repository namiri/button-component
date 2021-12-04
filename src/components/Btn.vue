<template>
  <div class="hello" style="display: flex">
    <!-- :variant="variant" -->
    <!--     :class="['my-button', {'warning': isWarning}]" -->
    <button
      :style="{ backgroundColor: bgColor, outline: outline }"
      :tagUser="signedUp ? 'Logout' : 'Login'"
      :class="[
        {
          'card-input__input': true,
          border: statusValidtion,
          'border-danger': statusValidtion,
        },
      ]"
    >
      test
      <i class=""></i>
    </button>
  </div>
</template>

<script>
export default {
  name: "Btn",
  props: {
    bgColor: String,
    icon: String,
    outline: {
      type: String,
      default: "off",
    },
    variant: {
      type: String,
      default: "primary",
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
button {
  margin: 5px;
  padding: 8px 19px;
  display: inline-block;
  border: 1px solid #ddd;
  border-radius: 5px;
  font-size: 14px;
}
</style>
