<template>
  <div class="page">
    <div class="nav">
      <li>
        <nuxt-link to="/settings">General</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/settings/deck">Deck</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/settings/schedule">Schedule</nuxt-link>
      </li>
    </div>
    <!-- <div class="main">
      <h3>General setting</h3>
    </div> -->
    <nuxt-child />
  </div>
</template>

<style lang="scss">
.page {
  display: flex;
  .main {
    margin-left: 3rem;
  }
}
</style>
