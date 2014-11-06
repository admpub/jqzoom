jQzoom Evolution Library - Javascript Image magnifier
==================================================

admpub改进如下：
默认情况下，大图的网址通过“a”标签中的“data-large-image”属性来取得。
可以通过在选项参数中指定“largeImageAttrName”元素值来自定义获取大图网址的属性名称。
在把“largeImageAttrName”的值设置为“href”的情况下，该“a”标签的click事件会被强制取消，
也就是链接不可点击，其它非“href”的情况下click事件不受影响，这点请注意。
可以在“a”标签的“rel”属性中按照“画廊名 + @ + 画廊缩略图包装元素.class或#id值”这种格式
来避免为了取得画廊缩略图元素搜索所有a标签，从而提高性能。

画廊缩略图“a”标签中的“rel”属性值是一个json格式的数据，支持以下元素值：
{
    gallery: 'gal1',
    smallimage: './imgProd/triumph_small1.jpg',
    largeimage: './imgProd/triumph_big1.jpg',
    title:'哈哈哈',
    url:'http://www.coscms.com'
}