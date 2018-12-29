# excelPlug
a plug/demo/script for excel files(.xls only) r/w; 一个读/写excel文件(仅.xls格式)的脚本/插件, 可集成到你的代码中;(目前还不行))
暂时仅支持MySQL数据库
## 要求配置:
pymysql、xlrd、xlwt的正确安装，即相关数据库以及excel文件操作库的安装
## 接收参数
({数据库连接字符串与pymysql格式近似},excel地址(或file_contentsexcel=文件流,暂时没想好),table名称, {导入:\[数据库字段名\],导出:\[导出excel表头\]})
