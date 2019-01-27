# 项目初衷

实现pdf在线预览功能，此项目提供了三种预览方式：

1. pdf下载方式，好资源建议下载，如果有pdf预览插件则可以直接预览，但文件较大时则建议下载到本地阅读。
2. PDF.js，支持大文件分片加载，可能需要等待一会儿才能加载出第一页，但不用等到下载完成，缺点是暂时没有书签。
3. pdfobject.js，会提示下载进度，效果还算可以，优点是有书签，缺点是需要下载完整pdf，文件较大时等待时间较长。

# 适用场景

对于精品电子书，一定要下载珍藏！
如果系统会生成大量的pdf文件，或者doc文件，用户不愿意下载保存，只想要在线预览，则适合这种场景。

用户需求：浏览器在线预览文档，不想下载保存。

1. 浏览器预览插件方式，不可靠，用户浏览器各种各样，很多浏览器是弹出下载框，违背了用户不想下载的需求。
2. pdf文件较小，使用js加载也不会太慢，用户可以等待几秒。
3. doc文件预览之前需要转换为pdf或html（也许有js可以直接预览但我还不知道），可以选择每次预览都转html，也可以提前转pdf长期保存。

DOC转换接口：http://api.xlongwei.com/doku.php?id=api:doc

PDF大文件预览效果：https://pdf.xlongwei.com/pdfjs.html#中国青少年科学探索百科全书.pdf