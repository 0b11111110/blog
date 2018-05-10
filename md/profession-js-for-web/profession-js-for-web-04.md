- 语句
    - if
    - do-while
    - while
    - for
    - for-in
        - 枚举对象属性
        - ECMAScript 对象属性没有顺序，因此 for-in 循环输出的属性名的顺序是不可预测的
    - label
        - 可由 break 或 continue 引用，一般都要与循环语句配合使用。（多在返回多层循环时使用）
    - break 和 continue
    - with
        - 将代码的作用域设置到一个特定的对象中
    - switch
        - 比较值时使用的是全等操作符，不会发生类型转换
        - switch 语句中可以使用任何数据类型
        - case 的值不一定是常量，也可以是变量，甚至是表达式

- 函数
    - 执行完 return 语句之后停止并立即退出，之后的任何代码都不会执行
    - return 语句可以不带任何返回值，默认 undefined
    - ECMAScript 函数中的参数在内部是用一个数组来表示的。在函数体内可以通过`arguments对象`（并不是Array实例）来访问这个参数数组
    - arguments 的值永远与对应`命名参数`的值保持同步（但并不是相同的内存空间）
    - arguments 对象的长度（length）是由传入参数的个数决定的，不是由定义函数时的命名参数的个数决定的
    - ECMAScript 函数没有签名（因为其参数是由包含零或多个值的数组来表示的），所以无法实现真正意义上的重载。不过通过检查传入参数的类型和数量并作出不同的反应，可以模仿方法的重载
    - JavaScript 核心语言特性在 ECMA-262 中是以名为 ECMAScript 的伪语言的形式来定义的。包含了所有基本的语法、操作符、数据类型以及完成基本的计算任务所必需的对象，但没有对取得输入和产生输出的机制作出规定。