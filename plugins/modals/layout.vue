<template>
  <div>
    <div>
      <div v-if="visible" :data-modal="name">
        <div
          aria-modal="true"
          data-reach-dialog-content="true"
          tabindex="-1"
          class="modal_mask"
        >
          <div class="modal_body">
            <slot :payload="payload" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import VModal from './handle'

export default {
  props: {
    name: {
      type: String,
      require: true,
    },
  },
  data() {
    return {
      payload: null,
      visible: false,
    }
  },
  beforeMount() {
    VModal.EventBus.$on('open', (params) => {
      if (this.name === params.name) {
        this.open(params)
      }
    })
    VModal.EventBus.$on('close', (params) => {
      if (this.name === params.name) {
        this.close(params)
      }
    })
  },
  methods: {
    open(params) {
      this.visible = true
    },
    close(params) {
      this.visible = false
    },
  },
}
</script>
<style lang="scss" scoped>
.modal_mask {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  max-width: unset;
  height: 100vh;
  overflow-y: auto;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: rgba(18, 18, 18, 0.6);
  z-index: 9999;
}
</style>
