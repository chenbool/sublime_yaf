# sublime_yaf

[![GitHub stars](https://img.shields.io/github/stars/chenbool/sublime_yaf)](https://github.com/chenbool/sublime_yaf/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/chenbool/sublime_yaf)](https://github.com/chenbool/sublime_yaf/network)
[![License](https://img.shields.io/github/license/chenbool/sublime_yaf)](https://github.com/chenbool/sublime_yaf/blob/master/LICENSE)

> Sublime Text 语法提示插件，支持 Yaf 框架所有类、方法、属性

## 功能特性

| 特性 | 说明 |
|------|------|
| 代码片段 | 333+ 个代码片段 |
| 完整覆盖 | 覆盖 Yaf 核心类完整 API |
| 智能提示 | 支持 Tab 键快速补全 |
| 类文档 | 包含构造函数、析构函数、魔术方法等 |

## 安装

| 工具 | 安装文档 |
|------|----------|
| Sublime Text | [sublime 安装教程](https://github.com/chenbool/sublime_thinkphp5/wiki/Sublime%E5%AE%89%E8%A3%85) |
| VS Code | [vscode 安装教程](https://github.com/chenbool/sublime_thinkphp5/wiki/vscode%E5%AE%89%E8%A3%85) |

## 代码片段总览

| 分类 | 数量 | 说明 |
|------|------|------|
| Application | 18 | Yaf\Application 核心类 |
| Dispatcher | 24 | Yaf\Dispatcher 调度类 |
| Request | 34 | Yaf\Request 请求类 |
| Response | 15 | Yaf\Response 响应类 |
| Controller | 16 | Yaf\Controller 控制器 |
| View | 28 | Yaf\View 视图类 |
| Router | 22 | Yaf\Route 路由类 |
| Loader | 13 | Yaf\Loader 自动加载 |
| Registry | 5 | Yaf\Registry 注册表 |
| Session | 20 | Yaf\Session 会话 |
| Plugin | 7 | Yaf\Plugin 插件 |
| Config | 32 | Yaf\Config 配置类 |
| Exception | 2 | Yaf\Exception 异常类 |

## 核心类详细说明

### Yaf\Application

```php
\Yaf\Application::app()     // 获取应用实例
\Yaf\Application::run()    // 运行应用
\Yaf\Application::__construct() // 构造函数
```

| 触发词 | 说明 |
|--------|------|
| `Yaf_Applicationapp` | 获取应用单例 |
| `Yaf_Applicationrun` | 启动应用 |
| `Yaf_Application__construct` | 构造函数 |
| `Yaf_Applicationbootstrap` | 启动引导 |
| `Yaf_Applicationenviron` | 获取环境 |
| `Yaf_Applicationexecute` | 执行回调 |
| `Yaf_ApplicationgetAppDirectory` | 获取应用目录 |
| `Yaf_ApplicationgetConfig` | 获取配置 |
| `Yaf_ApplicationgetDispatcher` | 获取调度器 |
| `Yaf_ApplicationgetLastErrorMsg` | 获取最后错误信息 |
| `Yaf_ApplicationgetLastErrorNo` | 获取最后错误码 |
| `Yaf_ApplicationgetModules` | 获取模块列表 |
| `Yaf_ApplicationsetAppDirectory` | 设置应用目录 |

### Yaf\Dispatcher

| 触发词 | 说明 |
|--------|------|
| `Yaf_DispatchergetInstance` | 获取调度器实例 |
| `Yaf_Dispatcherdispatch` | 分发请求 |
| `Yaf_DispatcherenableView` | 启用视图 |
| `Yaf_DispatcherdisableView` | 禁用视图 |
| `Yaf_DispatchergetApplication` | 获取应用实例 |
| `Yaf_DispatchergetRequest` | 获取请求对象 |
| `Yaf_DispatchergetRouter` | 获取路由器 |
| `Yaf_DispatcherautoRender` | 自动渲染 |
| `Yaf_DispatchercatchException` | 捕获异常 |

### Yaf\Request

| 触发词 | 说明 |
|--------|------|
| `Yaf_Request_AbstractgetMethod` | 获取请求方法 |
| `Yaf_Request_AbstractgetModuleName` | 获取模块名 |
| `Yaf_Request_AbstractgetControllerName` | 获取控制器名 |
| `Yaf_Request_AbstractgetActionName` | 获取动作名 |
| `Yaf_Request_AbstractgetParams` | 获取参数列表 |
| `Yaf_Request_AbstractgetParam` | 获取单个参数 |
| `Yaf_Request_AbstractisGet` | 是否 GET 请求 |
| `Yaf_Request_AbstractisPost` | 是否 POST 请求 |
| `Yaf_Request_AbstractisAjax` | 是否 AJAX 请求 |
| `Yaf_Request_AbstractclearParams` | 清除所有请求参数 |

### Yaf\Route

| 路由类型 | 触发词 | 说明 |
|----------|--------|------|
| Static | `Yaf_Route_Static` | 静态路由 |
| Simple | `Yaf_Route_Simple` | 简单路由 |
| Supervar | `Yaf_Route_Supervar` | 超变量路由 |
| Map | `Yaf_Route_Map` | 映射路由 |
| Regex | `Yaf_Route_Regex` | 正则路由 |
| Rewrite | `Yaf_Route_Rewrite` | 重写路由 |

### Yaf\Controller

| 触发词 | 说明 |
|--------|------|
| `Yaf_Controller_Abstractforward` | 转发请求 |
| `Yaf_Controller_Abstractredirect` | 重定向 |
| `Yaf_Controller_Abstractdisplay` | 渲染视图 |
| `Yaf_Controller_AbstractgetView` | 获取视图 |
| `Yaf_Controller_Abstractinit` | 初始化方法 |

### Yaf\View

| 触发词 | 说明 |
|--------|------|
| `Yaf_View_Simpledisplay` | 显示模板 |
| `Yaf_View_Simplerender` | 渲染模板 |
| `Yaf_View_Simpleassign` | 分配变量 |
| `Yaf_View_Simpleclear` | 清除变量 |

### Yaf\Plugin

| 触发词 | 说明 |
|--------|------|
| `Yaf_Plugin_AbstractrouterStartup` | 路由启动前 |
| `Yaf_Plugin_AbstractrouterShutdown` | 路由关闭后 |
| `Yaf_Plugin_AbstractdispatchLoopStartup` | 分发循环开始 |
| `Yaf_Plugin_AbstractpreDispatch` | 分发前 |
| `Yaf_Plugin_AbstractpostDispatch` | 分发后 |
| `Yaf_Plugin_AbstractdispatchLoopShutdown` | 分发循环结束 |

### Yaf\Registry

| 触发词 | 说明 |
|--------|------|
| `Yaf_Registryget` | 获取注册项 |
| `Yaf_Registryset` | 设置注册项 |
| `Yaf_Registryhas` | 检查注册项 |
| `Yaf_Registrydel` | 删除注册项 |

### Yaf\Session

| 触发词 | 说明 |
|--------|------|
| `Yaf_SessiongetInstance` | 获取会话实例 |
| `Yaf_Sessionstart` | 启动会话 |
| `Yaf_Sessionhas` | 检查会话值 |
| `Yaf_Sessionget` | 获取会话值 |
| `Yaf_Sessionset` | 设置会话值 |
| `Yaf_Sessiondel` | 删除会话值 |

### Yaf\Loader

| 触发词 | 说明 |
|--------|------|
| `Yaf_LoadergetInstance` | 获取加载器实例 |
| `Yaf_Loaderautoload` | 自动加载 |
| `Yaf_LoaderregisterLocalNamespace` | 注册本地命名空间 |
| `Yaf_LoadersetLibraryPath` | 设置类库路径 |

## 常量

| 触发词 | 说明 |
|--------|------|
| `Yaf_Version` | Yaf 版本号 |
| `Yaf_Environ` | 环境常量 |
| `Yaf_Err_*` | 错误常量集合 |

## 使用示例

```php
// 初始化应用
$app = \Yaf\Application::app();

// 获取配置
$config = \Yaf\Application::app()->getConfig();

// 获取调度器
$dispatcher = \Yaf\Dispatcher::getInstance();

// 转发请求
$this->forward('index', ['name' => 'value']);

// 重定向
$this->redirect('/url');

// 获取请求参数
$name = $this->getRequest()->getParam('name');
```

## 相关项目

| 项目 | 仓库地址 |
|------|----------|
| Yaf 语法提示 | https://github.com/chenbool/sublime_yaf |
| Swoole 语法提示 | https://github.com/chenbool/sublime_swoole |
| ThinkPHP5 语法提示 | https://github.com/chenbool/sublime_thinkphp5 |

## 交流群

- QQ 群：484043598

## License

MIT License
