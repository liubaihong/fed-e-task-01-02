### fed-e-task-01-01 作业
1. 简答题
    1. 请说出下列最终的执行结果，并解释为什么   
    答：10， 因为循环结束后，i的值为10

    2. 请说出下列最终的执行结果，并解释为什么
    答：报错， 因为let定义的变量不会提升的作用域顶部，所以打印时无法初始化

    3. 结合ES6新语法，用最简单的方式找出数组中的最小值
    答：var arr = [12, 34, 32, 89, 4];
        const getMin = arg => Math.min(...arg);
        getMin(arr);
    
    4. 请详细说明var，let, const三种声明变量的方式之间的具体差别
    答：1、var作用域是整个封闭的函数，是全域；let, const是块级作用域；
        2、var会变量提升（作用域顶部初始化），只要在作用域内，即使在声明前使用也不会报错。let和const没有变量提升，在声明之前使用会报无法初始化
        3、let, const在相同作用域内不能重复声明
        4、const声明后不能修改，对象指的是不能修改指针
    
    5. 请说出下列最终的执行结果，并解释为什么
    答：20，因为箭头函数里面的this是创建环境的上下文而不是调用环境

    6. 简述Symbol类型的用途
    答：Symbol是一种新的原始数据类型，表示独一无二的值，可以用来作为变量、属性或函数名称，避免名称重复产生不必要错误。

    7. 说说什么是浅拷贝，什么是深拷贝
    答： 浅拷贝和深拷贝一般是相对于对象来说的，对象存储在堆内存中，浅拷贝只是复制了指针，原对象和拷贝对象指向同一个内存地址。深拷贝是将拷贝的值放入一个新的堆内存中，相互独立，互不影响。

    8. 请简述TypeScript与JavaScript之间的关系
    答： TypeScript是javascript的超集或者语法糖，最后还是编译为javascript执行。

    9. 请谈谈你所认为的TypeScript优缺点
    答：优点：1、类型系统的使用，尽可能避免因js弱类型带来的不确定性错误。
             2、增加代码的可维护性和可读性，使代码结构更清晰


        缺点：1、本身多了很多概念和语法，提高了js学习成本
              2、小项目会增加项目开发成本
              3、可能和一些js库结合的不是很好

    10. 描述引用计数的工作原理和优缺点
    答：工作原理：用一个计数器来维护对象的引用数，监控对象引用关系变化，判断当前引用数是否为0，为0则将空间释放和回收
    
        优点：1、发现垃圾时立即回收 
             2、最大限度减少程序暂停

        缺点：1、无法回收循环应用的对象
              2、时间开销大

    11. 描述标记整理算法的工作流程
    答：遍历所有对象---》找到所有活动对象（可达对象）并标记---》遍历所有对象---》移动没有标记对象到地址连续空间---》清除，回收空间

    12. 描述V8中新生代存储区垃圾回收的流程
    答：遍历所有对象---》找到所有活动对象并标记---》整理活动对象到地址连续空间---》将活动对象拷贝至To空间---》From与To交换空间完成释放

    13. 描述增量标记算法在何时使用及工作原理
    答：在内存未到上限时使用，原理：在程序执行空档期增量遍历标记（执行和标记交替进行），标记完成后清除垃圾，回收空间




    


    
