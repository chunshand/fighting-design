<script lang="ts" setup></script>

  const visible1 = ref(false)
  const finish = ()=>{
    console.log('111')
  }
</script>

<template>
  <f-count-down :time="60*1000" :on-finish="finish" format="HH:mm:ss:SSS" >

  </f-count-down>
  <f-button type="primary" @click="visible1 = true">打开</f-button>

  <f-dialog v-model:visible="visible1" title="标题文字">
    这是一个 Dialog
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>
    <h1>11</h1>

    <template #footer>
      <f-button type="default">默认按钮</f-button>
      <f-button type="primary">主要按钮</f-button>
    </template>
  </f-dialog>
</template>
