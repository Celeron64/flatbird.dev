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

.button--email {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #ff4444;
  color: #ff4444;
  text-decoration: none;
  margin: 10px;
  padding: 10px 30px;
  transition: all 2s ease-out;
}

.button--email:hover {
  color: #fff;
  background-color: #ff4444;
}

.button--blurple {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #7289da;
  color: #7289da;
  text-decoration: none;
  padding: 10px 30px;
  margin: 10px;
  margin-left: 15px;
  transition: all 2s ease-out;
}

.button--blurple:hover {
  color: #fff;
  background-color: #7289da;
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
  transition: all 2s ease-out;
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
          hid: 'og:title',
          name: 'og:title',
          content: 'Flatbird'
        },
        {
          hid: 'og:description',
          name: 'og:description',
          content: 'A website for the coolest bird ever.'
        },
        {
          hid: 'og:image',
          name: 'og:image',
          content: '/bird.png'
        }
      ]
    };
  }
};
</script>
