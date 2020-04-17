<template>
  <div class="c">
    <Logo />
    <h1 class="title">Flatbird<span class="subtitle">#0001</span></h1>
    <h3 class="subtitle">pro script kiddie</h3>
    <a href="mailto:bird@circlebot.xyz" class="button--email">
      Email
    </a>
    <a href="https://discord.gg/v2uS9nw" class="button--blurple">
      Discord
    </a>
    <a href="https://circlebot.xyz" class="button--66ccff">
      Main Project
    </a>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue';

export default {
  components: {
    Logo
  }
};
</script>

<style>
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
