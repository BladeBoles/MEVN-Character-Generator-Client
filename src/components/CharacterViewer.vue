<template>
  <div class="character-view">
    <h1>Character Viewer</h1>
    <p v-for="(character, index) in characters" v-bind:key="index">
      {{ character.name }} is a {{ character.profession }}.
    </p>
  </div>
</template>

<script>
  export default {
    name: 'CharacterViewer',
    props: {
      characters: Array
    }
  }


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
