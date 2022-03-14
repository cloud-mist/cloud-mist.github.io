---
layout: post
title:  "Jekyll的Data File"
date:   2022-03-14 12:00:52 +0800
categories: jekyll
---


## Data File 是干嘛的
从`_data` 文件夹下的`YAML`,`JSON`，`CSV`载入数据,主要是为了方便大量数据的复用。[^1]

## 简单实践

### 1.有个数据文件
假设有一个这样的csv文件（截取的**片段**）,在`_data`文件夹下

```
asciiCode,symbol
40,(
41,)
42,*
43,+
44,","
45,-
46,.
47,/
48,0
49,1
```

### 2.运用
我们就可以在写blog时，通过`site.data.test` 访问

#### code

<img src="/assets/jekdatafile1.png" width="70%" />

#### 结果
{% include jekdatafile-c1.txt %}

## 参考
[^1]: http://jekyllcn.com/docs/datafiles/
