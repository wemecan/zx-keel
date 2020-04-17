# zx-Keel(作者:初志鑫<1204505056@qq.com>)

## 注意事项

```
只能用于Vue CLI项目

```

## 鸣谢

```
努力了这么久,终于成了一名合格的代码搬运工,我只是有幸站在了巨人的肩膀上,感谢自己,感谢巨人...

```

## 实现功能

```
1.参考antdesign实现页面加载的骨架屏效果

```

### 商务合作与赞赏

```
邮箱  1204505056@qq.com
QQ 1204505056

如果你觉得这个项目帮助到了你，你可以赞赏一下作者:
```

![image](https://raw.githubusercontent.com/chuzhixin/donate/master/donation.png)

## 安装方法

```
cnpm i -S zx-Keel

```

### keel 组件 main.js 全局引入

```
import Vue from 'vue'
import {Keel,Heading,Img,Text} from 'zx-Keel'
Vue.component('byui-Keel', Keel)
Vue.component('byui-Keel-Heading', Heading)
Vue.component('byui-Keel-Img', Img)
Vue.component('byui-Keel-Text', Text)

```

### template 完整示例

```
<template>
	<div id="app">
		<byui-Keel v-if="show">
			<byui-Keel-Heading :Img="true" />
			<byui-Keel-Text :lines="5" />
		</byui-Keel>
	</div>
</template>

<script>
export default {
	name: 'app',
	data() {
		return {
			show: true
		};
	},
	mounted() {
		setTimeout(() => {
			this.show = false;
			alert('加载完成,关闭龙骨')
		}, 3000);
	}
};
</script>

<style>
body {
	margin: 0;
	padding: 0;
}
#app {
	font-family: 'Avenir', Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	Text-align: center;
	color: #2c3e50;
	padding: 20px;
}
</style>


```
