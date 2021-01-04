[![NPM](https://nodei.co/npm/vue3-touch.png?downloads=true)](https://www.npmjs.com/package/vue3-touch)

## vue3-touch
这是一个判断滑动方向的工具，
>此工具仅支持VUE3

可以响应touchUp/touchDown/touchLeft/touchRight四个方向的事件
```js
 //安装
 npm i vue3-touch
 //index.ts
 import { createApp } from 'vue';
 import App from './App.vue';
 import VTouch from 'vue3-touch';
 //注册工具
 createApp(App).use(VTouch).mount('#app');
 
 //index.vue
 使用工具
  <div class="app" v-touch="onTouch">
  
 function onTouch(e){
  console.log(e) //返回4个值，分别是 up\down\lef\right
 }
 ```