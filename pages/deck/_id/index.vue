<template>
  <section>
    <div class="r">
      <div class="ct text_center">
        <h3>Deck: Learn Englist By ...</h3>
        <div class="tools">
          <button class="btn btn_success">Start</button>
          <button class="btn btn_primary">create a card</button>
        </div>
        <hr class="devide" />
        <div class="r">
          <div class="c_3">
            <div class="card">
              <div class="front-cardt">
                <img
                  src="https://finance.vietstock.vn/image/QCG"
                  alt="thumbnail card"
                />
              </div>
              <div class="back-cardt">
                <h6>Shop</h6>
              </div>
            </div>
          </div>
          <div class="c_3">
            <div class="card">
              <div class="front-cardt">
                <img
                  src="https://finance.vietstock.vn/image/QCG"
                  alt="thumbnail card"
                />
              </div>
              <div class="back-cardt">
                <h6>Shop</h6>
              </div>
            </div>
          </div>
          <div class="c_3">
            <div class="card">
              <div class="front-cardt">
                <img
                  src="https://finance.vietstock.vn/image/QCG"
                  alt="thumbnail card"
                />
              </div>
              <div class="back-cardt">
                <h6>Shop</h6>
              </div>
            </div>
          </div>
          <div class="c_3">
            <div class="card">
              <div class="front-cardt">
                <img
                  src="https://finance.vietstock.vn/image/QCG"
                  alt="thumbnail card"
                />
              </div>
              <div class="back-cardt">
                <h6>Shop</h6>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style lang="scss">
section {
  padding: 3rem 0 0 0;
  .devide {
    margin: 2rem 0;
  }
}
</style>
<script>
export default {
  validate({ params }) {
    return /^[0-9]$/.test(params.id)
  },
}
</script>
