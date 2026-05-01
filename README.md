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

> 更多触发词请查看对应目录下的 .sublime-snippet 文件

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
| sublime_swoole | https://github.com/chenbool/sublime_swoole |
| sublime_yaf | https://github.com/chenbool/sublime_yaf |
| sublime_thinkphp5 | https://github.com/chenbool/sublime_thinkphp5 |
| sublime_thinkphp6 | https://github.com/chenbool/sublime_thinkphp6 |
| sublime_thinkphp8 | https://github.com/chenbool/sublime_thinkphp8 |
| sublime_laravel | https://github.com/chenbool/sublime_laravel |
| sublime_workerman | https://github.com/chenbool/sublime_workerman |
| sublime_webman | https://github.com/chenbool/sublime_webman |
| sublime_fastadmin | https://github.com/chenbool/sublime_fastadmin |

## 交流群

- QQ 群：484043598

## License

MIT License
