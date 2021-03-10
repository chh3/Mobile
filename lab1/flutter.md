# Flutter调研
1813063 陈画画

Flutter 是 Google 开源、免费的 UI 工具包，帮助开发者通过一套代码库高效构建多平台精美应用，支持移动、Web、桌面和嵌入式平台。

## 编辑工具

可以使用任意文本编辑器，结合Flutter的命令行工具来开发 Flutter 应用

我们采用Android Studio，其为 Flutter 提供了一个完整的集成开发环境。

先配置Flutter的环境

安装Android Studio的版本3.0以上，然后打开Android Studio安装Flutter和Dart插件

## 开发

打开IDE时，新建Flutter项目、应用程序，并确认Flutter SDK 的路径是否正确，如果没有则需要安装。一切就绪后，会创建一个叫myapp的项目目录，里面包含一个简单示例。
可以简单地运行，选择一个安卓设备来运行，如果没有可用地安卓设备，则可以创建一个虚拟机。

编译完成后即可运行。

### 尝试热重载(hot reload)

Flutter 通过 热重载 提供快速开发周期，该功能支持应用程序在运行状态下重载代码而无需重新启动应用程序或者丢失程序运行状态。修改一下代码，然后告诉IDE或者命令行工具你需要热重载，然后看一下模拟器或者设备上应用的变化

在热重载模式和功能开启地情况下不要做性能测试。


## UI

### Widget
Flutter的核心思想是用 Widget 来构建 UI 界面。 Widget 描述了在当前的配置和状态下视图所应该呈现的样子。当 widget 的状态改变时，它会重新构建其描述（展示的 UI），框架则会对比前后变化的不同，以确定底层渲染树从一个状态转换到下一个状态所需的最小更改。

 Widget 的主要工作是实现 build方法，该方法根据其它较低级别的 widget 来描述这个 widget。框架会逐一构建这些 widget，直到最底层的描述 widget 几何形状的 RenderObject。

 #### 常用Widgets

 Text 文本

 Row, Column 基于wen的flexbox布局模型在水平和竖直方向构建灵活的布局

 Stack Stack Widget基于Web中的绝对位置布局模型，按照绘制顺序将widget堆叠到一起

 Container 可以用来创建一个可见的矩形元素







