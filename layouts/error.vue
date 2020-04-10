<template>
  <div class="container">
    <div>
      <h1 v-if="error.statusCode === 404" class="title">404</h1>
      <h1 v-else>Something went wrong</h1>
      <h2 class="subtitle">Page not found</h2>
      <div class="links">
        <a href="mailto:bird@circlebot.xyz" class="button--yellow">
          Report a problem
        </a>
        <a href="/" class="button--grey">
          Go home
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    error: {
      type: Object,
      default: null
    }
  }
};
</script>

<style>
html {
  margin: 10px;
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  background: #2c2f33;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--yellow {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #fff1a3;
  color: #fff1a3;
  text-decoration: none;
  margin: 10px;
  padding: 10px 30px;
}

.button--yellow:hover {
  color: #2c2f33;
  transition: 2s;
  background-color: #fff1a3;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #99aab5;
  color: #99aab5;
  text-decoration: none;
  padding: 10px 30px;
  margin: 10px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  transition: 2s;
  background-color: #99aab5;
}

.button--66ccff {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #66ccff;
  color: #66ccff;
  text-decoration: none;
  padding: 10px 30px;
  margin: 10px;
  margin-left: 15px;
}

.button--66ccff:hover {
  color: #fff;
  transition: 2s;
  background-color: #66ccff;
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
  font-weight: 320;
  font-size: 100px;
  color: #8e9dbd;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
