<template>
  <header>
    <nav>
      <ul>
        <li>
          <NuxtLink to="/"> Home </NuxtLink>
        </li>
        <li>
          <NuxtLink to="/settings"> Setting </NuxtLink>
        </li>
        <li>
          <NuxtLink to="/profile"> Profile </NuxtLink>
        </li>
        <li>
          <NuxtLink to="/deck">Deck</NuxtLink>
        </li>
      </ul>
    </nav>
  </header>
</template>
<style lang="scss">
header {
  background-color: #000;
  color: #fff;
  height: 100px;
  display: flex;
  nav {
    height: inherit;
  }
  ul {
    align-items: center;
    display: flex;
    justify-content: center;
    list-style: none;
    margin: 0;
    padding: 0;
    li {
      margin: 0 1.5rem;
      a {
        color: #000ccc;
        text-decoration: none;
      }
    }
  }
}
</style>
