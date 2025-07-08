###  HTML笔记大全 ###

元素：
1.<div>   基本元素，可用于装载单/多元素，也可用于做装饰，可填除href外所有参数
2.<img>   图片元素，用于加载图片，参数有width、height、src（图片链接）、alt（图片加载不出来时显示）、style（格式："xxx:xxx; xxx:xxx;……"）、srcset（可设多个不同分辨率图片，浏览器自行决定展示，格式："xxx.jpg [原始宽度]w"）
            也可结合<a>标签使用
	    例：
		<a href = "https://example.com/">
			<img src = "xxx.jpg" />
		</a>
3.<a>    锚点链接,用于跳转，参数有href（链接内容）、target（跳转方式:_self[当前标签页]、_blank[新标签页]、_top[整个浏览器打开（* - *）我怎么知道是什么东西，根本不用好吧]）、mailto（结合href，格式：“href = 'malito:xxx@xxx.com' ”）、
	tel（拨打电话，结合href，格式：" href = 'tel:+8613650852241' "，仅可拨打电话的移动设备）
4.<html> 根元素，参数有lang（国家、地区代码，如"zh-cn"、"en-us"）、xmlns（只有xhtml需要，你别管），标准HTML中该元素内仅能包含两个直接子元素head和body（乱写的就别看了）
5.<title> 设置网页标题，无参数
6.<meta>    网页元数据元素，参数有charset（标准HTML中需作为<head>的第一个子元素，一般填"UTF-8"）、（property="og:title" content="[搜索引擎搜到的标题]"      就是这么用的）、（name="description" content="[简介]"    也就是这么用的）、
                   （name="keywords" content="[关键词]"  就是这么用的…）、（name="robots" content="index,follow"  允许搜索引擎爬虫）、（name="author" content="Starwave"    作者）、（property="og:type" content="website" 类型，文章则填article）、
		   （http-equiv="Content-Security-Policy" content="default-src 'self'" 只允许同源资源）、（http-equiv="X-UA-Compatible" content="IE=edge"  使用最新渲染引擎）、（name="viewport" content="width=device-width, initial-scale=1.0"  优化移动设
                      备浏览体验）
		<script type="application/ld+json">
			{
			  "@type": "Website",
			  "headline": "[搜索引擎上展示的网站名]",
			  "author": {
			    "@type": "Person",
			    "name": "Starwave"
			  }
			}
		</script> (和meta差不多，但有利于搜索引擎理解网页)
7.<h1>~<h6> 文字元素，参数有style（用法一样）
8.<p>文字段落元素，参数有style、lang（优先级高过<html>中的lang）
9.<strong><b>  文字元素，通常以粗体显示，某个入机的讲述人会将<strong>中的文字语气增强
10.<i>    文字元素，表示专业术语、外语
11.<u>    文字元素，下划线
12.<s>    文字元素，删除线
13.<mark>    标记、高亮
14.<small>    小字
15.<code>    代码元素，内嵌代码
16.<pre>    保留换行、空格
17.<samp>    程序元素，输出
18.<ul>
