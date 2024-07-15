<template>
  <el-table :data="table.data">
    <el-table-column v-for="item in table.columns" :key="item.prop" v-bind="item"></el-table-column>
  </el-table>
</template>

<script>
export default {
  name: 'CustomizeTable',
  props: {
    data: {
      type: Object,
      required: true,
    },
  },
  data() {
    return {}
  },
  computed: {
    table() {
      return this.data
    },
  },
  methods: {},
}
</script>
<style scoped lang="scss"></style>
