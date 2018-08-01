# gwm.js

> Generate Watermark

用于内部系统生成水印，可提示信息安全与责任追踪。安全问题不容忽视，对于内部人员敏感操作有一定的提示作用。

### 特性
+ 支持常见的 alert、confirm、toast、notice 四种类型弹窗
+ 可选择使用 IOS 或者 Material Design 风格的弹窗
+ 可自定义按钮的文字、样式、回调函数，支持多个按钮
+ 多个弹窗状态改变回调函数
+ 同时支持 jQuery 和 Zepto 库
+ 可扩展性强

### 截图
<p align="center"><img src="https://raw.githubusercontent.com/loadchange/gwm/master/images/demo.png" width="550"></p>

## 示例
点击这里查看效果→：[Demo示例](https://loadchange.github.io/gwm/index.html)


## 使用说明
**1、引入 JS 文件**
```javascript
<script src="../js/gwm.js"></script>
```
或者使用 npm 安装
```
npm install gwm
```

**2、构建水印**
```
gwm.creation()
```

## 参数
<table>
    <thead>
        <tr>
            <th>参数</th>
            <th>默认值</th>
            <th>说明</th>
        </tr>                           
    </thead>
    <tbody>
        <tr>
            <td>txt</td>
            <td>date 内部资料 请勿外传</td>
            <td>水印文字内容</td>
        </tr>
        <tr>
            <td>width</td>
            <td>158</td>
            <td>水印画布宽度</td>
        </tr>
        <tr>
            <td>height</td>
            <td>100</td>
            <td>水印画布高度</td>
        </tr>
        <tr>
            <td>x</td>
            <td>0</td>
            <td>水印坐标x</td>
        </tr>
        <tr>
            <td>y</td>
            <td>50</td>
            <td>水印坐标y</td>
        </tr>
        <tr>
            <td>font</td>
            <td>'microsoft yahe'</td>
            <td>设置水印字体</td>
        </tr>
        <tr>
            <td>fontSize</td>
            <td>12</td>
            <td>水印字体大小</td>
        </tr>
        <tr>
            <td>color</td>
            <td>#000</td>
            <td>水印字体颜色</td>
        </tr>
        <tr>
            <td>alpha</td>
            <td>0.1</td>
            <td>水印字体透明度</td>
        </tr>
        <tr>
            <td>angle</td>
            <td>-15</td>
            <td>水印文字倾斜角度</td>
        </tr>
    </tbody>
</table>


## 方法
| 方法            | 说明  |
| :--------       | :----  |
| gwm.creation | 创建水印。 |
| gwm.observing | 手动开启观察者，当水印元素被篡改视，重新渲染水印元素。 |
| gwm.cancel | 取消观察者，水印可以被隐藏或删除。 |


## 开发环境使用方法
**1、安装**
```
npm install
```

**2、在本地运行项目**
```
npm run dev
```
打开 index.html 预览效果

**3、build 命令**
```
npm run build
```