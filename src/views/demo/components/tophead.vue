<!--  -->
<template>
  <div class="t-first">
    <div>运单编号: <span>11230730002</span></div>
    <div>
      <el-button type="warning" plain>取消运单</el-button>
      <el-button type="primary">保存</el-button>
    </div>
  </div>
  <div class="t-second">
    <div class="s-left">
      <div class="s-l-o">
        <div>托运日期:2023-08-21~2023-08-28</div>
        <div>运单结算单位:烽火藤仓</div>
      </div>
      <div class="s-l-t">运输路线：1上海(始发城市)------2上海虹桥(装车站)-------3南京南站(目的地)------4南京(到达城市)</div>
      <div class="s-l-tr">
        <div>结算方式：月付</div>
        <div>服务方式：门到门</div>
        <div>服务方式：铁路集装箱</div>
        <div>支付方式：发货人付款</div>
        <div>回单</div>
      </div>
    </div>
    <div class="s-right">
      <div class="s-r-d">
        <div>运单服务金额</div>
        <div>¥21568.00</div>
      </div>
      <div class="s-r-d">
        <div>运单状态</div>
        <div>派车中</div>
      </div>
      <div class="s-r-d">
        <div>发票状态</div>
        <div>已开票</div>
      </div>
      <div class="s-r-d">
        <div>收款状态</div>
        <div>款未付</div>
      </div>
    </div>
  </div>
</template>

<script setup lang='ts'>

</script>

<style scoped>
.t-first {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.t-second {
  width: 100%;
  display: flex;
  font-size: 13px;
  flex-direction: row;
  justify-content: space-between;

  .s-left {
    display: flex;
    flex-direction: column;

    .s-l-o {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
    }

    .s-l-t {}

    .s-l-tr {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
    }
  }

  .s-right {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;

    .s-r-d {
      margin-right: 8px;
    }
  }
}
</style>