# Vue3 组件库搭建
## 一、搭建monorepo环境
> 使用 pnpm workspace 来实现 monorepo.
>
> 使用pnpm 安装包速度快，磁盘利用率高效，使用pnpm 可以快速建立 monorepo.

```javascript
npm install -g pnpm   # 全局安装pnpm
# 我这么安装了没屁用,所以我直接查了pnpm 的文档:https://www.pnpm.cn/installation

pnpm init # 初始化package.json 配置文件

pnpm install vue@next typescript -D 全局下添加依赖

npx tsc --init # 初始化ts配置文件
```
