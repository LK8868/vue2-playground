<template>
  <div>
    <CustomizeTable :data="table"></CustomizeTable>
  </div>
</template>

<script>
import CustomizeTable from '@/components/CustomizeTable/index.vue'
export default {
  name: 'HomeView',
  components: { CustomizeTable },
  data() {
    return {
      table: {
        columns: [
          {
            prop: 'date',
            label: '日期',
          },
          {
            prop: 'name',
            label: '姓名',
          },
          {
            prop: 'address',
            label: '地址',
            columnsType: 'slot',
          },
        ],
        data: [
          {
            date: '2016-05-02111',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1518 弄',
          },
          {
            date: '2016-05-04',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1517 弄',
          },
          {
            date: '2016-05-01',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1519 弄',
          },
          {
            date: '2016-05-03',
            name: '王小虎',
            address: '上海市普陀区金沙江路 1516 弄',
          },
        ],
      },
    }
  },
  created() {},
  methods: {},
}
</script>
<style scoped lang="scss"></style>
