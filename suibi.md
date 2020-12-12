# 随笔

## html中的3种链接

1. `link` - 链接资源，icon,css,js
1. `a` - 跳转，放置在元素上，第三方链接加rel="noopener noreferrer"  
1. `area` - 跳转，区域型链接，支持circle,rect,poly三种类型，需与 `img` 和 `map` 配合使用，

```html
<div>
  <img src="img.png" usemap="#shapes" width="200" height="200" />
  <map name="shapes">
    <area shape=circle coords="100, 100, 100" href="https://www.bilibili.com" />
    <area shape=rect coords="0,0,100,100" href="http://www.baidu.com" />
  </map>
</div>
```

## css 文档流

### vertical-align

vertical-align: top,bottom / text-top,text-bottom / middle / baseline

### BFC

主要作用，消除浮动导致的布局问题，过去通过 `overflow: auto` 解决，现在通过 `display: flow-root` 创建一个新的BFC

## 替换型元素

1. script
2. img
    * 根据屏幕尺寸，使用不同的图片 使用 `srcset`

        ```html
        // 根据屏幕宽度
        <img srcset="/png-200.png 200w, /png-400.png 400w">

        // 根据屏幕分辨率
        <img srcset="/png-2x.png 2x, /png-4x.png 4x">
        ```

    * 根据屏幕尺寸，设定不同的宽度，使用 `sizes`

        ```html
        <img src="png.png" sizes="(max-width: 600px) 200px, 50vw">
        ```

3. picture，使用source进行媒体查询
4. video，使用source进行兼容
5. audio，使用source进行兼容
6. iframe

## 动画

## 颜色

rgba,hsla,渐变

## 可访问性
