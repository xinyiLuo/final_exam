### 全球国家幸福感研究
[pythonanywhere]:http://luoxinyi.pythonanywhere.com/

#### url个数：6个
* [首页](http://luoxinyi.pythonanywhere.com/)
* [rank](http://luoxinyi.pythonanywhere.com/rank)
* [score](http://luoxinyi.pythonanywhere.com/score)
* [difference](http://luoxinyi.pythonanywhere.com/difference)
* [GDP](http://luoxinyi.pythonanywhere.com/GDP)
* [selection](http://luoxinyi.pythonanywhere.com/selection)

#### 数据传递描述：
* 创建一个happiness的数据库，创建item表，为下拉框引入参数，再创建rank、score、difference、GDP的表，导入相应的.csv数据文件

#### HTML档描述：
* base.html:首页面，bootstrap导航栏可选择score、rank、difference、GDP
* result.html：表格 下拉框
* selection.html：跳转界面
* difference.html：2015年-2017年世界幸福分数差值
* GDP.html：2015年-2017年世界GDP与前十的幸福排名
* rank.html：2015-2017年世界幸福指数
* score.html：2015-2017年世界幸福分数

#### Web App动作描述：
1. 首页路由连接数据库，建立游标，查询到对应数据，返回results页面
2. 表单选择路由，获取表单传过来的the_selected的参数，连接数据库，建立游标，执行数据查询语句。条件判断参数类型，根据类型绘制相应的图表。
3. 页面路由，连接数据库，建立游标，执行查询语句，根据结果绘制图表
