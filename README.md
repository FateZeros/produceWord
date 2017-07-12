## produceWord
java 

## freemarker
  由于POI和ITEXT在处理复杂word文档格式欠缺，并且需要在Word制定位置插入图片的时。
  发现freemarker可以通过设定word模版，经过处理生成ftl文件后，可直接通过freemarker的工具jar包可以生成制定位置的Word文件。
  
## 基本流程
word模版 -> 2003word-xml -> xml -> freemarker生成word文档。

删除：xml中<w:binData w:name="wordml://02000003.jpg" xml:space="preserve"></w:binData>内容

## 启动地址
http://localhost:5010/newProject/

[Freemarker生成Word1](http://blog.csdn.net/jackfrued/article/details/39449021)</br>
[Freemarker生成Word2](http://ylcodes01.blog.51cto.com/5607366/1842693)</br>
[Servlet3.0](http://blog.csdn.net/zhongweijian/article/details/8279650)
[XML格式化](http://tool.oschina.net/codeformat/xml)

https://www.zhihu.com/question/22146521

https://www.zhihu.com/question/29454095
