<template>
  <div class="app-container">
    <div class="app-title">
      <div>
        <span>会议标题：</span><el-input class="input-style"></el-input>
        <el-button type="primary" class="span-style">查询</el-button>
        <el-button type="warning">清空</el-button>
      </div>
    </div>
    <div class="table-style">
      <div class="button-style">
        <el-button type="warning" plain>取消预订</el-button>
      </div>
      <el-table
        :data="tableData"
        :header-cell-style="{'text-align':'center', 'background-color' : '#EFEFEF'}">
        <el-table-column
          prop="title"
          label="会议标题"
          align="center">
        </el-table-column>
        <el-table-column
          label="会议室"
          align="center">
        </el-table-column>
        <el-table-column
          label="会议日期"
          align="center">
        </el-table-column>
        <el-table-column
          prop="time"
          label="会议开始时间"
          align="center">
        </el-table-column>
        <el-table-column
          prop="time"
          label="会议结束时间"
          align="center">
        </el-table-column>
      </el-table>
    </div>
  </div>
</template>

<script>
  export default {
    name: "MyReserve",
    data() {
      return {
        tableData: [
          {
            title: '周三例行会议',
            num: 'D463626571',
            sendPeople: '张红',
            applePeople: '郑强',
            time: '2020-06-15',
            type_exp: '会议'
          },
          {
            title: '大赛通知',
            num: 'D9979735346',
            sendPeople: '张贺',
            applePeople: '邓世强',
            time: '2020-06-03',
            type_exp: '通知'
          },
          {
            title: '周四例行会议',
            num: 'D685634657',
            sendPeople: '张敏',
            applePeople: '郑强',
            time: '2020-05-28',
            type_exp: '会议'
          },
          {
            title: '人员调配通知',
            num: 'D79476583',
            sendPeople: '董成文',
            applePeople: '刘诗诗',
            time: '2020-05-16',
            type_exp: '通知'
          },
          {
            title: '周三例行会议',
            num: 'D89579345',
            sendPeople: '张红',
            applePeople: '郑强',
            time: '2020-05-05',
            type_exp: '会议'
          },
        ],
        value1: ''
      }
    }
  }
</script>

<style scoped>
  .app-title {
    padding: 30px;
    background-color: #fff;
  }
  .input-style {
    width: 200px;
  }
  .span-style {
    margin-left: 150px;
  }
  .table-style {
    background-color: #fff;
    margin-top: 30px;
    padding: 30px;
  }
  .button-style {
    float: right;
    margin-bottom: 20px;
  }
</style>
