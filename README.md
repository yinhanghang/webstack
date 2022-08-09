# Hugo 版 WebStack 主题
安装git,hugo,在coding创建仓库，根据仓库创建静态网站（好像空的仓库不能创建网站，建议成功上传仓库文件成功后创建网站）      

hugo.exe new site ./   
    ./ 创建在当前目录   
进入themes   
放下载到的主题 文件夹名字WebStack-Hugo  （目前下载地址：https://github.com/shenweiyan/WebStack-Hugo）  
本地使用  
    hugo.exe server --theme=WebStack-Hugo  
生成静态文件 
    hugo.exe --theme=WebStack-Hugo --baseUrl="我的coding网址"  
进入根目录public目录 （生成文件不在这个目录，找一下根目录的docs） 
    git init  
	git remote add origin coding仓库  
	git add -A  
	git commit -m "dierci"  
	git push -u origin master  
	 
	上传报错使用  
	原因：好像是本地没有readme.md文件  
	git pull --rebase origin master  





修改配置：  
    themes\WebStack-Hugo\exampleSite   
    这个文件夹是主题作者的配置相关  
    config.toml：放到网站根目录，baseURL = "自己网站"，其他要改的目前不清楚  
    data\webstack.yml
    配置网站相关当行相关，可以修改自己想要的网站     
    content\about.md   
    相关文件，可以改一改   
    docs   
    作者的静态文件，我直接删除了整个文件夹    

themes目录结构  

└─WebStack-Hugo
    ├─layouts
    │  ├─partials
    │  └─_default
    └─static
        └─assets
            ├─css
            │  └─fonts
            │      ├─elusive
            │      │  ├─css
            │      │  └─font
            │      ├─fontawesome
            │      │  ├─css
            │      │  └─fonts
            │      ├─glyphicons
            │      ├─linecons
            │      │  ├─css
            │      │  └─font
            │      └─meteocons
            │          ├─css
            │          └─font
            ├─images
            │  └─logos
            └─js

