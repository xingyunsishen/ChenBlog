# ChenBlog
ChenBlog

# 开发环境
Python版本：3.5
Django版本：1.8

# 如何使用？
## 先安装环境
`pip install -r requirements.txt`
## 初始化数据库
`python manage.py makemigrations`
`python manage.py migrate`
## 创建管理员用户
`python manage.py createsuperuser`
## 配置网站
+ SITE_NAME = 'ChenBlog'  //站点名称
+ SITE_MASTER = 'woodcoding'    //博主
+ SITE_SIGNATURE = '相信爱笑的人运气不会太差！'  //签名
+ SITE_PAGINATE_NUM = 10        //分页数量
+ DUOSHUO_SHORT_NAME = 'chenblogtest'    //多说短名，（请到多说官网申请）
+ DUOSHUO_NEW_COMMENTS = True       //最新评论是否显示，默认显示
+ COLORTAG = False //彩色标签开关，默认关闭，感觉彩色和目前主题不搭如有需要自己开启, 添加css样式tag即可
+ FRIENDLINK = True     //友情链接是否显示
+ MARKDOWN = False      //是否开启MarkDown

## 启动网站
`python manage.py runserver`

# 目前具有的功能：

+ 文章发布功能(Tinymce编辑器)
+ 代码高亮（prism or pyments）
+ 文章评论（多说）
+ 分类功能
+ 标签功能
+ 导航条菜单自定义功能
+ 自定义静态页面(v0.2新增，模板文件见下方)
+ 友情链接功能
+ Markdown编辑功能

## 自定义静态页面的模板文件解释：
* 请在增加静态页面的时候URL路径前面添加‘pages’目录，例如：/pages/about/（防止出现混乱）
* 自带三个模板，blank.html(空模板)，default.html(默认模板，带工具条和导航)，navbar.html(只带导航条)

# 部分代码实现参考：
+ http://python.usyiyi.cn/django_182/index.html
+ https://github.com/djangoStudyTeam/DjangoBlog/tree/blog-tutorial
