###  HTML笔记大全 ###

元素：
1.div   基本元素，可用于装载单/多元素，也可用于做装饰，可填除href外所有参数
2.img   图片元素，用于加载图片，参数有width、height、src（图片链接）、alt（图片加载不出来时显示）、style（格式："xxx:xxx; xxx:xxx;……"）、srcset（可设多个不同分辨率图片，浏览器自行决定展示，格式："xxx.jpg [原始宽度]w"）
            也可结合<a>标签使用
          例：
            <a href = "https://example.com/"
                  <img src = "xxx.jpg" />
            </a
3.a    锚点链接,用于跳转，参数有href（链接内容）、target（跳转方式:_self[当前标签页]、_blank[新标签页]、_top[整个浏览器打开（* - *）我怎么知道是什么东西，根本不用好吧]）、mailto（结合href，格式：“href = 'malito:xxx@xxx.com' ”）、
      tel（拨打电话，结合href，格式：" href = 'tel:+8613650852241' "，仅可拨打电话的移动设备）
4.html 根元素，参数有lang（国家、地区代码，如"zh-cn"、"en-us"）、xmlns（只有xhtml需要，你别管），标准HTML中该元素内仅能包含两个直接子元素head和body（乱写的就别看了）
5.title 设置网页标题，无参数
6.meta    网页元数据元素，参数有charset（标准HTML中需作为<head>的第一个子元素，一般填"UTF-8"）、（property="og:title" content="[搜索引擎搜到的标题]"      就是这么用的）、（name="description" content="[简介]"    也就是这么用的）、
                   （name="keywords" content="[关键词]"  就是这么用的…）、（name="robots" content="index,follow"  允许搜索引擎爬虫）、（name="author" content="Starwave"    作者）、（property="og:type" content="website" 类型，文章则填article）、
               （http-equiv="Content-Security-Policy" content="default-src 'self'" 只允许同源资源）、（http-equiv="X-UA-Compatible" content="IE=edge"  使用最新渲染引擎）、（name="viewport" content="width=device-width, initial-scale=1.0"  优化移动设
                      备浏览体验）
            <script type="application/ld+json"
                  {
                    "@type": "Website",
                    "headline": "[搜索引擎上展示的网站名]",
                    "author": {
                      "@type": "Person",
                      "name": "Starwave"
                    }
                  }
            </script (和meta差不多，但有利于搜索引擎理解网页)
7.h1~h6 文字元素，参数有style（用法一样）
8.p文字段落元素，参数有style、lang（优先级高过<html>中的lang）
9.strong<b  文字元素，通常以粗体显示，某个入机的讲述人会将<strong>中的文字语气增强
10.i    文字元素，表示专业术语、外语
11.u    文字元素，下划线
12.s    文字元素，删除线
13.mark    标记、高亮
14.small    小字
15.code    代码元素，内嵌代码
16.pre    保留换行、空格
17.samp    程序元素，输出
18.ul   无序列表（没有顺序标记，列表项前会有一个"・"），可在css或style参数中设置list-style-type的值，有disc(实心圆)、circle(空心圆)、square(方形)、none(无符号)
19.ol    有序列表，可填参数有type，参数值可以为：1（数字），A（大写字母），a（小写字母），I（大写罗马数字），i（小写罗马数字）
20.nav    示例：
            <nav
                  <ul
                        <li<a href = "#section1" 第一部分</a </li
                  </ul
            </nav
            <div id = "section1" </div
21.video …… controls 、audio …… controls     视频、音频元素，参数有src
22.iframe    嵌入网页，参数有src、width、height
23.form    表单容器，参数一般为action="/submit" method="POST"
24.input    输入元素,形式有：
            <input type="text"                 <!-- 文本框 -->
            <input type="password"       <!-- 密码框 -->
            <input type="number"         <!-- 数字输入 -->
            <input type="checkbox"      <!-- 复选框 -->
            <input type="radio"             <!-- 单选按钮 -->
            <input type="file"                 <!-- 文件上传 -->
            <input type="submit"           <!-- 提交按钮 -->
25.select & option    选择框，用法：
            <select>
                  <option value="1">选项1</option>
                  <option value="2">选项2</option>
            </select>
      其中，value可对接Javascript
26.label    表单标签，关联输入控件，较普通标签更有可用性
27.tabel    表格容器
28.tr    表格行
29.th    表头单元格（仅供表头使用）
30.td    表格数据单元格（仅供内容使用）
31.thead    表头区域
32.tbody    表体区域
33.tfoot    表脚区域
34.caption    表格标题
35.header    网站头部（与head区分开）
36.footer    网站底部
37.main    网站主体
38.article    独立文段
39.section    章节
40.aside    侧边栏
41.span    文字段（少量文字），与div基本一致
42.details    折叠栏，搭配summary和div使用，内部可以放其他元素
43.summary    折叠时显示的标题
44.dialog    弹出交互组件框，使用h2元素设置标题，p元素设置内容，button设置关闭
45.style    内嵌css代码，单元素行数尽量不超200行
46.script    内嵌Javascript代码，也可用于外部导入，格式：<script src = [文件地址]》</script》      可以添加async参数（无值），异步加载脚本，建议只对不重要脚本使用
47.link    导入CSS、网页图标，或预加载资源，参数有rel（类型，CSS填stylesheet，图表填icon，字体填preload）、as（给字体使用）、href（文件地址）
