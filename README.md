# Daily-notes
Web related notes.

- ##### <u>函数、对象</u>    
     `函数`、`对象`、`同步回调`、`异步回调`的理解和使用

     

- ##### <u>JS的error处理</u>   
  JS中的`错误类型`、`错误处理`、`错误对象`

  

- ##### <u>什么是Promise</u>   
  什么是Promise，Promise的基本使用

  

- ##### <u>为什么使用Promise</u>   
  为什么使用Promise，因为对比不同的回调方式，promise指定回调方式更加灵活，支持`链式调用`

  

- ##### <u>Promise API 使用</u>   
  Promise.resolve、Promise.reject、Promise.all、Promise.race

  

- ##### <u>Promise的几个关键问题</u>   
     1、error属于promise哪个状态   
     2、一个promise指定多个成功/失败回调函数   
     3、状态改变与指定回调函数的先后次序   
     4、异常传透   
     5、中断promise传递   

     

- ##### <u>async与await</u>   

   ###### 				1.async function  (function return Promise)

   - 函数返回Promise对象   

   - promise对象的结果由async函数执行的返回值决定   

     

   ###### 2.await expression (value or Promise)  

   - expression一般是Promise对象，也可以是其他值   
   - 如果是Promise对象，await返回的是Promise成功的值   

   - 如果是其他值，直接将此值作为await的返回值   

    

   ###### 3.注意 

   - await必须写在async中，但async可以没有await      

   - 如果await的Promise失败，就会抛出异常，需通过`try...catch...`捕获处理    



- ##### <u>async与await</u> 

  - 宏队列：`定时器回调`、`ajax回调`、`dom事件回调`
  - 微队列：`Promise回调`、`mutation回调`
  - JS执行时会区别对待这2个队列
    - JS引擎首先必须先执行所有的初始化同步任务代码
    - 每次准备取出第一个宏任务执行前，都要将所有的微任务一个一个取出来执行