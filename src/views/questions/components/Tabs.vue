<template>
  <el-tabs type="card">
    <el-tab-pane v-for="(item, index) in tabList" :key="index" label="">
      <span slot="label"><i :class="item.icon" />{{ item.name }}</span>
      <div class="">{{ item.name }}</div>
      <span v-pre>
                _.-"\
          _.-"     \
        ,-"          \
        \    基 社    \
        \ \    本 区    \
        \ \    法      \
          \ \         _.-;
          \ \    _.-"   :
            \ \,-"    _.-"
            \(   _.-"
              `--"
      </span>
    </el-tab-pane>
  </el-tabs>
</template>

<script>
export default {
  name: 'Tabs',
  props: {
    tabList: {
      type: Array,
      default: () => {
        return []
      }
    }
  }
}
</script>

<style scoped>
</style>
