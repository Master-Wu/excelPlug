# excelPlug
> a plug/demo/script for excel files(.xls only) r/w; 一个读/写excel文件(仅.xls格式)的脚本/插件, 可集成到你的代码中;(目前还不行))
暂时仅支持MySQL数据库
## 要求配置:
pymysql、xlrd、xlwt的正确安装，即相关数据库以及excel文件操作库的安装
## 接收参数
({数据库连接字符串与pymysql格式近似})

## 各方法接受参数与返回值
导入数据库excel地址:
write_to_db(路径或file_contentsexcel=文件流, table名称, 数据库各字段名列表\['id','name','xxx',等 \])
return 成功数量

数据库取值导出为excel:
write_to_excel(table名, excel表头各字段命名列表\[ "id","姓名","xxx",等 \], filePath="导出文件路径", sqlWhere="你的筛选条件select xx,xxx,vgf from table名 where xxxxx")
return 如传入文件路径则返回导出数量
return 未指定路径则返回excel文件流?

暂时就这么着吧, 还代码没写完, 老子吃饭去了

将model/object导出为excel:
object_to_excel(obj, filePath="文件路径")
return excel文件流
return 指定了文件路径则仅返回1/0
