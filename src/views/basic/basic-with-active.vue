<template>
  <div class="view-box">
    <div id="toolbar">
      <input type="checkbox" v-model="active1" /> Toggle Active1
      <input type="checkbox" v-model="active2" /> Toggle Active2
    </div>
    <div class="container">
      <vue-drag-resize-rotate :active.sync="active1">
        <p>
          外部组件通过控制
          <b>:active</b> prop来控制组件的激活状态
        </p>
      </vue-drag-resize-rotate>
      <vue-drag-resize-rotate :active.sync="active2">
        <p>
          外部组件通过控制
          <b>:active</b> prop来控制组件的激活状态
        </p>
      </vue-drag-resize-rotate>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      active1: false,
      active2: false
    }
  },
  methods: {
  }
}
</script>

<style>
</style>