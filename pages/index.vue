<template>
  <div id="root ">
    <div class="ct">
      <div class="banner">
        <div class="thumbnail-banner"></div>
      </div>
      <div class="popular-decks">
        <h3 class="text_center my_3">3 popular deck for You</h3>
        <div class="r">
          <div class="c_4">
            <div class="card">Deck 1</div>
          </div>
          <div class="c_4">
            <div class="card">Deck 1</div>
          </div>
          <div class="c_4">
            <div class="card">Deck 1</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
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
.banner {
  height: 350px;
  margin-top: 2rem;
  .thumbnail-banner {
    background: url('~assets/imgs/top-banner.jpg') center center;
    background-size: cover;
    height: inherit;
  }
}
</style>
