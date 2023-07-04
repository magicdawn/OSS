# 岑涛 - 前端工程师

## 个人概况

- 性别 : 男
- 年龄 : 30
- 学历 : 华北电力大学(保定) - 2015 届 - 本科
- GitHub : https://github.com/magicdawn
- NPM : https://www.npmjs.com/~magicdawn
- 个人博客 : https://magicdawn.fun/

## 联系方式

magicdawn@qq.com / +86 15128208955

## 技能

- 精通 JavaScript, 熟悉 TypeScript, 精通 Node.js 平台.
- 熟悉 前端开发, 熟悉 React / Vue 技术栈.
- 熟悉 Node.js 后端开发. (Web 框架 / redis / MySQL / RabbitMQ) 等技术栈. (1.5 years)
- 熟练使用基于 Node.js 的工具链, 如 webpack / vite 等打包工具, babel / eslint / prettier 等工程化工具.
- 熟悉 Electron 平台, 有原生扩展开发经验(nan / napi). (1.5 years)

## 工作经历

### 2021.6 - 2021.11 石墨文档-武汉, 前端工程师

负责石墨文档-轻文档产品线的线上维护, 私有部署版本维护. 基于 Quill 的富文本编辑器研发.
我在其中完成了文档订阅 / 图片复制优化 / 跟随模式 等功能的研发.

### 2017.11 - 2021.5 滴滴, 高级前端工程师

#### 滴滴自研 IM: D-Chat

参与滴滴自研 IM D-Chat 的迭代开发, 项目技术栈为 Electron + React, 支持桌面端 Mac & Windows 客户端.
我在其中:

- 作为轮值版本负责人, 顺利完成版本迭代.
- 负责 IM 中文件/图片模块:
  - 优化了文件上传 / 下载.
  - 优化了图片复制/粘贴的效率, 使用 N-API 封装了 simple-mac-clipboard API, 解决 electron clipboard API 导致的 renderer crash.
  - 为桌面端引入图片压缩功能: 引入了 mozjpeg wasm / oxipng 为桌面端引入图片压缩功能, 后封装了基于 N-API 的 node-mozjpeg 等, 使图片不改变尺寸情况下大幅减少文件大小.
  - 为桌面端引入图片缩略图功能: 集成 sharp 库, 使端上拥有了基于原图生成缩略图的能力, 使用场景: 发送图片前预览, 自己发送的图片预缓存等.
  - 图片消息缓存优化等等.
- 参与设计了插件系统, 建设了插件脚手架(yeoman generator), 扩展 IM 成为工作台, 方便更多团队将业务集成进来.
- 代码片消息优化, 工作状态 等日常需求迭代.

#### 滴滴智慧交通-城市大脑

龙华大脑是基于内部滴禹 sass 平台, 为深圳市龙华区系统定制的智慧城市大脑项目, 是滴滴智慧交通第一个千万级合同.
我在其中整体负责龙华大脑项目开发, 交付.

- 项目初期, 独自支持了私有部署, 客户需求的 MVP 版本实现, 重要系统的开发.
- 项目后期, 带实习生 & 外包人员建设了重点车辆, 拥堵研判, 出行规律, 勤务考核等系统.
- 负责维护公共的 UI 组件库, 地图组件库, 项目脚手架, 公共 cli 工具等.

### 2016.05 - 2017.11 凤凰金融, Node.js & 前端工程师

#### 项目经历

- C 端主 App on Android 的打包/升级/灰度系统: 实现了安卓 apk 安装包根据基础包批量生成渠道包的功能, 系统开发过程中的时候因各种超时, 内存, 其他原因的失败问题, 整理实现了 promise.x 系列工具包, 很好支持了系统的平稳运行.
- C 端主 App 推送系统/消息中心: 基于 APNs/小米/极光的推送系统实现, 使用 rabbitmq 做任务调度, mysql 统计成功率, 在服务端实现了重试, 并发控制等功能.
- C 端主 App 美股模块, 实时行情长链接系统: 使用 socket.io 对接移动端 App 实现美股行情数据的推送, 并设计了数据节流, 数据压缩, 多机部署等方案.
- C 端主 App 美股模块, 用户开户入金与券商(FirstTrade)对接, 项目难点是宽松的用户资料输入与券商要求的严格输入之间的差距的抹平, 以及分布式架构下需保证券商提供接口的单点性, 后来通过 redis setnx 实现的 redlock 成功保证不会多次调用券商开户接口.
- 海外理财业务 - Api 侧: 实现了完整的用户系统, 对接了海外常用的 Facebook & Google signin, 实现了基于 redis 的限流方案. 还负责了短信平台的对接, 限流方案的设计等. 在使用 Sails 框架过程中整理开发了 waterline-auto 工具, 类似 sequelize-auto 自动从 MySQL 种读取表结构生成 Model, 极大方便了 Model 的编写.
- 海外理财业务 - FE 侧: 实现了基于 Vue 技术栈的 H5/PC C 端站点, 我在其中帮助团队引进了 eslint / prettier 等工程化工具, 规范了开发流程. 负责引入 Google Analytics / Google AdWords / Facebook Pixel 等常用海外营销统计工具. 此业务规模后来达到了千万级, 并且产生了盈利.
- 海外理财业务 - CMS 系统: 此项目是海外理财业务的内容管理系统(用户/标的/推荐位/奖励活动管理/配置中心 等), 团队基于 ant-design 选型了 React 技术栈, 在不熟悉 React 技术栈的情况下快速上手了开发, 并能快速迭代.

### 2015.07 - 2016.03 美团外卖, 前端工程师

#### 项目经历

外卖数据组 dolphin 数据可视化及决策平台的开发, 项目基于 jQuery / Highcharts / DataTable.
主要负责一些可视化大盘的开发, 一些基础服务的对接如公司 sso 系统. 在其中改进了 node.js proxy 层代理数据后端的
方式, 能基于配置化代理后端接口, 避免手动处理路由, 手动请求, 手动 map response 给前端. 推动了代码 review 的落地.

## 开源项目

- https://github.com/magicdawn/OSS 我创建的 应用/库 目录
- https://github.com/magicdawn/bilibili-app-recommend B 站首页推荐模块, 油猴脚本, 7K+ 活跃用户
- https://github.com/magicdawn/yun-playlist-downloader : 网易云音乐的歌单/专辑/电台下载器 cli, 支持并发控制, 音质选择, 出错重试等特性
- https://github.com/magicdawn/clash-config-manager clashX 配置生成器, Electron 桌面端 App
- https://github.com/magicdawn/weread-spy 基于 puppeteer 和微信读书网页版的 ePub 电子书生成器
- https://github.com/magicdawn/bj-hospital-vis : 北京社保定点医院的可视化
- https://github.com/magicdawn/impress-router : 将 Express 中的 router 移植到 koa 中
- https://github.com/magicdawn/node-mozjpeg : 基于 N-API 的 mozjpeg 的 node binding
- https://github.com/magicdawn/handy-img 图片压缩工具
- 更多查看 GitHub 主页 / npm 主页.

## 自我评价

善于抓住问题关键, 善于利用工具或创建好用的工具解决问题 <br />
记忆力不错.
