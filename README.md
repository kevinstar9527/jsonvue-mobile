# jsonvue-mobile

#### 介绍
jsonvue-mobile 是基于Vue2 和 Vant 的移动端微代码表单库，仅需少许配置即可生成对应的表单页面。更专注于表单字段联动设计提供多种联动方式（命令式和响应式）

#### 安装教程

1.  安装相关依赖文件

```
npm install jsonvue-mobile vant@2.11.0 vee-validate@3.4.15
```

2.  在main.js 中初始化

```
//引入vant
import Vant from 'vant';
import 'vant/lib/index.css';

//引入vee-validate
import {ValidationObserver,ValidationProvider，extend,localize} from "vee-validate";
Vue.component('ValidationProvider',ValidationProvider)
Vue.component('ValidationObserver',ValidationObserver)

//引入jsonvue-mobile
import JSONVIEW from 'jsonvue-mobile'
import 'jsonvue-mobile/dist/components.esm.css'
Vue.use(JSONVIEW)

JSONVIEW.initValidate(extend,localize)
```

#### 使用说明
https://blog.csdn.net/u011663865/article/details/135463025?spm=1001.2014.3001.5502