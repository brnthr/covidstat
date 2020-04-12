<template>
    <div class="left-menu">
      <router-link tag="button" :to="{ name: 'avion' }">
        Avion
      </router-link>

      <router-link tag="button" :to="{ name: 'retard' }">
        Retard
      </router-link>

      <router-link tag="button" :to="{ name: 'mouvement' }">
        Mouvement
      </router-link>

      <router-link tag="button" :to="{ name: 'aéroport' }">
        Aéroport
      </router-link>
    </div>
</template>

<style lang="scss" scoped>
@import './src/scss/index.scss';

.left-menu {
  display: flex;
  justify-content: flex-start;
  flex-direction: column;
  height: 100%;
  background: transparent;
  min-width: 150px;
  justify-content: center;
  background-color: $secondary;


  button {
    background: transparent;
    color: $primary;


    &:hover {
      background: rgb(100, 173, 127);
    }
  }
}
</style>
