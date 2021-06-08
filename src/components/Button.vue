<template>
  <div>
      <button>load more</button>
  </div>
</template>

<script>
export default {
    name: 'Button'
}
</script>

<style lang="scss" scoped>
@import '../style/variables';
@import '../style/mixins';
    div {
        margin-top: 20px;
    }
    button {
        @include mainBtn;
        &:hover {
            background-color: transparent;
        }
    }
</style>