<template>
  <div class="c">
    <div>
      <logo />
      <h1 class="title">
        Aaron
      </h1>
      <h2 class="subtitle">
        <img src="https://cdn.discordapp.com/emojis/543967292409511956.gif?v=1" />
      </h2>
      <div class="links">
        <a href="mailto:contact@circlebot.xyz" class="button--yellow">
          Email me
        </a>
        <a
          href="https://circlebot.xyz"
          target="_blank"
          title="free advertising"
          class="button--66ccff"
        >
          Circle
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/aaron.vue';

export default {
  components: {
    Logo
  },
  head() {
    return {
      title: this.title,
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: 'theme-color',
          name: 'theme-color',
          content: '#66ccff'
        },
        {
          hid: 'og:title',
          name: 'og:title',
          content: 'aaron'
        },
        {
          hid: 'og:description',
          name: 'og:description',
          content: 'yes.'
        },
        {
          hid: 'og:image',
          name: 'og:image',
          content: '/aaron.png'
        }
      ]
    };
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
  animation: 5s appear;
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

@keyframes appear {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
