<script setup lang="ts">
import {
  ChatDotRound,
  Document,
  Menu as IconMenu,
  Setting,
  EditPen
} from '@element-plus/icons-vue'
import {useRouter} from 'vue-router'
const router = useRouter()

function change(key: string, keyPath: string[]) {
  console.log(key)
}
</script>

<template>
  <el-menu
      default-active="1"
      class="el-menu-vertical-demo"
      :router=true
  >
    <el-menu-item index="/index/modifyProfile">
      <el-icon>
        <icon-menu/>
      </el-icon>
      <span>修改信息</span>
    </el-menu-item>
    <el-menu-item index="/index/checkUserInfo">
      <el-icon>
        <document/>
      </el-icon>
      <span>所有用户</span>
    </el-menu-item>
    <!--<el-menu-item index="/index/addUser">
      <el-icon>
        <setting/>
      </el-icon>
      <span>添加用户</span>
    </el-menu-item>-->
    <el-menu-item index="/index/chat">
      <el-icon>
        <ChatDotRound/>
      </el-icon>
      <span>随便聊聊</span>
    </el-menu-item>
    <el-menu-item index="/index/writing">
      <el-icon>
        <EditPen/>
      </el-icon>
      <span>写作助手</span>
    </el-menu-item>
  </el-menu>
</template>

<style scoped>
</style>