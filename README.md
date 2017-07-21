## produceWord
java 

## freemarker
  由于POI和ITEXT在处理复杂word文档格式欠缺，并且需要在Word制定位置插入图片的时。
  发现freemarker可以通过设定word模版，经过处理生成ftl文件后，可直接通过freemarker的工具jar包可以生成制定位置的Word文件。
  
## 基本流程
word模版 -> 2003word-xml -> xml -> freemarker生成word文档。

删除：
 xml中<w:binData w:name="wordml://02000003.jpg" xml:space="preserve"></w:binData>里面的内容，换成图片转换的base64字段插入。

## 启动地址
http://localhost:5010/newProject/

## 获取文件地址
 与.class 文件位于同一目录下，可以通过Class类的getResourceAsStream()方法来获得输入流
```bash
InputStream in = 类名.class.getResourceAsStream("文件名"); //适用于静态方法或实例方法 

InputStream in = this.getClass().getResourceAsStream("文件名"); //适用于实例方法 
```

[Freemarker生成Word 1](http://blog.csdn.net/jackfrued/article/details/39449021)</br>
[Freemarker生成Word 2](http://ylcodes01.blog.51cto.com/5607366/1842693)</br>
[Servlet3.0](http://blog.csdn.net/zhongweijian/article/details/8279650)
[XML格式化](http://tool.oschina.net/codeformat/xml)</br>
[java路径](http://blog.sina.com.cn/s/blog_752265d10101821c.html)


https://www.zhihu.com/question/22146521

https://www.zhihu.com/question/29454095
