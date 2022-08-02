<h1 align="center">Welcome to Hamibot-starter 👋</h1>
<p align="center">
  <a href="https://www.npmjs.com/package/script-template" target="_blank">
    <img alt="Version" src="https://img.shields.io/npm/v/script-template.svg">
  </a>
  <a href="#" target="_blank">
    <img alt="License: MPL--2.0" src="https://img.shields.io/badge/License-MPL--2.0-yellow.svg" />
  </a>
</p>

> 一个用来快速开始编写 `Hamibot` 脚本的模板，使用 `TypeScript` 编写。
>
> 通过声明文件提供 `Hamibot` 绝大部分函数的代码提示、类型检查和文档，帮你减少键入次数和查询官方文档的时间。提供常用的代码片段，直接调用可以辅助更快完成开发，并让你能专注于核心功能。
>
> 欢迎各位大佬帮我一起完善这个项目！

## 安装依赖

```sh
npm install
```

## 使用方法

在 `.\src` 文件夹下编写代码，程序入口为 `src\index.ts` 。

完成编写以后使用下面的命令打包项目，打包后的文件路径为: `.\dist\bundle.js` 。

```sh
npm run build
```

## 注意事项

1. 编写 UI 或悬浮窗时请记得将文件扩展名修改成 `tsx` 。
2. 有时候函数的返回值可能会根据某个参数或者设置而改变，此时如果你十分确定不会出现问题，请使用断言，例如：

```typescript
// 类型断言
let xxx = sensors.register("xxx") as SensorEventEmitter;

// 非空断言（推荐，因为有的类型被隐藏了，想要使用还需要手动导入。）
let yyyy = sensors.register("yyy")!;
```

## TODO List

- [ ] 添加声明文件 [23/26]
  - [ ] UI
  - [ ] Util
  - [ ] Canvans
- [ ] 使用 `Eslint` 在提交前统一代码风格
- [ ] 将所有的预制函数使用 `TypeScript` 重写
- [ ] 检查泛型注释
- [ ] 检查回调函数注释
- [ ] 检查注释中的类和方法是否使用行内代码格式
- [ ] 检查注释中的示例代码是否都能够运行
- [ ] 统一函数类型（Function、function）

## 作者

👤 **BATU1579**

- Github: [@batu1579](https://github.com/batu1579)

## 支持

如果有帮到你的话，帮我点颗小星星叭~ ⭐️

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_
