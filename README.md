

## 第一章：前言
> 与其说这是一个入门教程，不如说是我的自学笔记。大前端的时代，工程化，组件化的思想促成了前后端分工。前端不再满足小小的页面布局，正在扮演着愈发重要的角色。整理这套笔记，我也参考了很多东西。在学习过程中，我看了三套视频教程，传智的，IT营的，慕课网的。此外，还有必读的官网教程和一本书[《深入浅出React和Redux》](https://pan.baidu.com/s/1kCh7rVkppMpMHFNiteRZlg)。这本书业界很有名，需要的点击书名即可下载，提取码：**8e31**。话不多说，下面开始正文。


### React简介
* https://reactjs.org 官网
` A JavaScript library for building user interfaces`
> 官网的解释就这一句，用于构建用户界面的js库。给我的感觉是低调奢华有内涵，实际上，你会发现，越是优秀的事物越低调。react严格上来讲同vue一样，算是库而不是框架。之所以习惯性的叫做框架，是因为它们强大的生态系统。拿react来说，UI层的react本身，数据层状态管理redux，flux，用于处理异步请求的axios，解决跨域问题的fetch-jsonp,路由react-router,此外，还有超级活跃的社区。

**火热程度**
不夸张的说，背靠脸书的react从2013发布到现在，说是全球最火也不为过。当然，这种情况在国外更明显，国内目前还是vue占上风，但react市场份额同样不小。有这样一种说法，react和vue虚拟dom设计思想的出现，终究会引领新的潮流，传统主打操作dom的jQuery将逐渐退出舞台。

**具体**
目前国内的一二线互联网公司大部分都在使用React进行开发，比如阿里、美团、百度、去哪儿、网易 、知乎这样的一线互联网公司都把React作为前端主要技术栈。或者你可以去招聘网站看看，只要是前端，基本上三大框架都要求你至少懂一个，当然，更多的要求你懂vue或者react。至于angular，相对笨重，现在份额少的可怜。

**React Fiber**
这是一个新名词，指的是react16的版本，这一版本性能和易用度上，都有很大的提升。除了火爆的react本身，还有用于移动端开发的ReactNative和用于虚拟现实技术开发的React VR。所以说，react的前景非常广，前端学习react是大势所趋。最后留个图，自行体会。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622061636959.png)
***
**学习react的优势**

* 持续高热度:关注的人多，你遇到问题解决的可能性和途径就会多。
* 良好生态:几乎所有开发需求都有成熟的解决方案。
* 官方文档超级详细：很多react相关书都是参考官方文档
* 容易上手：只需要你有基本的html+css+js基础，主要是js
* 小伙伴多：在活跃的react社区，说不定还能解决你的单身问题。



### 开车前的提醒
> 严格说，react 的学习门槛不是很高，但如果你还不知道什么是js，建议先去找门课程学一下。react对于彻底零基础的小白来说，还是有些不太好理解的地方，比如jsx语法，你会觉得很怪异。在这之前，如果你学过es6，node或者vue最好，这样你学起来会更容易。此外，你最好对包管理工具有一定的了解，项目中安装依赖会常用，比如npm或者脸书官方的yarn。



###  关于笔记阅读
> 首先，不得不重申一下，这只是笔记而已，没有视频教程。适合有一定基础的小白系统了解react使用，也适用于有一定react基础的人复习使用。基本上该上代码的地方都会上代码，也会标注我踩过的坑，这一点不必担心。如果代码量大，我会发个百度网盘链接放源码，代码量少就贴图或者粘贴代码。

**划重点，这里讲的只是react入门基础，也只涉及react本身，没有redux之类的。**



### 学习社区推荐--掘金
* 这里我只想推荐一个，[掘金](https://juejin.im/)。
* 自认为掘金是最活跃，技术含量最高的程序员社区，里边大牛很多。
* 如果你不一直摸鱼划水，在里边确实能学到很多东西。




## 第二章：react vs vue
* 最热和最火的两个框架碰到一起，关于它们的对比就永远不会少。
* 先来个简单的比较
* 相同点

```
良好的生态系统，轻量级框架。
虚拟dom
数据驱动视图，组件化思想。
```

|  |  |
|--|--|
|react优点  |
|灵活性和响应性：它提供最大的灵活性和响应能力。||
|虚拟DOM：基于文档对象模型，允许浏览器友好地以HTML，XHTML或XML格式排列文档|
|丰富的JavaScript库：来自世界各地的贡献者正在努力添加更多功能。||
|可扩展性：由于其灵活的结构和可扩展性，React已被证明对大型应用程序更好。||
|不断发展： React得到了Facebook专业开发人员的支持，他们不断寻找改进方法。||
|Web或移动平台: React提供React Native平台，可通过相同的React组件模型为iOS和Android开发本机呈现的应用程序||

**缺点**
`陡峭的学习曲线：由于复杂的设置过程，属性，功能和结构，它需要深入的知识来构建应用程序。`


* 结合vue详谈

> 与react相比，vue.js的下载量更少，并且主要用于构建有吸引力的单页面应用程序和Web应用程序。但是，vue.js具有适应性强的体系结构，使其成为广泛使用的框架之一，具有最新的库和包。

**使用vue的优缺点**
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622071313846.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)

* 个人看法：中小项目推荐vue，大项目推荐react，具体情况具体分析。
***

```
至此，理论介绍告一段落，开始飙车。请开个好车，比如vscode。
```



##  第三章：开发环境搭建
### Node.js安装
`在开始前，请确保你的电脑安装了node，不知道装没装，就命令行工具node -v 一下，有版本号是成功安装的`
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622072252224.png)

    * 没安装也不要慌，打开Node中文网址：http://nodejs.cn/
    * 下载对应你电脑的版本，要用**稳定版**，切记 。
    * 如果你用的英文官网，请看下边这个图这个，表示稳定版本
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622072553595.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
* 当然，如果你安装过了，只要版本不是差特别多就没问题，不必重装

### 安装官方脚手架create-react-app
* 这里介绍两种方式，习惯用哪个你自己选
**第一种**
	` npm install -g create-react-app `
	` create-react-app  myapp`
	
	**第二种**
	`npx  create-react-app  myapp`

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622073518837.png)
* 上述代码的myapp是项目名，可以自定义
### 项目初始化
* 安装完成后，请执行如下命令

```
cd myapp
npm start
```
* 项目名不一定要和我的一致，切换进去，启动就好
* `npm i -g yarn`(可选命令)
* 此外，你如果全局安装了yarn，用yarn start启动也行
* 安装过程可能有点慢，稍等一会儿

**效果图**
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622074305705.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622074249332.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)



## 第四章：目录结构介绍
安装完成并初始化项目后，打开项目文件夹，你会看到如下内容
我用的yarn，部分文件和npm的有差异，问题不大

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622074648146.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)

|  |  |
|--|--|
| README.md | 项目说明文件，先不用管它，等托管github或实际工作使用以markdown语法编写就好 |
|package.json|webpack配置和项目包管理文件，里边有些命令脚本和依赖，先不用管它|
|lock文件|package-lock.json或者yarn.lock都是锁定安装版本号的，保证你托管GitHub后大家下载安装的依赖是一致的|
|gitignore |git配置忽略文件，不需要上传的可以写里边，比如node_modules文件夹|
|node_modules |项目依赖包，如果你学过node，对这个应该很熟悉|
|public |开放出去的公共资源，如果你想读取本地json，请放这个目录下|
|src|放源码的位置，也是对我们开发者而言最核心的东西|




### public文件夹详解
* 初始化项目后，里边有三个小东西

* `favicon.ico : 网站图标，看，就是这玩意`
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622075909285.png)
***
* `index.html : 首页的模板文件，注释啥玩意的可以删了`
***
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622080039613.png)
* 这行代码在禁用js时候生效


` mainifest.json：移动端配置文件，先不用管。`

### src文件夹详解
*  这个目录里边放的是源代码，也是核心文件夹

    index.js : 项目的入口文件，根组件挂载根元素

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622080413857.png)

    *.css ：样式表，不用管
    App.js : 根组件
    serviceWorker.js:移动端离线浏览相关，先不用管
    logo.svg :一个小图片，也不用管

***
### hello world初识


为了后续开发方便，我们把目录精简一下，去掉css，图片等没用的东西,来个hello world
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622080906782.png)
- 记得把导入的语句一同删除（删除后文件不存在导入会报错）
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622081038446.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)

**App.js**
```js
import React from 'react';

function App() {
  return (
    <div >
      hello world
    </div>
  );
}

export default App;

```
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622081318141.png)
* 搞完了这样，页面干净的只有hello world，跑在默认的3000端口
***


## 第五章：类组件和函数组件的编写

> 在react中，一切皆组件。传统布局头部，左侧导航，主体内容，尾部，都可以看作是一个个组件，独立维护。这像搭积木，一块块的小组件最终搞出个小房子。react组件分为两种，函数组件和类组件，两者都会用到。`相比之下，类组件更普遍，但如果组件中不涉及业务逻辑，函数组件更好用些。`下边举个例子说明什么二者区别。

***
### 简单的函数组件

* 你也许会感到意外，这就是函数组件了？没错，就是这样。
```js
function Header(){
  return <h1>我是头部</h1>;
}
```
* 如何使用呢？

```js
function App() {
  return (
    <Header/>
  );
}
```
* 这样就行了

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622090055633.png)
> 仔细观察，你会发现App组件也是个函数组件。此外，组件不管是定义还是使用都是大写。确实这样，react中，区分组件和HTML标签的方式就是大小写。大写的以组件方式解析，小写的以HTML标签解析。对了，单双标签无所谓，看个人习惯。
***
### 简单的类组件

> 真正有关键字定义类是es6开始的，用class。下面用类组件改写上述App函数组件，实现相同的效果，输出hello world


```js
import React, {Component} from 'react'
class App extends Component{
    render(){
        return (
            <div>
                hello world
            </div>
        )
    }
}
export default App;
```


也许你不太理解上边的import React, {Component} from 'react'，那个大花括号，是es6的语法，解构赋值，推荐参考下阮一峰大神的[es6入门](http://es6.ruanyifeng.com/#docs/object#%E5%AF%B9%E8%B1%A1%E7%9A%84%E6%89%A9%E5%B1%95%E8%BF%90%E7%AE%97%E7%AC%A6)
* 代码中不会再写var，用let或const代替，详情参见[let](http://es6.ruanyifeng.com/#docs/let)
* 要是不理解，也可以拆分来写
import React from 'react'
const Component = React.Component

```js
import React from 'react';
const Component = React.Component;
class App extends Component {
  
  render() {
    return (
      <div>
        hello world
      </div>
    );
  }
}

export default App;
```


* export default App; 这句话是将组件暴露出去，需要的时候用import引入

### 图片资源，样式表引用问题
* 在react中，图片引入是有讲究的，分为本地图片引入和网络图片引用
* 网络图片引用和以前一样，img标签src属性写图片链接地址就行
* 本地图片这样不行，需要以路径形式导入，也要有alt属性

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622092458703.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)

* 你是否注意到，你在js文件居然引入了css文件！！！
* 这都是脚手架中webpack帮我们做的
* 如果你还不清楚webpack，请参考 https://www.webpackjs.com/

## 第六章：jsx语法
### jsx简介
> jsx是Javascript和XML结合的一种语法糖，它可以让我们更快的编写代码，属于html+js混写。这种语法最先在react中使用，后来vue中也可以，但不常见。jsx语法用熟悉了自然是快的，但对初学者而言，并不是很容易理解。

**jsx的优势**
详情参见 https://www.cnblogs.com/clearyang/p/6899639.html

* 这里简单举个例子
* jsx遇到<，就当作HTML解析，遇到{就当JavaScript解析.

* 比如我们写一段JSX语法

  *  <h1>{1+2}</h1>

***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622094428181.png)
* 可以看到，除了h1的语义，js表达式也被识别了

### jsx踩坑
* jsx中不允许用class属性，需用className代替
* 组件名必须大写
* 事件必须修正this指针，且绑定事件名时要使用小驼峰的写法onclick必须写成onClick

```js
constructor(props){
  super(props)
  this.fun = this.fun.bind(this)      
}

onClick = {() => ()} //绑定的事件名小驼峰写法
onClick = {this.fun.bind(this)}
```

* 如果写行内样式用双花括号`{{}}` `  <p style={{color:"red"}}>hello</p>`
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622095901130.png)
***
*  jsx中不允许label标签使用for属性，需用htmlFor代替
* jsx中所有的标签都必须闭合，`<br>`不行,必须`<br/>`
* jsx中注释比较讲究，` {/*JSX 中的注释方式*/}`,单行也可以

```js
{
	//jsx单行注释
}
```
* jsx语法中最外层必须有一个包裹元素，这样不行
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622095241342.png)
***
* 如果不想加一个额外元素，可以用Fragment官方提供的占位符
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622095500728.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622095440861.png)
### jsx中使用三元运算符

```js
  <h1>{false?"hello":"world"}</h1>
```
* false 显示world，true显示hello

## 第七章 传统实例-todoList
* 巴拉巴拉了半天，都是零碎的知识点，下边就用一个比较有代表意义的todoList实例来进一步体会react。

### 新建TodoList
* 将src下的App.js删除，新建TodoList.js,然后将index.js要导入的文件和挂载的组件一并修改

```js
import React from 'react';
import ReactDOM from 'react-dom';
import TodoList from './TodoList';//注意点1
import * as serviceWorker from './serviceWorker';
ReactDOM.render(<TodoList />, document.getElementById('root'));//注意点2
serviceWorker.unregister();

```

### 完善TodoList.js

```js
import React,{Fragment} from 'react'
const Component = React.Component
class TodoList extends Component {
 
  render() {
    return (
      <Fragment>
        <div><input type="text" /> <button> 添加 </button></div>
               <ul>
                   <li>学习react</li>
                   <li>学习vue</li>
               </ul> 
     </Fragment>
    );
  }
}

export default TodoList;
```
* 样式不是重点，最后会美化一下，先凑合着看
* 注意最外层包裹元素的事
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622102941108.png)
***



## 第八章：响应式设计原理和数据的绑定方法


### 响应式设计
* react中文文档有这样一段话
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622120651916.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
***
> 核心就是以数据驱动视图的改变。react并不建议你直接操作DOM元素,而是要通过数据进行驱动，改变界面中的效果。数据变了，视图就变了。mvvm框架都是如此，包括vue，也是数据驱动的形式改变视图。这对于开发者而言十分友好，只需要关注数据本身，大大提升了开发效率。

**关于vue，react，jquery的一些思考**

    * 补充一点，虽然react，vue，angular都有操控dom的钩子ref，但都不建议操作dom解决问题，除非是一些不涉及数据本身的特殊问题。
    * 在《深入浅出Reqct和Redux》这本书中，有这样一个观点：react天生就是取代jQuery的。
    * 由于历史遗留问题，jquery的市场份额依旧不小，但操控dom性能消耗确实大。
    * vue，react这种虚拟dom的设计思想底层仅仅是创建js对象，比较前后js对象是否一致，从而决定是否重新渲染，渲染哪部分。
    * 相比之下，创建对象的性能消耗肯定比创建dom低很多，jquery退出历史舞台是大势所趋。



### 数据绑定
* 需求：添加事务todo-item
* `思考： 上边说了响应式数据， 数据不能写死，要动态绑定数据。那么在哪里绑定呢？`
* 答案是：**写在构造函数里**
* 类在被加载的时候，构造函数就会被执行，不需要手动调用

```js
    constructor(props){
    //调用父类的构造函数，固定写法
    //虽然props不用可以不写，但官方推荐你这样写
        super(props) 
        this.state={
            inputValue:'' , // 关联input输入的值
            list:[]    //事务列表
        }
    }
```
`如果你学过vue，这里会更容易理解，在数据绑定这一块，vue和react差不多`

* 绑定语法很简单，就一句话：

```html
<input value={this.state.inputValue} type="text" /> 
```
* 这个时候，你可以试着改变构造函数中inputValue的值，你会发现，页面数据立刻变了。
* 此时，并不是完全没有毛毛问题的，打开控制台，你会发现这样有一个警告
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622123219745.png)
***
* 提示你在没有onChange事件处理函数的情况下为表单控件设置了value属性，这将呈现只读字段。如果字段应该是可变的，使用“defaultvalue”。否则，设置“onchange”或“readonly”。
* 说了一大堆，加个onChange事件处理函数就行了


### 事件绑定
* 这个事件绑定也很简单，一句话的事：

```js
 <input type="text" value={this.state.inputValue} onChange={this.changeInputValue} />
```
* 注意，onChange必须小驼峰
* 上边只是绑定了，但是这个方法我们还没有定义
* 这里定义方法this的指向是个大坑，一会儿会遇到
 * 我们现在要做的是获取输入的值，并赋值给state的inputValue
 * 可以用事件参数e.target.value获取输入值
* 在render外先定义个方法
* 也许你想这样写
```js
 changeInputValue(e){
        this.state.inputValue=e.target.value
    }
```
* 这样你就入坑了

**问题分析**
* react不允许直接对状态进行修改，需要使用this.setState方法
* this的指向有问题，上下文this不一致

一步步解决
`解决问题1`
```js
changeInputValue(e){
      this.setState({
        inputValue:e.target.value
      })
    }
```
`解决问题2`

```js
onChange={this.changeInputValue.bind(this)}
```
* 这个时候输入框可以正常输入值且不会报错
* 补充：这个this绑定也可以像官方文档那样提到构造函数里
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622131244195.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
***
* 也可以不绑定，方法定义时候用箭头函数

```js
changeInputValue = (e) => {
    this.setState({
      inputValue: e.target.value
    })
  }
```

 

## 第九章：列表渲染
还是那句话，数据驱动试图，数据不能写死，下面我们把自己写死的两个li去掉，遍历状态里的list。为保证数据不为空，我们在list初始化的时候就加两个数据进去。
`list: ['学习react','学习vue']`

* 重点来了
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622132004286.png)
***
* map是es6的方法，不太懂的自行补学
 **踩坑点**
* li标签的取值item不加花括号{}，报错，注意，{}是jsx语法环境，不加不识别
* 遍历的子元素没有key值，什么叫没有key值，就是上边那样
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019062213232742.png)
***
* 在这里可以先用索引代替，但并不是个好方法
* `    return <li key={index}>{item}</li>`
 
 ### 关于遍历子元素使用索引做key的弊端

> 之前说过，react是基于虚拟dom的，涉及diff算法。先看下下边这个图
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622132758440.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
***
* 虚拟dom会创建两个js的对象用于前后数据比对，来决定是否更新数据。如上图那样，这两个对象的依赖是靠索引建立的，这样的话，一旦索引发生改变，这个依赖就需要重新建立，白白浪费了时间，有性能问题。建议在数据源上加个id标识作为key，或者使用自身作为key，即a对a，b对b

***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622133315362.png)
*** 
### 添加事务
* 折腾半天，下边为按钮添加事件处理函数，方法和之前一样
```html
  <button onClick={this.addTodoItem}> 添加 </button>
```
```js
  addTodoItem=()=>{
    this.setState({
      list: [...this.state.list,this.state.inputValue],
      inputValue:""// 输入框置空，方便下次输入
    })
  }
```
* 上述...是es6扩展运算符，相当于将上述 list: ['学习react','学习vue']，拆解为'学习react','学习vue'，然后和后加入的一项重新组成新数组['学习react','学习vue','新事务']
***
### 键盘监听
* 下面实现一个敲回车添加的功能
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622134559613.png)
***

```js
 enterAdd=(e)=>{
    if(e.keyCode===13){
      this.addTodoItem();
    }
  }
```

###  删除事务
* 现在我们想实现这样一个功能，点击某一项可以删除它
* 核心点两个，传递参数，调用数组的splice方法

* 为ul的每个li注册点击事件，并把索引传过去

```js
  return <li key={item}  onClick={this.delTodoItem.bind(this,index)}>{item}</li>
```
* delTodoItem

```js
 delTodoItem=(index)=>{
    let list=this.state.list;//备份下数据，不要直接修改
    list.splice(index,1)
    this.setState({
      list: list//其实这里可以简写为一个list
    })
  }
```
### 全部代码

```js
import React, { Fragment } from 'react'
const Component = React.Component
class TodoList extends Component {
  constructor(props) {
    super(props) //调用父类的构造函数，固定写法，虽然props不用可以不写，但官方推荐你这样写
    this.state = {
      inputValue: '', // 关联input输入的值
      list: ['学习react','学习vue']    //事务列表
    }
  };

  changeInputValue = (e) => {
    this.setState({
      inputValue: e.target.value
    })
  }
  addTodoItem=()=>{
    this.setState({
      list: [...this.state.list,this.state.inputValue],
      inputValue:""
    })
  }
  enterAdd=(e)=>{
    if(e.keyCode===13){
      this.addTodoItem();
    }
  }

  delTodoItem=(index)=>{
    let list=this.state.list;
    list.splice(index,1)
    this.setState({
      list: list
    })
  }
  render() {

    return (
      <Fragment>
        <div>
          <input onKeyUp={this.enterAdd} type="text" value={this.state.inputValue} onChange={this.changeInputValue} />
          <button onClick={this.addTodoItem}> 添加 </button>
        </div>
        <ul>
          {
            this.state.list.map((item,index)=>{
              return <li key={item}  onClick={this.delTodoItem.bind(this,index)}>{item}</li>
            })
          }
        </ul>
      </Fragment>
    );

  }
};

export default TodoList;
```

## 第十章 开发辅助
> 这里介绍一款好用的vscode插件。俗话说，磨刀不误砍柴工，刀快才好用，开发也是这个道理，有优秀的编辑器，优秀的插件，没理由不用啊。

### 插件推荐
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019062214101888.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
***
* 安装很简单，插件商店一搜就好了，完事点安装
* 使用看文档，都很清晰

* 举几个例子
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622141315735.png)

***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622141417849.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
*** 
* 具体的自行感受，给我的感觉是6的飞起，越来越喜欢vscode

### 自定义代码段
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622141644943.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
***
* 你也可以按需要自己搞一搞
### 快捷键映射
* 之前我一直用sublime，快捷键也用习惯了，还好vscode支持快捷键映射
* 还是刚才那个界面，点击按键映射
* 下载，完活!
***
[在这里插入图片描述](https://img-blog.csdnimg.cn/201906221419217.png)
***

 ##  第十一章 组件拆分
>  上边我们已经实现了todoList的基本功能，但是，都堆在一个文件里，不太好看，需要抽离一下。可以将每一个li抽成一个小组件TodoItem。



### 创建TodoItem小组件

```js
import React, { Component } from 'react';
class TodoItem extends Component {
    constructor(props) {
        super(props);
        this.state = {  };
    }
    render() {
        return (
            <h1>TodoItem</h1>
        );
    }
}

export default TodoItem;
```
试着在TodoList里边使用一下

**TodoList.js**
* 导入
```js
import TodoItem from "./TodoItem";
```
* 使用
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019062214310129.png)
* 效果图
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622143148317.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
***
* 这里我们改一下最开始的代码，让代码看起来更简洁
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622143252243.png)

 **进一步拆分**
 ***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622143626814.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)

***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622143653851.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
***
* 接下来，重点来了，以上的拆分还不健全，因为数据都在父组件，儿子TodoItem还毛毛都没有呢。

### 父->子组件传值
* 最基础的，属性传值就好，像这样
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622144802622.png)
* 上述的父->子传值就结束了，todo_item是自定义的，保证和儿子接收的名字一样就行
* 子组件需要用this.props.xxx的形式进行接收，这里就是this.props.todo_item
* 子组件
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622144908910.png)

* 你会发现控制台报错了，还是key的问题。
* 你是不是想接着传值，像刚才那样？
* 如果是，恭喜你，又踩坑了。
* 此时，我们已经抽了一个小组件出来，key应该加在小组件上，而不是小组件里边的li身上
### 子->父组件传递数据
* 上述添加没问题，但是删除抽离后还没有搞。我们想抽离后实现抽离前的效果，问题来了，现在关键就是在子组件中调用父组件的删除方法。

**问题关键**
* 传方法
* 传索引
* 子组件定义方法并接收父组件传递的数据，执行事件处理函数
* 子组件通过调用父组件的方法实现数据回传

父组件--传方法--传索引
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622150811161.png)
子组件--定义方法--点击执行事件处理函数--本质就是执行父组件的删除方法
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622150933258.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)

## 全部代码
***
[链接](https://pan.baidu.com/s/14aw3-QaumZQKbUK2jLZyBw) 提取码：x47l 
* 使用的话先npm i 安装下依赖


## 第十二章：数据流方向
>  如果你之前学过angular，你应该知道双向数据绑定这个概念，指令是ng-model。angular是双向数据流，父子组件通信相对方便。但有些时候，我们不想儿子改变父亲的值，只能用，不能改。react这点最明显，vue中表单控件还有个v-model双向数据绑定的指令。

* 还是上边的例子，在父组件传值的时候可以把list直接传过去，但是对子组件是只读的，一旦你试图修改就会报错。在不考虑redux，flux等状态管理框架的时候，父子组件通信常用的就是上边的方法。


### 与jQuery结合
*  首先，确实这两个可以一起用。
* react只关心挂载的根元素root，其他的不关心，爱咋搞咋搞。
* 换句话说，jquery不操控root内的元素就没事

**纠结点**
 * 实际上，这个问题没什么实际意义，技术选型本身就有问题
 * 一个主张操控dom，一个不推荐操控dom，把这两个放一起打架吗？

* 也许你想试试，好，那就试试

* 打开public文件夹下的index.html,没用注释删除

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <link rel="shortcut icon" href="%PUBLIC_URL%/favicon.ico" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta name="theme-color" content="#000000" />
    <link rel="manifest" href="%PUBLIC_URL%/manifest.json" />
    <title>React App</title>
  </head>
  <body>
    <noscript>You need to enable JavaScript to run this app.</noscript>
    <div id="root"></div>
   <script src="https://cdn.bootcss.com/jquery/3.4.1/jquery.min.js"></script>
   <script>alert($)</script>
  </body>
</html>
```
* 确实能用，但没什么卵用
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622152852663.png)
***
## 第十三章：调试工具react developer tools的使用

### 简介
> 如果你不是前端小白，懂最基础的调试，那你应该知道一个好的调试工具的重要性，比如谷歌开发者工具。火爆的react也有对应的调试工具，react developer tools。不想翻墙，用qq浏览器就行，它可以关联到谷歌应用商店，不用翻墙就能下载。


* 这个东西有三种状态，像下图这样，就是与react无关时候的状态。
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019062215340941.png)
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622153515191.png)
***
 * 这种说明页面是react相关，且是开发环境，比如我们的myapp
 ***
 ![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622153608424.png)
 ***
 * 打开知乎，就这样，说明是生产环境的react

### 使用
* 给个图，自行体会吧。
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622153818515.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
***
## 第十四章：PropTypes类型检查
### 介绍
> js是基于面向对象思想的语言，不是真正的面向对象语言，在类型检测上并不完善，这也是typescript大火的原因之一。上述在在父组件向子组件传递数据时，并没有对传递的属性值进行限制，想传什么传什么，自由度太高。这在工作中是完全不允许的，大型项目，缺少必要校验，后期维护极为坑。

### 使用
* 引入 `import PropTypes from 'prop-types';`

import PropTypes from 'prop-types'
* 类外部使用

```
xxx.propTypes={
       p1:PropTypes.string.isRequired,
       p2:PropTypes.func,
       p3:PropTypes.number
}
```
---
xxx是类名（组件名）
p表示传递过来的属性
其他的见明知意，不解释了

### 默认值defaultProps

* 有些属性限定是isRequired，但是又不想传，就用defaultProps 

```
xxx.defaultProps = {
 	   p:'...'
}
```

## 第十五章：ref的使用
### 说明
> react，涉及dom操作的都不推荐，ref也是如此，当然，ref也不是一无是处。

### 简单使用
* 设置
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622160438414.png)
* 使用
	* 此时，e.target.value就被取代了
	* 事件参数e也没用了，可以去掉
	
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622160505640.png)
***
* 你还可以这样用
* ` ref={(input)=>{this.input=input}}`
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622160830358.png)
* 补充：this.setState()是异步的，如果你想操控dom，可以写在它的回调函数里。



## 第十六章：生命周期
* 很重要的东西，先来个图
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622161444469.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
***
### 简介
> 生命周期就像一个人出生到死亡的过程，在react中，这些生命周期钩子函数十分有用，很多场合我们都会遇到。此外，值得注意的是，react每个组件都有上述提到的所有周期函数，并不是根组件或父组件才有。严格说，生命周期函数会在组件渲染到销毁这个过程的某一个时刻自动执行，不需要你多费心。但是render特别，所有的生命周期函数react都有默认实现，唯独没有render的实现。也就是说，组件里你可以什么周期函数都不写，构造函数也可以不要，但是不写render不行。

### 初始化阶段
> 这个阶段主要是定义属性（props）和状态(state)，当然，还有this指向的绑定。
> 在构造函数中，constructor是一个特别的存在，算不算生命周期函数都行，看你怎么理解。
> 构造函数在类加载就会自动执行，完成数据初始化。
> 如果你学过java，这点应该体会的更清楚，有参构造，无参构造，构造方法重载巴拉巴拉。。。

### Mounting阶段
**componentWillMount** 
> 在组件即将被挂载到页面的时刻执行，只执行一次，没啥鸟用，就是个陪跑的对称函数.能在这里放的，直接放构造函数就行。

**render** 
*  页面state或props发生变化时执行。

**componentDidMount** 
> 组件挂载完成时被执行,只执行一次。这个好用，基本上ajax请求都在这里发。

**补充：生命周期函数执行顺序与你书写顺序无关。**

### update阶段
  **componentWillReceiveProps**
  > 子组件接收到父组件传递过来的参数，且父组件render函数重新，非第一次存在dom中被执行，不太常用。

  
**shouldComponentUpdate（nextProps,nextState）**
> 该函数会在组件更新之前，自动被执行。它要求返回一个布尔类型的结果，必须有返回值，默认是true，如果是false，后续组件就不会进行更新。可以用来做性能优化，比较组件前后状态属性是否一致，不一致才去更新。



 **componentWillUpdate**
> 用处不大，发生在组件更新前，如果shouldComponentUpdate返回false，这个函数就不执行了

 **componentDidUpdate**
* componentDidUpdate 组件更新之后执行




### 销毁阶段

**componentWillUnmount**
> 你也许会好奇，别的函数都是兄弟姐妹的，这个就没陪跑的吗？
> 确实没有，销毁就销毁了，没啥好接着做的。
> 在这里可以做些善后工作，清除定时器啥的。


## 第十七章 axios发送 ajax请求
* 首先说明一点，axios不是react独有，vue也可以用
* 第三方的东西使用起来三步走
* 第一，安装，第二，查文档，第三，复制粘贴


### 安装
npm install -save axios
或者 yarn add axios

### 使用
[文档](https://www.npmjs.com/package/axios)  
```js
const axios = require('axios');
import axios from 'axios' // 也行
axios.get(apiUrl)
  .then(function (response) {
    // handle success
    console.log(response);
  })
  .catch(function (error) {
    // handle error
    console.log(error);
  })
  .finally(function () {
    // always executed
  });
```

  ### 扩展--fetch-jsonp
* 这个不支持jsonp跨域，需要的话可以用fetch-jsonp
* [文档](https://www.npmjs.com/package/fetch-jsonp)

 **安装**
npm install fetch-jsonp

**使用**
```js
import fetchJsonp from 'fetch-jsonp'
fetchJsonp('/users.jsonp')
  .then(function(response) {
    return response.json()
  }).then(function(json) {
    console.log('parsed json', json)
  }).catch(function(ex) {
    console.log('parsing failed', ex)
  })
```

        
## 第十八章 生产环境vs开发环境
	极致快vs高效率
* 前者代码需要压缩，后者不需要
* 前者删除注释，后者不需要
* 前者不需要热更新，后者需要
* 测试工具前者不需要，后者需要
* 语法检查工具前者不需要，后者需要
** **


## 第十九章 动画--react-transition-group
* [超级详细的官方文档](https://reactcommunity.org/react-transition-group/css-transition)


## 第二十章 redux+antd+react实现todoList
* [感兴趣的戳这里](https://blog.csdn.net/qq_42813491/article/details/93201947)
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622172035806.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
***
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190622172007761.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQyODEzNDkx,size_16,color_FFFFFF,t_70)
