---
title: 「算法」竞赛中常用的c++黑魔法
date: 2021-05-08 14:01:02
tags: 算法
categories: 算法
katex: true
---



内容大部分查考**therainisme**的笔记本 

🔗 [这里是他的笔记本](https://notebook.therainisme.com/algorithm/%5B99%5D%E7%AB%9E%E8%B5%9B%E4%B8%AD%E5%B8%B8%E7%94%A8%E7%9A%84C++%E9%BB%91%E9%AD%94%E6%B3%95.html#%E5%8A%A8%E6%80%81%E6%95%B0%E7%BB%84-vector)

# 动态数组 vector

操作和Python的list类似

```c++
vector<int> v; // 声明

v.push_back(x); // 尾部添加一个元素
v.pop_back(); // 删除尾部元素
v.insert(v.begin()+2,2); // 在第二个元素后插入新元素
v.back(); // 取出尾部的元素
v.size(); // 返回vector的大小
v.clear(); // 清空vector
```

# 栈 stack

```c++
stack<int> s;
s.push(x); // 压入栈中元素
int n = s.top(); // 返回栈顶元素
int  = s.size(); // 返回栈的大小
s.pop(); // 弹出栈顶元素
s.empty(); // 判断栈是否为空
```

# 单向队列 queue

```c++
int x=1;
queue<int> q; // 声明

q.push(x); // 推入队列中元素
q.empty(); // 判断是否为空
q.front(); // 取出对列首部的元素
q.back(); // 取出队尾元素
q.size(); // 返回队列长度
q.pop(); // 弹出队首元素
```

# 字符串 string

```c++
string s = "aabbcc";
s.push_back('a'); // 像尾部追加一个字符
char c = s.back(); // 获取尾部的字符
char c2= s.front(); // 获取头部的字符
s.pop_back(); // 弹出尾部的字符

// 字符串翻转
reverse(s.begin(),s.end()); // 不需要重新赋值
// 排序
sort(s.begin(),s.end());
// 插入元素
s.insert(2,"ahh"); // 在第二个元素后插入
// 删除元素
s.erase(2, 3); // 从第二个元素开始删除后面的3个元素

string d = s.substr(1,3); // 从索引为1的元素开始获取3个元素
int a = s.find("aa"); // 找到返回索引，找不到返回-1
```





































