<template>
  <div>
    <nuxt />
  </div>
</template>

<style>
:root {
  --white: #fff;
  --grey: #a9a9a9;
  --dark: #2c2f33;
  --red: #c8102e;
  --dark-red: #720215;
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
}
.center {
  padding: 70px 0;
  text-align: center;
}
.NuxtLogo {
  border-radius: 50%;
  width: 312px;
  height: 312px;
}
.discrim {
  font-family: sofia-pro, sans-serif;
  font-weight: 900;
  font-style: normal;
  font-size: 41px !important;
  color: var(--grey);
  margin: 0;
  padding: 0;
}
.home-buttons {
  margin-top: 10px;
}
.btn {
  color: var(--red);
  font-family: sofia-pro, sans-serif;
  font-size: 16px;
  background: transparent;
  transition: 2s ease-in-out;
  display: inline-block;
  text-decoration: none;
  margin: 10px;
  padding: 10px 30px;
  border-radius: 4px;
  border: 1px solid var(--red);
}
.btn:hover {
  color: var(--white) !important;
  background: var(--red) !important;
}
h1 {
  font-family: sofia-pro, sans-serif;
  font-weight: 900;
  font-style: normal;
  font-size: 81px;
  color: var(--white);
  margin: 0;
}
h2 {
  font-family: sofia-pro, sans-serif;
  font-weight: 600;
  font-style: normal;
  font-size: 40.5px;
  color: var(--red);
  margin: 0;
}
h3 {
  font-family: sofia-pro, sans-serif;
  font-weight: 500;
  font-style: normal;
  font-size: 35px;
  color: var(--white);
  margin: 0;
}
p {
  font-family: sofia-pro, sans-serif;
  font-weight: 300;
  font-style: normal;
  font-size: 20px;
  color: var(--white);
  margin: 0;
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
          hid: 'og:theme-color',
          name: 'og-theme-color',
          content: '#c8102e'
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
