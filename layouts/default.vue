<template>
  <div>
    <nuxt />
  </div>
</template>

<style>
:root {
  --white: #fff;
  --dark: #2c2f33;
  --red: #c8102e;
}
html {
  margin: 10px;
  background: var(--dark);
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  margin: 30px;
}
.center {
  padding: 70px 0;
  text-align: center;
}
.NuxtLogo {
  border-radius: 50%;
}
h1 {
  font-family: sofia-pro, sans-serif;
  font-weight: 900;
  font-style: normal;
  font-size: 81px;
  color: var(--white);
}
</style>

<script>
export default {
  head() {
    return {
      title: this.title,
      link: [
        {
          rel: 'stylesheet',
          href: 'https://use.typekit.net/yao2abo.css'
        }
      ],
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
