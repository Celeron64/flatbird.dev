<template>
  <div class="c">
    <Logo />
    <h1 class="title">404. not found.</h1>
    <h3 class="subtitle">serious yikes</h3>
    <a href="mailto:bird@circlebot.xyz" class="button--email">
      report an issue
    </a>
  </div>
</template>

<script>
import Logo from '~/components/404.vue';

export default {
  components: {
    Logo
  },
  props: {
    error: {
      type: Object,
      default: null
    }
  }
};
</script>

<style>
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
body {
  height: 100%;
  cursor: default;
}
*:hover {
  cursor: default;
}
.c {
  margin-top: 50px;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: #2c2f33;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 320;
  font-size: 60px;
  color: #fff;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: rgb(145, 145, 145);
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
