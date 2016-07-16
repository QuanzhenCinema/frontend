# frontend
全真电影院数据库项目の前端静态页面

`master`分支已弃用，请浏览`gh-pages`分支。
点击本库的[Github Pages](https://quanzhencinema.github.io/frontend/)查看DEMO，在登录页右下角点击`经理页面`直接跳转到经理后台页面。

##主要更新
> 详细更新看commit记录就好了

+ July 16 上线了后台模板

## 文件安排（暂定）
+ 用户界面首页`.html`文件放于最外层；要是首页的文件多起来的话就打个包放在`/customer`里面好了。
+ 经理后台管理页面使用了已有的后台组件，为了方便全部放在`/manager`文件夹中。其中`.html`文件全部放在`/manager/pages`下。
+ 销售员的界面预计会放在`/saler`里面（还没放）
+ 出于能省就省的穷人心态全部`.html`引用的bootstrap相关文件都是最顶层的`/css`,`/js`和`/font`文件夹里的

## 使用的轮子
+ 全局样式[bootstrap](http://www.bootcss.com/)
+ 后台模板[SB Admin 2](http://startbootstrap.com/template-overviews/sb-admin-2/)
+ 登录界面的输入框动画模板[Text Input Effect里面的Hoshi](http://tympanus.net/codrops/2015/01/08/inspiration-text-input-effects/)
+ 排片的时间管理模块[FullCalendar](http://fullcalendar.io/)
+ 在线选座模块[jQuery Seat Charts](https://github.com/mateuszmarkowski/jQuery-Seat-Charts)