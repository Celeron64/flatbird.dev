<template>
  <div>
    <nuxt />
  </div>
</template>

<style>
html {
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
  padding: 10px 30px;
}

.button--yellow:hover {
  color: #2c2f33;
  background-color: #fff1a3;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #99aab5;
  color: #99aab5;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #99aab5;
}

.button--66ccff {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #66ccff;
  color: #66ccff;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--66ccff:hover {
  color: #fff;
  background-color: #66ccff;
}
</style>

<script>
export default {
  head() {
    return {
      title: this.title,
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: 'theme-color',
          name: 'theme-color',
          content: '#fff1a3'
        },
        {
          hid: 'og:title',
          name: 'og:title',
          content: 'Flatbird'
        }
      ]
    }
  }
}
</script>
