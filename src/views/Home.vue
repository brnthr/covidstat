<template>
  <div class="home">
    <Content />
  </div>
</template>

<script>
// @ is an alias to /src
import Content from '@/components/Content.vue';

export default {
  name: 'home',
  components: {
    Content
  }
}
</script>

<style lang="scss" scoped>
@import './src/scss/index.scss';

.home {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  align-items: flex-start;
  height: 100%;
  color: $primary;

  .page {
    display: flex;
    flex-grow: 1;
    height: calc(100% - 75px);

    .content {
      flex-grow: 1;
      overflow: scroll;

      & > div {
        display: flex;
        justify-content: flex-start;
        padding: 32px;
      }
    }
  }
}
</style>