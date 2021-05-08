# 特效

## Web APIs

1. JavaScript得组成
2. BOM-浏览器对象模型
3. DOM-文档对象模型



## DOM

1. 基本概念
   - 文档对象模型(Document Object Model),是W3C组织推荐得处理可扩展标记语言得标准编程接口.它是一种与平台和语言无关得应用程序接口,它可以动态的访问程序和脚本,更新其内容、结构和文档风格.
2. DOM又称之为文档书模型
   1. <img src="D:\Work\新建文件夹\Study\Image\JavaScript特效\image-20210508194400157.png" alt="image-20210508194400157" style="zoom:50%;" />
   2. 概念
      - 文档：一个网页可以称之为文档。
      - 节点：网页中的所有内容都是节点（标签、属性、文本、注释等）。
      - 元素：网页中的标签。
      - 属性：标签的属性。
   3. DOM常用操作
      - 获取文档元素
      - 对文档元素进行增删改查操作
      - 事件操作
3. Window和document
   1. Window
      - 所有浏览器都支持window对象，它支持浏览器窗口。
      - 所有的JS全局对象，函数以及变量都能自动成为window对象的成员。
      - 全局变量是window对象的属性，全局函数是window对象的方法。
   2. document
      - document也是window对象的属性之一。
      - document对象是documentHTML的一个实例，也是window对象的一个属性，因此document对象也能作为全局对象来访问。
      - 常用属性：console.log(document.head);、document.getElementById("对象ID");。
4. 事件
5. 文档加载过程
6. 文档页面元素获取
7. 节点之间得关系
8. 节点操作
9. 编码
10. 九宫格布局
11. date
12. 定时器

## BOM