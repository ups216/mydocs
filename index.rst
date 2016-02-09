.. _rst_mydoc2016

Visual Studio ALM的动手实验
==============================

概述
-----
    本文档库提供Visual Studio ALM的动手实验文档及相关资源。

    :撰写日期: |today|
    :作者: **徐磊**
    :主页: `DevOps Hub <http://devopshub.cn>`_

内容
-----

.. toctree::
    :titlesonly:
    
    getting-started/index
    concepts/index

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

JavaScript是非常强大的开发语言，不仅仅在客户端，也在服务器端

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
    

    