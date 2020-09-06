<template>
  <div class="center grid">
    <vs-row justify="center" align="center">
      <vs-col
        vs-type="flex"
        vs-justify="center"
        vs-align="center"
        lg="12"
        sm="10"
        xs="10"
      >
        <h1 class="title">How to use the bot</h1>
      </vs-col>
    </vs-row>
    <vs-row justify="center" align="center">
      <vs-col
        vs-type="flex"
        vs-justify="center"
        vs-align="center"
        lg="12"
        sm="10"
        xs="10"
      >
        <h2 class="subtitle">
          This page explains how to connect your discord account to the bot for
          choosing your roles. <br /><br />
          To start using the bot you need to click the button below.
        </h2>
      </vs-col>
    </vs-row>
    <vs-row justify="center" align="center">
      <vs-col
        vs-type="flex"
        vs-justify="center"
        vs-align="center"
        lg="12"
        sm="10"
        xs="10"
      >
        <vs-button color="discord" size="xl">
          <i class="bx bxl-discord"></i> Login</vs-button
        >
      </vs-col>
    </vs-row>
  </div>
</template>

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
</style>
