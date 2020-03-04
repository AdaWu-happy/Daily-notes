# Daily-notes
Web related notes.

1.  函数、对象    
函数、对象、同步回调、异步回调的理解和使用

2. JS的error处理   
JS中的错误类型、错误处理、错误对象

3. 什么是Promise   
什么是Promise，Promise的基本使用

4. 为什么使用Promise   
为什么使用Promise，因为对比不同的回调方式，promise指定回调方式更加灵活，支持链式调用

5. Promise API 使用   
Promise.resolve、Promise.reject、Promise.all、Promise.race

6. Promise的几个关键问题   
  1、error属于promise哪个状态   
  2、一个promise指定多个成功/失败回调函数   
  3、状态改变与指定回调函数的先后次序   
  4、异常传透   
  5、中断promise传递   
 
7. async与await   
<br>  1.async function (function return Promise)   
    + 函数返回Promise对象   
    + promise对象的结果由async函数执行的返回值决定   
<br>  2.await expression (value or Promise)  
    + expression一般是Promise对象，也可以是其他值   
    + 如果是Promise对象，await返回的是Promise成功的值   
    + 如果是其他值，直接将此值作为await的返回值   
<br>  3.注意   
    + await必须写在async中，但async可以没有await   
    + 如果await的Promise失败，就会抛出异常，需通过try...catch...捕获处理  
  
