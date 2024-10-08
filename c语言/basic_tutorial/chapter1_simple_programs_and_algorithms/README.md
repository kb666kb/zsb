
### 第一节：C语言的32个关键字

C语言中有一些特殊的单词，称为**关键字（Keywords）**，它们在语言中有特定的含义和用途，不能用作变量名、函数名等标识符。以下是C语言的32个关键字：

- **auto**: 用于声明自动存储期的局部变量。
- **break**: 用于立即退出最内层的循环或switch语句。
- **case**: 用于switch语句中，指定一个条件分支。
- **char**: 数据类型关键字，用于声明字符型变量。
- **const**: 用于声明一个常量，其值在程序运行期间不可更改。
- **continue**: 用于跳过当前循环的剩余部分，并开始下一次循环迭代。
- **default**: 在switch语句中，当没有case匹配时执行的默认分支。
- **do**: 与while结合使用，构成do-while循环结构。
- **double**: 数据类型关键字，用于声明双精度浮点型变量。
- **else**: 与if语句结合使用，指定if条件不满足时执行的代码块。
- **enum**: 枚举类型关键字，用于声明一组命名的整型常量。
- **extern**: 声明一个全局变量的引用，表示变量定义在别的文件中。
- **float**: 数据类型关键字，用于声明单精度浮点型变量。
- **for**: 用于创建一个for循环。
- **goto**: 无条件跳转到程序中同一函数内的标签。
- **if**: 用于条件判断，根据条件执行不同的代码块。
- **int**: 数据类型关键字，用于声明整型变量。
- **long**: 数据类型关键字，用于声明长整型变量。
- **register**: 建议编译器尽可能将变量存储在CPU寄存器中。
- **return**: 从函数返回一个值，并结束函数执行。
- **short**: 数据类型关键字，用于声明短整型变量。
- **signed**: 表明一个整型变量是有符号的。
- **sizeof**: 运算符，用于获取数据类型或变量的大小（以字节为单位）。
- **static**: 用于声明静态存储期的变量，或指定函数内部的静态链接。
- **struct**: 结构体类型关键字，用于声明结构体类型。
- **switch**: 用于基于不同的情况执行不同的代码块。
- **typedef**: 用于为已存在的数据类型创建一个新的别名。
- **union**: 联合类型关键字，用于声明一个可以存储不同类型数据的变量。
- **unsigned**: 表明一个整型变量是无符号的。
- **void**: 数据类型关键字，用于声明无返回值的函数或无类型的指针。
- **volatile**: 告诉编译器该变量的值可能在外部被改变，不要进行优化。
- **while**: 用于创建一个循环，循环条件为真时重复执行代码块。

### 第二节：C语言的标识符

#### 标识符的定义

在C语言中，标识符是用来标识变量、函数、数组、结构体等实体的名字。标识符为程序中的各种元素提供了一个唯一的名称，使得程序员可以通过这些名称来引用它们。

#### 标识符的命名规则

1. **首字符规则**：标识符的第一个字符必须是字母（a-z或A-Z）或下划线（_）。
2. **后续字符规则**：标识符的后续字符可以是字母、数字（0-9）或下划线。
3. **长度限制**：虽然C语言标准没有明确限制标识符的最大长度，但编译器可能有长度限制，通常建议不超过31个字符。
4. **关键字不可用**：标识符不能与C语言的关键字相同。

#### 标识符的命名习惯

- **驼峰命名法**：多个单词组合时，除第一个单词外，每个单词的首字母大写，如`myVariable`。
- **下划线命名法**：多个单词之间使用下划线连接，如`my_variable`。
- **匈牙利命名法**：在变量名前加上小写字母表示变量类型，如`iCount`表示整型变量。

#### 标识符的使用示例

```c
int myNumber; // 一个整型变量
float averageScore; // 一个浮点型变量
void printMessage(); // 一个函数
```

#### 注意事项

- **清晰性**：标识符应尽量描述其用途或含义，避免使用无意义的字符组合。
- **一致性**：在同一个项目中，应保持命名风格的一致性。
- **避免冲突**：避免使用与标准库函数或类型相同的标识符，以免造成冲突。

通过合理使用标识符，可以提高代码的可读性和可维护性。在编写代码时，始终牢记良好的命名习惯对于团队协作和代码长期维护的重要性。

### 第三节：最简单的C语言程序

#### “Hello World！”

```c
#include <stdio.h>
main()
{
    printf("Hello World!");
}
```

#### C语言程序结构

C语言程序的结构特点如下：

- **预处理指令**：以`#`开头的指令，如`#include`，用于包含头文件或定义宏等。
- **主函数**：`main`函数是每个C程序的入口点，必须存在。它返回一个整数，通常`0`表示程序正常结束。
- **函数体**：包含在大括号`{}`内的代码块，是程序执行的主体。
- **输出函数**：`printf`是标准库中的输出函数，用于向控制台输出信息。
- **返回语句**：`return`语句用于结束函数执行，并可返回一个值给操作系统。
- **终止符**：`;`作为语句终止符。
- **注释符**：`/* */`作为注释符，在这个符号里面可以写一些注释内容。

C语言程序的格式特点如下：

- 一般习惯用小写字母，大小写敏感。
- 不使用行号，无程序行概念。
- 可使用空行或空格，常用锯齿形书写格式。

### 第四节：运行C程序的步骤和方法

#### 1. 编写源代码

首先，使用文本编辑器（如Notepad++, Sublime Text, Visual Studio Code等）编写C语言源代码，并保存为`.c`扩展名的文件。例如，创建一个名为`hello.c`的文件，内容如下：

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

#### 2. 编译源代码

编写完源代码后，需要使用C编译器将其编译成机器语言。常见的C编译器有GCC（GNU Compiler Collection），它通常包含在Linux发行版中，并可通过MinGW在Windows上使用。

##### 在Linux上编译

打开终端，使用以下命令编译`hello.c`文件：

```bash
gcc hello.c -o hello
```

这将编译`hello.c`文件，并生成一个名为`hello`的可执行文件。

##### 在Windows上编译

如果你使用的是MinGW或Cygwin，可以在命令行中使用类似的命令：

```bash
gcc hello.c -o hello.exe
```

这将生成一个名为`hello.exe`的可执行文件。

#### 3. 运行程序

编译成功后，你将得到一个可执行文件。接下来，根据你的操作系统运行这个文件。

##### 在Linux上运行

在终端中，你可以通过以下命令运行程序：

```bash
./hello
```

这将执行程序并输出：

```bash
Hello, World!
```

##### 在Windows上运行

在命令行中，你可以直接输入：

```bash
hello.exe
```

或者双击生成的`hello.exe`文件（在文件管理器中）来运行程序。

#### 注意事项

- 确保编译器安装正确，并且环境变量配置得当，以便在命令行中直接调用编译器。
- 如果编译过程中出现错误，编译器会显示错误信息。根据提示修改源代码，然后重新编译。
- 在不同的操作系统和环境中，编译器的安装和使用可能会有所不同。确保遵循适用于你系统的指南。

### 第五节：C语言程序的算法

#### 1. 什么是算法

##### 1. 算法的定义

算法是解决特定问题的一系列定义明确的计算步骤。在计算机科学中，算法是指导计算机如何执行特定任务的一组指令。算法可以用于各种计算任务，从简单的数学运算到复杂的数据处理和分析。

##### 2. 算法的特点

- **有限性**：算法必须在有限步骤后终止。
- **确定性**：算法的每一步骤都必须清晰无歧义。
- **输入**：算法有零个或多个输入。
- **输出**：算法至少有一个或多个输出。
- **有效性**：算法的每一步骤都必须足够基本，能够被精确地执行。

##### 3. 算法的重要性

在C语言程序设计中，算法是核心部分。一个高效的算法可以显著提高程序的性能和资源利用率。算法的选择和设计直接影响到程序的运行速度、内存使用和可维护性。

##### 4. 如何表示算法

算法可以用多种方式表示，包括自然语言描述、流程图、伪代码等。在C语言中，算法通常通过编写源代码来实现。

###### 示例：计算两个数之和的算法

**伪代码**：

```
开始
     输入两个数 a 和 b
     计算 sum = a + b
     输出 sum
结束
```

**C语言代码**：

```c
#include <stdio.h>

int main() {
    int a, b, sum;
    printf("请输入两个整数：");
    scanf("%d %d", &a, &b);
    sum = a + b;
    printf("两数之和为：%d\n", sum);
    return 0;
}
```

##### 2. 简单的算法举例：求和1~100

求和1到100是一个经典的算法问题，通常用来演示循环结构和累加过程。这个问题的目标是计算从1加到100的总和。

##### 3. 算法步骤

1. 初始化一个变量（例如sum）用于存储总和，初始值设为0。
2. 使用循环结构，从1迭代到100。
3. 在每次迭代中，将当前的迭代值加到sum变量上。
4. 循环结束后，输出sum变量的值，即为所求的总和。

##### 4. C语言实现

以下是使用C语言实现求和1到100的代码示例：

```c
#include <stdio.h>

int main() {
    int sum = 0;
    for (int i = 1; i <= 100; i++) {
        sum += i;
    }
    printf("1到100的总和是：%d\n", sum);
    return 0;
}
```

##### 5. 算法分析

这个算法的时间复杂度为O(n)，其中n是循环的次数，在这个例子中为100。这是一个线性时间复杂度的算法，意味着随着n的增加，算法所需时间成线性增长。

##### 6. 结语

通过这个简单的例子，我们可以看到算法在解决实际问题中的应用。虽然求和1到100是一个基础问题，但它展示了算法设计的基本原则，如初始化、迭代和累加。掌握这类基础算法对于解决更复杂的编程问题是非常有帮助的。

#### 3. 算法的特性

算法具有以下五个基本特性：

##### 1. 有穷性（Finiteness）

算法必须在有限步骤后终止。这意味着算法的执行过程是有限的，不会无限进行下去。

##### 2. 确定性（Definiteness）

算法的每一步骤都必须是清晰且无歧义的。对于相同的输入，算法的每一步都应该产生相同的结果。

##### 3. 输入（Input）

算法可以有零个或多个输入。这些输入是算法开始执行前必须提供的数据。

##### 4. 输出（Output）

算法至少有一个或多个输出，这些输出是算法执行结果的表示。输出应满足问题的要求。

##### 5. 有效性（Effectiveness）

算法的每一步骤都必须足够基本，能够被精确地执行。这意味着算法中的每一步骤都可以通过有限次数的基本操作来完成。


#### 4.怎样表示一个算法

可以用不同的方法表示算法，常用的有：

- 自然语言
- 伪代码
- 传统流程图
- 结构化流程图
- PAD图

### 第六节：基本数据类型


在C语言中，基本数据类型是用于声明变量的内置类型，它们直接对应于计算机内存中的存储单元。每种基本数据类型都有其特定的用途和范围。以下是C语言中常见的基本数据类型：

#### 基本类型

- **短型（short）**
  - 用于存储较小的整数。
  - 通常占用2个字节。
  - 有符号(signed),占16位数,数的表示范围：-32768~32767
  - 无符号(unsigned),占16位数，数的表示范围：0~65535

- **整型（int）**
  - 用于存储标准整数。
  - 通常占用4个字节。
  - 有符号
  - 有符号(signed),占16位数,数的表示范围：-32768~32767
  - 无符号(unsigned),占16位数，数的表示范围：0~65535

- **长整型（long）**
  - 用于存储较大的整数。
  - 通常占用4个字节（在32位系统中）或8个字节（在64位系统中）。
  - 有符号(signed),占32位数，数的表示范围：-2147483648~2147483647
  - 无符号(unsigned),占32位数，数的表示范围：0~4294967295

- **单精度型（float）**
  - 用于存储单精度浮点数。
  - 通常占用4个字节。
  - 有符号，占32位数，数的表示范围：3.4e-38~3.4e38

- **双精度型（double）**
  - 用于存储双精度浮点数。
  - 通常占用8个字节。
  - 有符号，占64位数，数的表示范围：1.7e-308~1.7e308

- **字符类型（char）**
  - 用于存储单个字符。
  - 通常占用1个字节。
  - 有符号，占8位数，数的表示范围：-128~127
  - 无符号(unsigned char)，占8位数，数的表示范围：0~255

#### 构造类型

- **数组**
  - 用于存储固定大小的相同类型元素的集合。

- **结构体（struct）**
  - 用于将不同类型的数据组合成一个单一的复合类型。

- **共用体（union）**
  - 用于存储不同类型的数据，但所有数据共享同一块内存空间。

- **枚举类型（enum）**
  - 用于定义一组命名的整型常量。

#### 指针类型

#### 空类型（void）
  - 表示没有返回值或无类型。

#### 定义类型（typedef）
  - 用于为已存在的数据类型创建一个新的别名。


### 第七节：常量和变量

#### 1. 常量

- **定义**：程序运行时其值不能改变的量（即常数）。

- **分类**：

   - **符号常量**：用标识符代表常量。
     - **定义格式**：`#define 符号常量 常量`（不是语句，不用";"）。
     - **示例**：
       ```c
       #define Pi 3.141
       ```

   - **直接常量**：
     - **整型常量**（整常数），三种形式：
       - 十进制整数：由数字0~9和正负号表示。
       - 八进制整数：由数字0开头。
       - 十六进制整数：由0x开头。
     - **实型常量**（实数或浮点数），小数，表示形式：
       - 十进制小数形式：例如 `0.2`。
       - 指数形式：例如 `1.2e-3`。
     - **字符常量**：
       - 定义：用单引号括起来的单个普通字符或转义字符。
       - 常规字符：例如：`'A'`、`'2'`、`'#'`等。
       - 转义字符：由一个反斜杠 `\` 后跟规定字符构成。
       - 转义字符表：

         | 转义字符 | 含义 |
         |:--------:|:--------:|
         | \n    | 换行 |
         | \t    | 水平制表 |
         | \v    | 垂直制表 |
         | \b    | 退格 |
         | \r    | 回车 |
         | \f    | 换页 |
         | \a    | 响铃 |
         | \\\    | 反斜线 |
         | \‘    | 单引号 |
         | \“    | 双引号 |
         | \ddd  | 3位8进制数代表的字符 |
         | \xhh  | 2位16进制数代表的字符 |

     - **注意**：
       - 字符常量可以参加运算，例如：`'a'+1`（字符 `'a'` 的ASCII码值加1）。
       - `'a'<'b'` 实际是比较两个字符的ASCII码值。

   - **字符串常量**：
     - 定义：用双引号括起来的字符序列。
     - 示例：`"Hello, World!"`。
     - 字符串常量实际上是一个字符数组，以空字符 `'\0'` 结尾，用于表示字符串的结束。
     - 字符串可以进行连接操作，例如：`"Hello, " "World!"` 等同于 `"Hello, World!"`。

#### 2. 变量

- **定义**：在程序运行过程中其值可以改变的量。

- **使用**：在程序中声明变量时，必须指定其类型，例如 `int a;` 声明了一个整型变量 `a`。

- **变量的初始化**：
   - 变量可以在声明时直接初始化，例如 `int b = 10;`。
   - 也可以在声明后单独赋值，例如 `b = 20;`。

- **变量的作用域**：
   - 局部变量：在函数或代码块内部声明的变量，其作用域限定在该函数或代码块内。
   - 全局变量：在函数外部声明的变量，其作用域为整个程序。

- **变量的存储类别**：
   - 自动存储类（auto）：局部变量默认的存储类别。
   - 静态存储类（static）：在程序执行期间一直存在的变量。
   - 寄存器存储类（register）：建议编译器尽可能将变量存储在CPU寄存器中。
   - 外部存储类（extern）：用于声明在其他文件中定义的全局变量。


---
