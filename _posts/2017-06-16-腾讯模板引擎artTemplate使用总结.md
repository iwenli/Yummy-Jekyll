---
layout: post
title: 腾讯模板引擎artTemplate使用总结
category: 技术
tags: [模板引擎,artTemplate]
---

2017-06-16

作者：iwenli

GitHub：[https://github.com/iwenli](https://github.com/iwenli)

## 0x1.前页

模板引擎之artTemplate使用总结

GitHub: https://aui.github.io/art-template/

文档：https://aui.github.io/art-template/docs/

## 0x2.引入
cdn:
`<script type="text/javascript" src="//cdn.txooo.com/public/aui.artTemplate/artTemplate.js"></script>`

## 0x3.定义模板
```
<script type="text/html" id="t-mchResultProduct">
    {{each Products}}
    <li class="shop-item-ctn">
        <a class="shop-item-link" href="/shop.html?id={{$value.Id}}&source=shop">
            <img class="li_img  p-lazy" alt="{{$value.ProductName}}" data-original="{{$value.ProductImgs | productImgs}}"
                 src="">
            <div class="shop-item-price">
                <em>￥</em>{{$value.Price | priceToFixed}}
            </div>
        </a>
    </li>
    {{/each}}
</script>
<script type="text/html" id="t-mchResult">
    {{each list}}
    <li class="list-item">
        <div class="list_item clearfix shop-info-header">
            <div class="shop-logo-img-wrapper">
                <img class="shop-logo-img p-lazy" alt="{{$value.ComName}} logo" data-original="{{$value.MchLogo | productImgs}}" src="">
            </div>
            <div class="shop-title">
                <label>{{$value.ComName}}</label>
            </div>
            <div class="shop-sales-info">
                <span>销量<span class="num">{{$value.ProductSalesTotalCount}}</span></span>
                <span class="prodect-count">共 <span class="num">{{$value.ProductTotalCount}}</span> 件宝贝</span>
            </div>
            <span data-id="{{$value.Id}}" class="button button-fill j-gostore">进店逛逛</span>
        </div>
        <ul class="shop-item-list-wrapper clearfix">
            <!--引入子模板-->
             {{if $value.data != null}}
                 {{include 't-mchResultProduct' $value}}
             {{/if}}
        </ul>
    </li>
    {{/each}}
</script>
```
## 0x4.自定义外部函数

+ 定义：
```
template.helper('productImgs', function (data) {
    var array = data.split(',');
    return array.length > 0 ? array[0] : '/Skin/SalesV2/Img/nologo.png';
});
```
+ 用法：
`{{$value.MchLogo | productImgs}}` 或 `{{productImgs($value.MchLogo)}}`

## 0x5.填充数据渲染 
```
var html = template('t-mchResult', { list: obj.Models });
$(_this).find('.j-mch-result').append(html);
```

<!--more-->

## 0x8.尾言 小结

`原创`