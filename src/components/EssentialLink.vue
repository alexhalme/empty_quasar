<template>
  <q-item clickable tag="a" target="_blank">
    <q-item-section avatar>
      <q-icon name="send" />
    </q-item-section>

    <q-item-section>
      <q-item-label caption>
        {{ caption }}a
      </q-item-label>
    </q-item-section>
  </q-item>
</template>

<script>
import { defineComponent } from 'vue'

emptyRequest = function () {
  return {
    b: 'c'
  }
}

export default defineComponent({
  name: 'EssentialLink',
  props: {
    caption: {
      type: String,
      required: false,
      default() { return '' }
    }
  },
  data() {
    return {}
  }
})
</script>
