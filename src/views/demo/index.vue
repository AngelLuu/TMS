<!--  -->
<template>
  <div class='container'>
    <div class="top">
      <Tophead />
    </div>
    <div class="cen">
      <div>
        <el-tabs v-model="state.activeName" class="demo-tabs" @tab-click="changeTab">
          <el-tab-pane label="User" name="first">
            <div>
              <div class="form-box">
                <div class="">
                  <el-form v-model="state.sendForm" class="form-left ">
                    <div class="font-column">
                      发货方
                    </div>
                    <div class="flex flex-col">
                      <div class="flex flex-row">
                        <el-form-item label="托运单位">
                          <el-input v-model="state.sendForm.danwei" />
                        </el-form-item>
                        <el-form-item label="托运人">
                          <el-input v-model="state.sendForm.person" />
                        </el-form-item>
                        <el-form-item label="托运电话">
                          <el-input v-model="state.sendForm.phoneNum" />
                        </el-form-item>
                      </div>
                      <el-form-item label="托运地址">
                        <el-input v-model="state.sendForm.adress" />
                      </el-form-item>
                    </div>
                  </el-form>
                </div>
                <div>
                  <el-form v-model="state.sendForm" class="form-left ">
                    <div class="font-column">
                      发货方
                    </div>
                    <div class="flex flex-col">
                      <div class="flex flex-row">
                        <el-form-item label="托运单位">
                          <el-input v-model="state.sendForm.danwei" />
                        </el-form-item>
                        <el-form-item label="托运人">
                          <el-input v-model="state.sendForm.person" />
                        </el-form-item>
                        <el-form-item label="托运电话">
                          <el-input v-model="state.sendForm.phoneNum" />
                        </el-form-item>
                      </div>
                      <el-form-item label="托运地址">
                        <el-input v-model="state.sendForm.adress" />
                      </el-form-item>
                    </div>
                  </el-form>
                </div>
              </div>
              <div>
                <el-form v-model="state.sendForm" class="flex items-center">
                  <div class="font-column">
                    货物信息
                  </div>
                  <div class="flex flex-col">
                    <div class="flex flex-row">
                      <el-form-item>
                        <div class="text-center">
                          <div>货物名称</div>
                          <el-input v-model="state.sendForm.danwei" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>规格型号</div>
                          <el-input v-model="state.sendForm.person" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>包装</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>重量</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>体积</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>数量</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>计费方式</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>单价</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <div>
                        <el-button type="primary">添加货物</el-button>
                      </div>
                    </div>
                  </div>
                </el-form>
              </div>
              <div>
                <el-form v-model="state.sendForm" class="flex items-center">
                  <div class="font-column">
                    客户应付
                  </div>
                  <div class="flex flex-col">
                    <div class="flex flex-row">
                      <el-form-item>
                        <div class="text-center">
                          <div>保费</div>
                          <el-input v-model="state.sendForm.danwei" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>保额</div>
                          <el-input v-model="state.sendForm.person" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>代收货款</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>手续费</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>装卸费</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>送货费</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>提货费</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>中转费</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>其他费用</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <el-form-item>
                        <div class="text-center">
                          <div>合计费用</div>
                          <el-input v-model="state.sendForm.phoneNum" />
                        </div>
                      </el-form-item>
                      <div>
                        <el-button type="primary">添加费用</el-button>
                      </div>
                    </div>
                  </div>
                </el-form>
              </div>
            </div>
          </el-tab-pane>
          <el-tab-pane label="Config" name="second">Config</el-tab-pane>
          <el-tab-pane label="Role" name="third">Role</el-tab-pane>
          <el-tab-pane label="Task" name="fourth">Task</el-tab-pane>
        </el-tabs>
        <div class="flex flex-row">
          <el-card>
            <template #header>
              <div class="flex justify-between">
                <span>送货单</span>
                <el-button type="primary" @click="state.drawerFlag = true" text>添加费用</el-button>
              </div>
            </template>
            <div class="flex flex-row">
              <el-form label-position="right" label-width="70px" class="mr-20px">
                <el-form-item label="托运单位">
                  <el-input></el-input>
                </el-form-item>
                <el-form-item label="送货单号">
                  <el-input></el-input>
                </el-form-item>
                <el-form-item label="送货车号">
                  <el-input></el-input>
                </el-form-item>
                <el-form-item label="送货箱号">
                  <el-input></el-input>
                </el-form-item>
                <el-form-item label="送货运费">
                  <el-input></el-input>
                </el-form-item>
                <el-form-item label="装卸费">
                  <el-input></el-input>
                </el-form-item>
                <el-form-item label="等候费">
                  <el-input></el-input>
                </el-form-item>
                <el-form-item label="送货合计">
                  <el-input></el-input>
                </el-form-item>
                <el-form-item label="送货核销">
                  <el-input></el-input>
                </el-form-item>
                <el-form-item label="派车时间">
                  <el-date-picker type="datetime" placeholder="Select date and time" />
                </el-form-item>
                <el-form-item label="取货时间">
                  <el-date-picker type="datetime" placeholder="Select date and time" />
                </el-form-item>
              </el-form>
              <div>
                <el-steps direction="vertical" :active="4">
                  <el-step title="处理中" />
                  <el-step title="待供应商接单" />
                  <el-step title="接单派车中" />
                  <el-step title="司机已接单" />
                  <el-step title="送货已装车" />
                  <el-step title="送货已送达" />
                  <el-step title="送货已签收" />
                  <el-step title="回单已确认" />
                </el-steps>
              </div>
            </div>
          </el-card>
        </div>
      </div>
    </div>
    <div class="bom"></div>
    <el-drawer v-model="state.drawerFlag" title="I am the title" direction="rtl" :before-close="handleClose" class="my-drawer">
      <template #header>
        <h4>增加费用项</h4>
      </template>
      <template #default>
        <div>
          测试
        </div>
      </template>
      <template #footer>
        <div style="flex: auto">
          <el-button @click="cancelClick">cancel</el-button>
          <el-button type="primary" @click="confirmClick">confirm</el-button>
        </div>
      </template>
    </el-drawer>
  </div>
</template>

<script setup lang='ts'>
import { nextTick, reactive } from 'vue'
import Tophead from './components/tophead.vue'

const state = reactive({
  activeName: 'first',
  sendForm: {
    danwei: '',
    person: '',
    phoneNum: '',
    adress: ''
  },
  drawerFlag: false
})

const changeTab = (tab: any, e: any) => {
  console.log('tab', tab.props.name)
  console.log('e', e)
  nextTick(() => {
    console.log(state.activeName)
  })
}

const handleClose = (done: () => void) => {
  done()
  //ts-gnore
  // ElMessageBox.confirm('Are you sure you want to close this?')
  //   .then(() => {

  //   })
  //   .catch(() => {
  //     // catch error
  //   })
}

function cancelClick() {
  state.drawerFlag = false
}
function confirmClick() {
  state.drawerFlag = false
}

</script>

<style scoped>
.container {
  width: 100%;
  padding: 4px;
  display: flex;
  flex-direction: column;
  flex: 1;

  .top {
    /* display: flex; */
    width: 100%;
  }

  .form-box {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }

  .form-left {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }
}
.my-drawer{
  height: 100%;
}
</style>