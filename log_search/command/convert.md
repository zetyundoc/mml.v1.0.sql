#转换

##eval

**描述**

评估表达式并将生成的值放入字段中。

**语法**

eval &lt;eval-field&gt;=&lt;eval-expression&gt; {,&lt;eval-field&gt;=&lt;eval-expression&gt;}

**参数说明**

&lt;eval-field&gt;

&emsp描述：生成的值的目标字段名称。如果字段名称已经存在于事件中,eval 将覆盖该值。

&emsp语法：&lt;string&gt;

&lt;eval-expression&gt;

&emsp描述：算数表达式

&emsp语法：&lt;expression&gt;

**示例**

1. 静态值

    eval path as aaa
    
2. 表达式

    eval "doc['index_name'].value" as test
