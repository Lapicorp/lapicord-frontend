<template>
  <div id="app">
    <link
      href="https://cdn.jsdelivr.net/npm/boxicons@2.0.5/css/boxicons.min.css"
      rel="stylesheet"
    />
    <div class="center examplex">
      <vs-navbar
        v-model="active"
        :color="navbarColor"
        text-white
        shadow
        target-scroll="#padding-scroll-content"
        padding-scroll
        center-collapsed
      >
        <template #left>
          <img src="/logo-256.png" alt="logo" width="48" height="48" />
        </template>
        <vs-navbar-item id="home" :active="active == 'home'" to="home">
          Home
        </vs-navbar-item>
        <vs-navbar-item
          id="getStarted"
          :active="active == 'getStarted'"
          to="start"
        >
          Get Started
        </vs-navbar-item>
        <vs-navbar-item id="about" :active="active == 'about'" to="about">
          About this service
        </vs-navbar-item>
        <template #right>
          <vs-button color="discord">
            <i class="bx bxl-discord"></i> Login</vs-button
          >
        </template>
      </vs-navbar>
      <div id="padding-scroll-content" class="square"></div>
    </div>
    <Nuxt />
  </div>
</template>

<script>
export default {
  data: () => ({
    active: 'home',
    navbarColor: 'dark',
  }),
}
</script>

<style>
#app {
  display: flex;
  align-items: center;
  width: 100%;
  justify-content: center;
  height: 100vh;
}

html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
