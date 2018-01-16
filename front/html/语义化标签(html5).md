<h3>分为三部分：节元素标签、文本元素标签、分组元素标签</h3>
<p>header元素代表"网页"或"section"的页眉，包含（h1~h6,hgroup），没有个数限制;</p>
<p>footer元素代表"网页"或"section"的页脚，没有个数限制，除了包裹内容不一样，其他跟header类似</p>
<p>hgroup元素代表标题，当元素有多个层级时，可以将多个h元素放在其内，如文章的标题和副标题
<p>nav代表导航链接区域，用于主要导航部分</p>
<p>section元素代表文档中的"节"或"段"，指的是一篇文章的主题分段</p>
<p>article、aside、nav可以理解为特殊的section，能用这些的就不用section</p>
<p>article目的是为了让开发者独立开发或重用</p>
<p>address：代表区块容器，必须是作为联系信息出现，邮编地址、邮件地址等，一般出现在footer</p>
<br />
<p>自身独立的情况下：用article</p>
<p>相关内容：用section</p>
<p>没有语义：用div</p>