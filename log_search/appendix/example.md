|序号	|类型	|日志检索语句|
| :--- | :--- | :--- |
|1|	普通检索|	index opm* &#124 sort  @timestamp asc|
|2|     普通检索|	index opm* &#124 sort  @timestamp desc|
|3|	全文检索|	host="x-shcs-adj-v03"|
|4|	聚合检索	|index opm* &#124 stats max(@timestamp) as Ttime by path|
|5|	聚合检索|	index opm*&#124 stats max(@timestamp) as Ttime by path|
|6|	聚合检索	|stats count() as count_log by index_name|
|7|	聚合检索|	app_apache* "xampp" &#124 sort @timestamp asc|
