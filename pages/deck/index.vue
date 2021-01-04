<template>
  <div id="root">
    <header>
      <h1>pls enter number of deck to show</h1>
      <input
        v-model="deckId"
        type="text"
        placeholder="please enter number of deck to show"
      />
      <button @click="showDeck">go to deck</button>
    </header>
  </div>
</template>

<script>
export default {
  data() {
    return {
      deckId: '1',
    }
  },
  methods: {
    showDeck() {
      // this.$router.push('/deck/' + this.deckId)
      this.$router.push(`/deck/${this.deckId}`)
    },
  },
}
</script>
