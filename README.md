# C++那些事

### 0.项目概要

学习C++内容，包括理论、源码、实践、课程代码、项目等。

### 1.基础部分

- [const那些事](./basic_content/const)
- [static那些事](./basic_content/static)
- [this那些事](./basic_content/this)
- [inline那些事](./basic_content/inline)
- [sizeof那些事](./basic_content/sizeof)
- [函数指针那些事](./basic_content/func_pointer)
- [纯虚函数和抽象类那些事](./basic_content/abstract)
- [vptr_vtable那些事](./basic_content/vptr_vtable)
- [virtual那些事](./basic_content/virtual)
- [volatile那些事](./basic_content/volatile)
- [assert那些事](./basic_content/assert)
- [位域那些事](./basic_content/bit)
- [extern那些事](./basic_content/extern)
- [struct那些事](./basic_content/struct)
- [struct与class那些事](./basic_content/struct_class)
- [union那些事](./basic_content/union)
- [c实现c++多态那些事](./basic_content/c_poly)
- [explicit那些事](./basic_content/explicit)
- [friend那些事](./basic_content/friend)
- [using那些事](./basic_content/using)
- [::那些事](./basic_content/::)
- [enum那些事](./basic_content/enum)
- [decltype那些事](./basic_content/decltype)
- [引用与指针那些事](./basic_content/pointer_refer)
- [宏那些事](./basic_content/macro)

---


### 2.进阶部分 

#### 2.1 [effective_c++](./effective_c++)

正在更新...

#### 2.2 [C++2.0新特性](./c++2.0/)

- [Variadic Templates](./c++2.0/variadic)

- Spaces in Template Expressions

  ```cpp
  vector<list<int> > //ok in each C++ version
  vector<list<int>> // before c++ 11 error error: ‘>>’ should be ‘> >’ within a nested template argument list,c++11后可以正常通过
  ```

- [nullptr and nullptr_t](./c++2.0/nullptr.cpp)

- [Automatic Type Deduction with auto](./c++2.0/auto.cpp)

- [Uniform Initialization ](./c++2.0/uniform_initialization.cpp)

- [initializer_list](./c++2.0/initializer.cpp)

- [explicit for ctors taking more than one argument](./c++2.0/explicit.cpp)

- [range-based for statement](./c++2.0/auto.cpp)

  ```cpp
  for(decl:col) {
      statement
  }
  ```

- [=default,=delete](./c++2.0/default_delete.cpp)

  如果你自行定义了一个ctor,那么编译器就不会给你一个default ctor
  如果强制加上=default,就可以重新获得并使用default ctor.

- Alias(化名)Template(template typedef)

  - [alias.cpp](./c++2.0/alias.cpp) 
  - [template_template.cpp](./c++2.0/template_template.cpp)

- [template template parameter](./c++2.0/template_template.cpp)

- [type alias](./c++2.0/type_alias.cpp)

- [noexcept](./c++2.0/noexcept.cpp)

- [override](./c++2.0/override.cpp)

- [final](./c++2.0/final.cpp)

- [decltype](./c++2.0/decltype.cpp)

- [lambda](./c++2.0/lambda.cpp)

- [Rvalue reference](./c++2.0/rvalue.cpp)

- [move aware class](./c++2.0/move.cpp)

- 容器-结构与分类

  - (1) 序列式容器包括：array(C++2.0新引入),vector,deque,list,forward_list(C++2.0新引入)
  - (2) 关联式容器包括：set/multiset,map/multimap
  - (3) 无序容器(C++2.0新引入,更换原先hash_xxx为unordered_xxx)包括：unordered_map/unordered_multimap,unordered_set/unordered_multiset

- [Hash Function](./c++2.0/hash.cpp)

- [tuple](./c++2.0/tuple.cpp)

  学习资料：https://www.bilibili.com/video/av51863195?from=search&seid=3610634846288253061

#### 2.3 [C++并发编程v1](./c++2.0/./concurrency_v1)

- [第一章](./c++2.0/./concurrency_v1/chapter1)
- [第二章](./c++2.0/./concurrency_v1/chapter2)

学习资料：https://chenxiaowei.gitbook.io/cpp_concurrency_in_action/

#### 2.4 [STL源码剖析](./stl_src)

**stl源码剖析：gcc4.9.1**

- [array](./stl_src/array.md)
- [deque](./stl_src/deque.md)
- [queue and stack](./stl_src/queue_stack.md)
- [list](./stl_src/list.md)
- [vector](./stl_src/vector.md)
- [typename](./stl_src/typename.md)
- [traits](./stl_src/traits.md)
- [iterator](./stl_src/iterator.md)
- [谈谈STL设计之EBO优化](./stl_src/谈谈STL设计之EBO优化.md)
- [rb_tree](./stl_src/rb_tree.md)
- [set and multiset](set_multiset.md)
- [map and multimap](./stl_src/map_multimap.md)
- [hashtable](./stl_src/hashtable.md)
- [myhashtable](./stl_src/myhashtable.md)
- [unordered_map](./stl_src/unordered_map.md)

## 3.多线程与多进程

### 3.1 Threading In C++

- [介绍](./Threading_In_CPlusPlus/1.thread)
- [创建线程的五种类型](./Threading_In_CPlusPlus/2.create_type)
- [Join与Detachs](./Threading_In_CPlusPlus/3.join_detach)
- [mutex in C++ Threading](./Threading_In_CPlusPlus/4.mutex)

> 学习自：
>
> https://www.youtube.com/watch?v=eZ8yKZo-PGw&list=PLk6CEY9XxSIAeK-EAh3hB4fgNvYkYmghp&index=4

### 4.学习课程

#### 4.1 [极客时间《现代C++实战30讲》](https://time.geekbang.org/channel/home)

- [堆、栈、RAII：C++里该如何管理资源？](./modern_C++_30/RAII)
  - [堆](./modern_++_30/RAII/heap.cpp)
  - [栈](./modern_C++_30/RAII/stack.cpp)
  - [RAII](./modern_C++_30/RAII/RAII.cpp)
- [自己动手，实现C++的智能指针](./modern_C++_30/smart_ptr)
  - [auto_ptr、scope_ptr](./modern_C++_30/smart_ptr/auto_scope.cpp)
  - [unique_ptr](./modern_C++_30/smart_ptr/unique_ptr.cpp)
  - [shared_ptr](./modern_C++_30/smart_ptr/shared_ptr.cpp)
- [右值和移动究竟解决了什么问题？](./modern_C++_30/reference)
  - [左值与右值](./modern_C++_30/reference/reference.cpp)
  - [延长声明周期](./modern_C++_30/reference/lifetime.cpp)
  - [引用折叠](./modern_C++_30/reference/collapses.cpp)
  - [完美转发](./modern_C++_30/reference/forward.cpp)
  - [不要返回本地变量的引用](./modern_C++_30/reference/don'treturnReference.cpp)
- [容器1](./modern_C++_30/container1)
- [容器2](./modern_C++_30/container2)
- [异常](./modern_C++_30/exception)
- [字面量、静态断言和成员函数说明符](./modern_C++_30/literalAssert)
- [是不是应该返回对象？](./modern_C++_30/returnObj)
- [编译期多态：泛型编程和模板入门](./modern_C++_30/compilerpoly)
- [译期能做些什么？一个完整的计算世界](./modern_C++_30/compilercompute)
- [SFINAE：不是错误的替换失败是怎么回事?](./modern_C++_30/SFINAE)
- [constexpr：一个常态的世界](./modern_C++_30/constexpr)
- [函数对象和lambda：进入函数式编程](./modern_C++_30/functionLambda)

### 5.拓展部分

#### 5.1 [C++惯用法](./codingStyleIdioms)

##### 你最喜欢的c++编程风格惯用法是什么?

- [1.类初始化列表](./codingStyleIdioms/1_classInitializers)
- [2.枚举类替换命名空间](./codingStyleIdioms/2_enumclass_namespace)
- [3.RAII(资源获取即初始化)](./codingStyleIdioms/3_RAII)
- [4.copy and swap](./codingStyleIdioms/4_copy-swap)
- [5.pImpl(指针指向具体实现)](./codingStyleIdioms/5_pImpl)

#### 5.2 一些问题

- [C++中如何将string类型转换为int类型？](./basic_content/extent/string_int.md)

### 6.工具篇

- [容器快捷输出工具](./tool/output)

  对吴老师的代码进行了修改，[点击此处直通代码](./tool/output/output_container.h)

  输入：

  ```cpp
  map<int, int> mp{
              {1, 1},
              {2, 4},
              {3, 9}};
      cout << mp << endl;
  ```

  输出结果显示：

  ```cpp
  { 1 => 1, 2 => 4, 3 => 9 }
  ```

- 像Python一样简单输出
  
  - [像Python一样玩C/C++](./tool/像Python一样玩CC++.md)
  
- 观察编译过程变化
  
  -  [https://cppinsights.io](https://cppinsights.io/)

### 7.代码运行

- **代码环境**

  Ubuntu 18.04

- **工具**

  CLion  gcc/g++

### 8.关于作者

个人公众号：

![](./img/wechat.jpg)

