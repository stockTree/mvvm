# mvvm
1.实现的页面效果（双向绑定效果）
在input内输入内容会展现在下方，点击input会触发绑定的点击事件

2mvvm 由model view viewmodel组成
单向：view是视图，model是数据，用viewmodel把model显示到view上
双向：用viewmodel把model显示到view上，同时可以操作view,通过viewmodel把修改的的数据返回到model中。


里面用到了数据劫持Object.definedProperty(obj,prop,descript)的属性描述和存取描述，
还用到了观察者模式，自己是观察者对内容进行订阅，当内容改变的时候，调用自己的update方法更新。
