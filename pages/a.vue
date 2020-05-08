<template>
  <v-layout column justify-center>
    <h1>One sec, let me redirect you..</h1>
    <h2>oof!</h2>
  </v-layout>
</template>

<script>
export default {
  middleware({ store, redirect }) {
    return redirect('https://discord.bio/p/bird');
  }
};
</script>
