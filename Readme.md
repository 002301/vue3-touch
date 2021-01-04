[![NPM](https://nodei.co/npm/vue3-touch.png?downloads=true)](https://www.npmjs.com/package/vue3-touch)

## vue3-touch
This is a tool that responds to the sliding direction

Can respond to events in four directions: touchUp/touchDown/touchLeft/touchRight

这是一个判断滑动方向的工具，

可以响应touchUp/touchDown/touchLeft/touchRight四个方向的事件
```js
 //npm install
 npm i vue3-touch
 //index.ts
 import { createApp } from 'vue';
 import App from './App.vue';
 import VTouch from 'vue3-touch';
 createApp(App).use(VTouch).mount('#app');
 
 //index.vue
 
<template>
  <div class="app" v-touch="onTouch">

  </div>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator';
@Component({})
export default class App extends Vue{

    private onTouch(e) {
      console.log(e) // up/down/left/right
    }
}
</script>

<style lang="scss" scoped>
.app{
    width:100%;
    height:100%;
}
</style>
 ```