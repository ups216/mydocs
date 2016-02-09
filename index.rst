.. _rst_mydoc2016

reST 文档格式测试
==============================

概述
-----
    本文档库提供Visual Studio ALM的动手实验文档及相关资源。

    :撰写日期: |today|
    :作者: **徐磊**
    :主页: `DevOps Hub <http://devopshub.cn>`_
    
----


内容
-----

.. toctree::
    :titlesonly:
    
    getting-started/index
    concepts/index

----

代码示例
--------

**C#代码示例**

一下是C#代码示例

.. code-block:: c#
    :linenos:

    public void Startup(){
        Console.WriteLine("Hello World!");
    }
    

**PowerShell代码示例**

一下是PowerShell代码示例，本实验文档将大量使用PowerShell来进行环境配置

.. code-block:: powershell
    :linenos:
    
    get-help *
    
**JavaScript代码示例**

JavaScript是非常强大的开发语言，不仅仅在客户端，也在服务器端。

注意以下代码的第9和11行被高亮显示！

.. code-block:: javascript
    :linenos:
    :emphasize-lines: 9,11
    
    'use strict';

    const express = require('express');

    // Constants
    const PORT = 8080;

    // App
    const app = express();
    app.get('/', function (req, res) {
    res.send('Hello world\n');
    });

    app.listen(PORT);
    console.log('Running on http://localhost:' + PORT);
    
表格示例
--------

使用reST编写表格，如下：


**GridTable 示例**


+------------------------+------------+----------+----------+
| Header row, column 1   | Header 2   | Header 3 | Header 4 |
| (header rows optional) |            |          |          |
+========================+============+==========+==========+
| body row 1, column 1   | column 2   | column 3 | column 4 |
+------------------------+------------+----------+----------+
| body row 2             | Cells may span columns.          |
+------------------------+------------+---------------------+
| body row 3             | Cells may  | - Table cells       |
+------------------------+ span rows. | - contain           |
| body row 4             |            | - body elements.    |
+------------------------+------------+---------------------+


**SimpleTable 示例**

    
=====  =====  =======
A      B      A and B
=====  =====  =======
False  False  False
True   False  False
False  True   False
True   True   True
=====  =====  =======

图片示例
--------

.. figure:: /images/github.jpg
    :width: 200
    
    图：Github Logo 图片猫
    

各种字体格式测试
---------------

测试一下等宽字体 ``git clone``

.. role:: ul
   :class: underline

:ul:`下划线` 效果

不留白的\ :ul:`下划线`\ 效果

.. role:: strike
    :class: strike
:strike:`这里是删除线` 效果


**这里是粗体** 效果，*这里是斜体* 效果

下面是列表

1. 列表可以折行
   对其则自动续行
   
   
2. 列表可以包含多个段落

   空行开始的心段落，
   新段落要和列表项内容对其
   
   
3. 列表下的代码注意对其

    ::
    
        $ printf "Hello World. \n"

多级列表

1. 数字和点是一种编号方式。

   A. 大写字母编号。

      a. 小写字母编号。
      b. 小写字母编号。

2. 继续一级列表。

   (I). 大写罗马编号。

       i). 小写罗马编号。

无序列表

* 星号、减号、加号开始列表。

  - 列表层级和缩进有关。

    + 和具体符号无关。
    + 和具体符号无关。
    + 和具体符号无关。
    
  - 列表层级和缩进有关。
  - 列表层级和缩进有关。

* 返回一级列表。

缩进

	
Python式段落缩进：

  第一级段落缩进。

    第二级段落缩进。

  返回一级段落缩进。
  
使用等宽字体作为说明框

``这些内容是需要你注意的，所以使用加框显示``

.. attention:: 如果需要了解如何快速使用本实验手册，请参考 :doc:`快速入门说明 <getting-started/index>` 这里的内容需要您仔细阅读.