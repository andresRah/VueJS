<template lang="pug">
  li.artist
    h2: a(v-bind:href="artistaa.url" target="_blank") {{ artistaa.name }}
    img(:src="artistaa.image[2]['#text']")
</template>

<script>
export default {
  name: "artist",
  props: ["artistaa"]
};
</script>

<style lang="stylus" scoped>
li.artist {
  display: block;
  margin: 10px 0;
}
</style>