## 控制器的特点

    1.创建控制器会有一个$scope,
    2.依赖注入
    3.DOM与控制器作用范围平行
    4.控制器可以嵌套使用，注意嵌套的是DOM标签
    5.控制器不能复用，而且作用仅仅是控制唯一可以操作的地方
    
    
##  ng-options="option.id as option.title for option in curOptionArray"

    可以理解成一个ng的语法 
    option.id是select提交的值 
    option.title是select显示的值 
    option代表数组curOptionArray里面的当前元素
    
    $sce 帮我们把html转译的
    依赖注入：你只要想使用，就要把它先注入进来
    
## 指令---扩展功能，封装插件

    装饰型指令（美化，增加功能）
    组件型指令 （编译一些功能，实现例如弹层，表格等效果）
    
    指令可以完全不依赖控制器
    通过模块来创建指令
    创建标签的规范：标签里不出现大写字母
    myHello----->第一个参数：代表指令名字
    template:'<h>hello</h><p>jlsajlkj</p>' -----> 第二个参数：代表定义默认返回对象
    
    var app=angular.module('appModule',[]);
        app.directive('myHello',function(){
            return {
                template:`<h>hello</h><p>jlsajlkj</p>`
            }
        })
        
        
    var app=angular.module('appModule',[]);
        app.directive('drag',function(){
            return {
                //link函数时唯一一个可以操作dom的地方,将我们的视图和数据进行绑定的（链接函数）
                link:function(scope,element,attrs){
                    //angular.element(div);//angular.element包住的对象就是一个jQuery对象
                    //scope代表当前元素
                    //element当前指令所在的元素默认为jq对象
                    // attrs表示当前元素属性
                }
            }
        })
        
##  利用es6的标签实现字符串快速拼接-----前提是用最新的wb版本
    
    用法举例：
    var name='zf';
    var age=8;
    console.log(``)

    ``
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    

