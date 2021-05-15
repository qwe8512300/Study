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
      - 常用属性：`console.log(document.head);`、`document.getElementById("对象ID");`。
   
4. 事件
   1. 基本概念：
      1. 事件：
         - 触发-响应机制
         - 用户和浏览器之间的交互行为，比如：点击按钮，鼠标进入/离开
      2. 事件三要素：
         - 事件源：触发事件的元素（标签）
         - 事件名称：click 点击事件
         - 事件的处理程序：事件触发后要执行的代码
   2. 使用方式：
      1. 定义一些函数，在触发时调用相关代码。
      2. 比如：
         - `window.onload=function(){console.log('这是一个默认加载事件');}`。
         - `document.getElementById('btn').onclick=function(){console.log('这是一个按钮点击事件。');}`。
   
5. 文档加载过程

6. 文档页面元素获取
   1. 根据ID获取元素
      - `document.getElementById('btn')`
      - ID具有唯一性，同一个ID只能有一个元素可以使用
   2. 根据标签名称获取元素
      - `document.getElementByTagName('btn')`
      - 因为TagName不具备唯一性，所以通过TagName会获取到所有使用该TagName的元素集。
   3. 根据name获取元素
      - `document.getElementByName('btn')`
      - 因为name不具备唯一性，所以通过name会获取到所有使用该name的元素集。
   4. 根据类名获取元素
      - `document.getElementByClassName('btn')`
      - 因为class不具备唯一性，所以通过class会获取到所有使用该class的元素集。
   5. 根据选择器获取元素
      - 选择器有两种方式进行获取。一种只会返回第一个，另一种会返回元素集
      - 第一种：`document.querySelector('btn')`返回第一个元素。
      - 第二种：`document.querySelectorAll`返回元素集。
   
7. 节点之间得关系

   1. 父子节点（上下级关系）

      - 获取父节点：`document.getElementById('btn').parentNode;`
      - 获取子节点：`document.getElementById('btn').chrildNode;`

   2. 兄弟节点（同级关系）

      - 获取下一个兄弟节点：

        ```javascript
        //获取下一个兄弟节点
        document.getElementById('btn').nextElementSibling;
        //获取下一个兄弟节点元素
        document.getElementById('btn').nextSibling;
        ```

      - 获取上一个兄弟节点：

        ```javascript
        //获取下一个兄弟节点
        document.getElementById('btn').previousElementSibling;
        //获取下一个兄弟节点元素
        document.getElementById('btn').previousSibling;
        ```

   3. 获取第一个/最后一个节点

      - 获取第一个子节点：

        ```javascript
        //获取第一个子节点
        document.getElementById('btn').firstElementChild;
        //获取第一个子节点元素
        document.getElementById('btn').firstChild;
        ```

      - 获取最后一个子节点：

        ```javascript
        //获取最后一个子节点
        document.getElementById('btn').lastElementChild;
        //获取最后一个子节点元素
        document.getElementById('btn').lastChild;
        ```

      - 获取所有子节点：

        ```
        //获取所有节点
        document.getElementById('btn').childNodes;
        //获取所有节点元素
        document.getElementById('btn').children;
        ```

   4. 获取所有节点

      1. NodeType：
         - 每个节点都有一个nodeType属性，用于表明节点的类型，节点类型有Node类型种定义的12个常量表示
         - 图示：![image-20210515150912666](D:\Work\新建文件夹\Study\Image\JavaScript特效\image-20210515150912666.png)

   5. 获取任意节点

8. 节点操作

9. 编码

10. 九宫格布局

11. date

12. 定时器

## BOM