#聚合

## Stats

**别名**

Groupby

**描述**

对索引进行聚合。

**语法**

stats &lt;aggr-function&gt;(&lt;field-name&gt;) as &lt;new-field-name&gt;  [by &lt;field-name&gt; {, &lt;field-name&gt;}]

#### 参数说明

&lt;aggr-function&gt;

描述：聚合函数支持列表，参考[聚合函数列表。](log_search/appendix/aggregation_list.md)

&lt;field-name&gt;

描述：字段名

&lt;new-field-name&gt;

描述：字段名

&lt;bool-expression&gt;

描述：逻辑表达式

**示例**

index opm*| stats min(@timestamp) as min_time by ip
index opm*|stats count(reccode) as count_a by ip |top 2 by count_a


##Top

**描述**

Top N，筛选排名前N的信息。

**语法**

top &lt;top-n&gt; &lt;aggr-function&gt;(&lt;field-name&gt;) as &lt;new-field-name&gt; by &lt;group-field-name&gt;

**示例**

index opm*|stats count(reccode) as count_a by ip |top 2 by count_a


