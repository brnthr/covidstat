<template>
  <div class="content">
    <Card :title="'Card'" :content="''" :width="'full'"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Card from '@/components/Card.vue';

export default {
  name: 'content',
  components: {
    Card,
  }
}
</script>

<style lang="scss" scoped>
@import './src/scss/index.scss';

.content {
  padding: 20px;
  max-height: calc( 100% - 2 * 20px);
  height: fit-content;
  overflow-y: scroll;
  border-radius: 10px;
  overflow-x: scroll;
  flex-grow: 1;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;

}
</style>