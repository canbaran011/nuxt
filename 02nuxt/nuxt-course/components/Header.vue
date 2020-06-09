<template>
  <div>
    <header class="header">
      <ul class="nav-items">
        <li>
          <nuxt-link to="/">HOME</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/users">USERS</nuxt-link>
        </li>
      </ul>
    </header>
  </div>
</template>

<style scoped>
.header {
  width: 100%;
  height: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: aquamarine;
}
.nav-items {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  width: 80%;
}
.nav-items a{
    text-decoration: none;
    color: palevioletred;

}
</style>
