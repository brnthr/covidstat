<template>
  <div class="card" :class="{full: (width === 'full'), half:(width === 'half')}">
    <span class="title">{{ title }}</span>
    <span class="content">{{ content }}</span>
  </div>
</template>

<script>

export default {
  name: 'card',
  props: {
    width: String,
    title: String,
    content: String,
  }
}
</script>

<style lang="scss" scoped>
@import './src/scss/index.scss';

.card {
  padding: 20px;
  display: flex;
  flex-direction: column;
  background: $background-secondary;
  border: solid rgb(93, 161, 118) 1px;
  border-radius: 10px;
  align-items: center;
  height: fit-content;
  flex-shrink: 1;
  flex-basis: auto;
  margin-bottom: 20px;

  .title {
    font-weight: bold;
    margin: 0 0 20px 0;
  }

}
</style>
