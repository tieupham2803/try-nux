<template>
  <div id="root">
    <div class="ct">
      <div class="d_flex justify_content_between my_3">
        <h2>List of your deck</h2>
        <button class="btn btn_success" @click.prevent="openModal">
          create a deck
        </button>
      </div>
      <ul class="decks-list">
        <li>
          <nuxt-link class="deck" to="/deck/1212122">
            <div class="deck-card card">
              <img
                src="https://dreamztoreality.net/wp-content/uploads/2019/08/Learn-English-590x369.jpg"
                alt="thumbnal card"
              />
              <div class="card_body">
                <h3>Title</h3>
                <p>Description</p>
              </div>
            </div>
          </nuxt-link>
        </li>
        <li>
          <nuxt-link class="deck" to="/deck/1212122">
            <div class="deck-card card">
              <img
                src="https://dreamztoreality.net/wp-content/uploads/2019/08/Learn-English-590x369.jpg"
                alt="thumbnal card"
              />
              <div class="card_body">
                <h3>Title</h3>
                <p>Description</p>
              </div>
            </div>
          </nuxt-link>
        </li>
      </ul>
    </div>
    <v-modal name="test">
      <h1>hello test modal</h1>
      <button class="btn btn_danger" @click.prevent="closeModal">X</button>
    </v-modal>
  </div>
</template>
<style lang="scss">
.decks-list {
  margin: 0;
  padding: 0;
  .deck {
    display: block;
  }
  li {
    margin-bottom: 1rem;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .deck-card {
    display: flex;
    flex-direction: row;
    height: 250px;
    img {
      height: auto;
      width: 250px;
    }
  }
}
</style>
<script>
export default {
  data() {
    return {
      deckId: '1',
    }
  },
  methods: {
    openModal() {
      this.$modal.open({
        name: 'test',
      })
    },
    closeModal() {
      this.$modal.close({
        name: 'test',
      })
    },
    showDeck() {
      // this.$router.push('/deck/' + this.deckId)
      this.$router.push(`/deck/${this.deckId}`)
    },
  },
}
</script>
