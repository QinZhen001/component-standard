# component-standard
wepy组件规范


## 分析
目前，共有以下页面

* author 作者页
* channel 频道页
* collection 收藏页
* hotRank 热门页
* index 首页
* detail 详情页


```
┣━ index 首页 ● 包括以下组件             
        ┣━ list               列表
        ┣━ banner        轮播图           
        ┣━ tab-up         上面的tabbar          
        ┣━ tab-down     下面的tabbar      
	     ┣━ refresh-button   刷新的按钮 (小挂件)
		  ┣━ reward-button   赞赏的按钮 (小挂件)
	   	┣━ webview-button    跳转webview的按钮(小挂件) 
┣━ detail 详情页  ● 包括以下组件 
               ┣━ baseScene类 音乐图文，图文，视频，祝福场景  
               ┣━ list     列表            
               ┣━ tab-down     下面的tabbar                        
┣━ hotRank 热门页 ● 包括以下组件 
         ┣━ list     列表     
         ┣━ tab-down     下面的tabbar      
┣━ collection 收藏页 ● 包括以下组件 
         ┣━ userInfo  用户信息            
         ┣━ list     列表          
         ┣━ tab-down     下面的tabbar            
┣━ channel 频道页 ● 包括以下组件 	
		 ┣━ userInfo  用户信息  
		 ┣━ list     列表     
┣━ author 作者页 ● 包括以下组件 	
        ┣━ ususerInfoer  用户信息 
	    ┣━ list     列表     
```





## 提醒

* **小挂件全部采用cover-view实现**
* 组件不用进行网络请求，数据由外部传入
* 分清楚组件内部应该处理的事件和应该传递到页面处理的事件
* list里面每一项都是一个card



## 规范

### 提交npm规范

提交npm的包应包括以下东西
```javascript
package.json  (配置文件)
README.md  (说明文档)
xxx.wpy (入口)
dist文件夹 （打包后的文件）
screenshot文件夹 （组件的截图）
```



> 具体看example文件夹



package.json 必填字段
* name （包名) **（按照包命名规范）**
* version （版本号）
* description （描述）
* main （入口文件 指向xxx.wpy）
* author (作者)

>生成package.json使用命令   **npm init**



### 包命名规范
npm包命名： **描述性词语-组件-皮肤**   (全小写字母)

例如：refresh-button-xxx
