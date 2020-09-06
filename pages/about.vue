<template>
  <div class="container">
    <div>
      <header class="content-logos">
        <logo />
      </header>
      <h1 class="title">Lapicord bot</h1>
      <h2 class="subtitle">
        Lapicord bot is a utils bot for choosing roles more easily than reaction
        roles on Discord.
      </h2>
      <div class="links">
        <h3 class="h3">Find the code here</h3>
        <a
          href="https://github.com/Lapicorp/lapicord-frontend"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          Frontend
        </a>
        <a
          href="https://github.com/Lapicorp/lapicord-backend"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          Backend
        </a>
        <a
          href="https://github.com/Lapicorp/lapicord-discord"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          Discord bot
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo,
  },
}
</script>

<style>
.home-enter-active,
.home-leave-active {
  transition: opacity 0.5s;
}
.home-enter,
.home-leave-active {
  opacity: 0;
}
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 55px;
  color: #35495e;
  letter-spacing: 1px;
  text-transform: capitalize;
  margin: 25px 0;
}

.subtitle {
  font-weight: 300;
  font-size: 1.1rem;
  color: #526488;
  word-spacing: 2px;
  padding-bottom: 15px;
  max-width: 600px;
}

.subtitle a {
  font-weight: 500;
  color: inherit;
}

.links {
  padding-top: 15px;
  margin-bottom: 20px;
}

.content-logos {
  display: flex;
  align-items: center;
  justify-content: center;
  min-width: 500px;
}

.plus {
  font-size: 2.5rem;
  margin: 15px;
  color: #35495e;
}

.h3 {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-weight: 400;
  margin: 10px;
}
</style>
