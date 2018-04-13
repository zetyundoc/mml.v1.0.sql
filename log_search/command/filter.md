#过滤

##Filter 
**
别名**

where

**描述**

根据条件过滤索引内容。

**语法**

filter &lt;bool-expr&gt;

**参数说明**

&lt;bool-expr&gt;

* 描述：逻辑表达式

* 语法：

    &lt;bool-expr&gt;::=  &lt;field&gt;&gt;|&lt;|==|!=|&lt;&gt;|in &lt;expression&gt; 
			|(&lt;bool-expr&gt;)
			| NOT &lt;bool-expr&gt;
			| &lt;bool-expr&gt; AND|OR &lt;bool-expr&gt;

				
**示例**

| filter host="x-shcs"