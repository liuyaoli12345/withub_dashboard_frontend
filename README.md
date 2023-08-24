# 这是Withub后台管理系统前端手脚架
## 快速开始
``` shell
 pnpm install
 pnpm dev
```
## To-dos
- 完善登录系统（目前是直接返回true）
- 完善dashboard
  - 添加用户管理模块
    - 搜索用户
    - 编辑、删除、添加用户
  - 添加课程管理模块
    - 爬虫操作中心
    - 搜索课程（应当提供按id搜索、按名称搜索和按教师搜索）
    - 课程流
  - 添加监控大屏
    - 需要等到主项目完成再实现
  - 添加报告模块
    - 需要等到主项目完成

## How to implement
- 用户管理模块
  - 目前对应组件UserManage.tsx
  - 没有api，没有子组件
- 课程管理模块
  - 目前对应ClassManage.tsx
  - 只有一个返回假数据的api Classinfo
  - 子组件ClassCard，是课程卡片，课程卡片应该还要提供一个详情页，还没有设计嘞
- 爬虫操作中心
  - 在课程管理模块下，后面考虑单独设一个爬虫的目录

## Problems
- ScrollTop里面UseScrollTrigger总是不生效，目前是直接让Fade组件接收true来保证始终在显示
  