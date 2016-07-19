# frontend
全真电影院数据库项目の前端静态页面

`master`分支已**重新启用**，请不要浏览`gh-pages`分支。
静态页面暂时部署于[Azure](https://quanzhencinema.github.io/frontend/)查看DEMO，在登录页右下角点击`经理页面`直接跳转到经理后台页面。

##主要更新
> 详细更新看commit记录就好了

+ July 18 上线了开发人员，用户首页，影片描述页，将静态库部署到Azure上
+ July 17 重新启用了`master`分支
+ July 16 上线了后台模板

##模块介绍
###客户界面`/`
+ 主页`/index.html`
+ 开发人员名单 `/developer.html`
+ 搜索结果页`/search.html`
+ 员工登录页`/login.html`

###经理后台`/manager`
+ 在Dashboard显示主要的功能入口以及统计数据 `pages/index.html`
+ 电影排片      `pages/movie.html`
+ 折扣管理      `pages/discount.html`
+ 会员管理      `pages/member.html`
+ 员工管理      `pages/staff.html`
+ 周边销售      `pages/snack.html`

## 文件安排（暂定）
+ 用户界面首页`.html`文件放于最外层；要是首页的文件多起来的话大概会打个包放在`/customer`里面
+ 经理后台管理页面使用了已有的后台组件，为了方便全部放在`/manager`文件夹中。其中`.html`文件全部放在`/manager/pages`下
+ 销售员的界面预计会放在`/saler`里面（还没放）
+ 出于能省就省的穷人心态全部`.html`引用的bootstrap相关文件都是最顶层的`/css`, `/js`和`/fonts`文件夹里的
+ 各种图片资源到底是分开放还是一起放并没有想好……先就全部都放在`/images`下吧

## 使用的轮子及其文档
+ 全局样式以及各种组件[bootstrap全家桶](http://www.bootcss.com/)
+ 后台模板[SB Admin 2](http://startbootstrap.com/template-overviews/sb-admin-2/)  
  这个模板似乎还自带了一大波数据可视化的库而且还挺好看的……于是可能就不用用别的库了【
+ 登录界面的输入框动画模板[Text Input Effect里面的Hoshi](http://tympanus.net/codrops/2015/01/08/inspiration-text-input-effects/)
+ 排片的时间管理模块[FullCalendar](http://fullcalendar.io/)
+ 在线选座模块[jQuery Seat Charts](https://github.com/mateuszmarkowski/jQuery-Seat-Charts)
+ 可编辑表格控件[X-editable(Bootstrap)](http://vitalets.github.io/x-editable/)