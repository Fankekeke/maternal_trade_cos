![](https://img.shields.io/badge/License-MIT-blue.svg)

![](https://img.shields.io/badge/Version-1.0.0-brightgreen.svg)

![](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

# 基于 SpringBoot + Vue 的母婴二手用品交易平台 (Buying and Selling Secondhand Baby and Maternity Items)

二手母婴用品 · 闲置交易 · 支付宝支付 · 收藏评价 · 消息互动 · 销售统计

本项目是一套面向母婴家庭闲置物品流转的二手交易平台，覆盖“商品发布、闲置交易、在线支付、订单管理、收藏评价、消息沟通、销售统计”等核心业务。系统分为管理员与普通用户两类角色：管理员负责平台整体运营、商品管理、订单管理、用户管理、评价管理、公告发布与销售统计；用户可发布闲置母婴用品、浏览交易市场、下单购买、在线支付、管理个人商品与订单、收藏心仪商品并对交易进行评价。

#### 安装环境
️**注意**：请确保您的开发环境已安装以下依赖。

JAVA 环境 

Node.js环境 [https://nodejs.org/en/] 选择14.17

Yarn 打开cmd， 输入npm install -g yarn !!!必须安装完毕nodejs

Mysql 数据库 一定要把账户和密码记住

redis

Idea 编译器

WebStorm OR VScode 编译器

#### 采用技术及功能

后端：SpringBoot、MybatisPlus、MySQL、Redis、
前端：Vue、Apex、Antd、Axios

平台前端：vue(框架) + vuex(全局缓存) + rue-router(路由) + axios(请求插件) + apex(图表)  + antd-ui(ui组件) + 百度地图 API

平台后台：springboot(框架) + redis(缓存中间件) + shiro(权限中间件) + mybatisplus(orm) + restful风格接口 + mysql(数据库)

开发环境：windows10 or windows7 ， vscode or webstorm ， idea + lambok

---

## 核心特性

- **母婴闲置商品发布**：用户可发布二手婴儿车、婴儿床、玩具、童装、奶粉罐、奶瓶、安全座椅等母婴用品，上传商品图片、描述新旧程度与交易价格。
- **交易市场浏览**：用户可按商品类型、价格区间、新旧程度、发布时间浏览二手母婴用品，支持关键词搜索。
- **支付宝在线支付**：用户下单后可通过支付宝完成在线支付，保障交易安全与支付便捷。
- **订单全流程管理**：支持待支付、已支付、待发货、已发货、已完成、已取消等订单状态流转，买卖双方可跟踪订单进度。
- **个人商品管理**：用户可管理自己发布的闲置商品，支持上架、下架、编辑、删除与查看商品浏览与成交情况。
- **卖出订单管理**：卖家可查看卖出订单，处理发货、确认收款与售后沟通。
- **我的收藏**：用户可收藏感兴趣的母婴用品，方便后续查看与购买。
- **评价管理**：交易完成后，买卖双方可对对方进行评价，形成信用反馈机制。
- **消息回复沟通**：买家与卖家可在线沟通商品详情、价格与交易方式，管理员可查看消息记录。
- **公告与首页图片管理**：管理员发布平台公告、交易规则与安全提示，并管理首页轮播图与推荐商品展示。
- **销售统计看板**：管理员可查看平台交易数据，包括订单数量、成交金额、热门商品类型、用户活跃度与销售趋势。
---

## 适用场景

- 母婴二手用品交易平台
- 闲置母婴物品交易商城
- 社区母婴用品交换平台
- 校园母婴二手市场
- 家庭闲置母婴用品流转平台
- 母婴用品二手交易社区
- 亲子闲置物品在线交易平台
---

## 功能模块概览

### 管理员端

- **用户管理**：管理用户账号、联系方式、账号状态、实名认证信息与历史交易记录。
- **商品管理**：查看平台全部二手母婴用品，支持违规商品下架、敏感信息处理与商品状态管理。
- **商品类型**：维护母婴二手商品分类，如婴儿车、婴儿床、童装、玩具、喂养用品、安全座椅、绘本等。
- **订单管理**：查看平台全部订单，跟踪订单状态，处理交易纠纷与异常订单。
- **评价管理**：查看用户对交易的评价，支持评价审核、隐藏与异常评价处理。
- **用户收藏**：查看用户收藏商品数据，分析用户偏好与热门商品。
- **消息回复**：查看用户之间的沟通消息，处理投诉与争议沟通记录。
- **公告管理**：发布平台公告、交易规则、安全提示、活动通知与系统维护信息。
- **销售统计**：统计订单数量、成交金额、热门商品类型、用户交易量、销售趋势与平台运营数据。
- **首页图片**：管理首页轮播图、推荐商品图片与平台宣传图片。

### 用户端

- **个人信息**：维护头像、昵称、联系方式、收货地址与个人简介。
- **交易市场**：浏览二手母婴用品，按分类、价格、新旧程度筛选商品，支持关键词搜索。
- **我的商品**：发布、编辑、下架、删除自己发布的闲置母婴用品，查看商品浏览与成交情况。
- **订单管理**：查看买入订单，跟踪待支付、已支付、待发货、已发货、已完成等状态。
- **卖出订单**：查看卖出订单，处理发货、确认收款、与买家沟通售后问题。
- **我的收藏**：收藏感兴趣的母婴用品，方便后续查看与下单购买。
- **评价管理**：对已完成交易进行评价，查看他人对自己的评价，积累交易信用。
- **支付宝在线支付**：对买入订单进行支付宝支付，查看支付状态与交易明细。

---

## 项目结构

```text
pharmacy-dispensing-system/
├── backend/            # 后端 API 服务
│   ├── src/
│   │   ├── controllers/  # 控制器
│   │   ├── models/       # 数据模型
│   │   ├── routes/       # 路由
│   │   └── services/     # 业务逻辑
│   └── package.json
├── frontend/           # 前端 Web 应用
│   ├── src/
│   │   ├── views/      # 页面视图
│   │   ├── components/ # 公共组件
│   │   └── store/      # 状态管理
│   └── package.json
├── docs/               # 项目文档与 API 接口说明
├── LICENSE
└── README.md
```
---


#### 前台启动方式
安装所需文件 yarn install 
运行 yarn run dev

#### 默认后台账户密码
[管理员]
admin
123456

[用户]
fank
123456

#### 项目截图
|  |  |
|---------------------|---------------------|
| ![](./assets/image%20(1).png) | ![](./assets/image%20(2).png) |
| ![](./assets/image%20(3).png) | ![](./assets/image%20(4).png) |
| ![](./assets/image%20(5).png) | ![](./assets/image%20(6).png) |
| ![](./assets/image%20(7).png) | ![](./assets/image%20(8).png) |
| ![](./assets/image%20(9).png) | ![](./assets/image%20(10).png) |
| ![](./assets/image%20(11).png) | ![](./assets/image%20(12).png) |
| ![](./assets/image%20(13).png) | ![](./assets/image%20(14).png) |
| ![](./assets/image%20(15).png) | ![](./assets/image%20(16).png) |
| ![](./assets/image%20(17).png) | ![](./assets/image%20(18).png) |
| ![](./assets/image%20(19).png) | 

#### 演示视频

暂无

#### 获取方式

Email: fan1ke2ke@gmail.com

WeChat: `Storm_Berserker`

`附带部署与讲解服务，因为要恰饭资源非免费，伸手党勿扰，谢谢理解😭`

> 1.项目纯原创，不做二手贩子 2.一次购买终身有效 3.项目讲解持续到答辩结束 4.非常负责的答辩指导 5.**黑奴价格**

> 项目部署调试不好包退！功能逻辑没讲明白包退！

<div align=center><img align="center" src="./assets/product_word.png" alt="fankekeke" /></div>

#### 其它资源
[2026年-答辩顺利通过-客户评价🀄](https://berserker287.github.io/2026/06/29/2026%E5%B9%B4%E7%AD%94%E8%BE%A9%E9%A1%BA%E5%88%A9%E9%80%9A%E8%BF%87/)

[2025年-答辩顺利通过-客户评价🍜](https://berserker287.github.io/2025/06/18/2025%E5%B9%B4%E7%AD%94%E8%BE%A9%E9%A1%BA%E5%88%A9%E9%80%9A%E8%BF%87/)

[2024年-答辩顺利通过-客户评价👻](https://berserker287.github.io/2024/06/06/2024%E5%B9%B4%E7%AD%94%E8%BE%A9%E9%A1%BA%E5%88%A9%E9%80%9A%E8%BF%87/)

[2023年-答辩顺利通过-客户评价🐢](https://berserker287.github.io/2023/06/14/2023%E5%B9%B4%E7%AD%94%E8%BE%A9%E9%A1%BA%E5%88%A9%E9%80%9A%E8%BF%87/)

[2022年-答辩通过率100%-客户评价🐣](https://berserker287.github.io/2022/05/25/%E9%A1%B9%E7%9B%AE%E4%BA%A4%E6%98%93%E8%AE%B0%E5%BD%95/)

[毕业答辩导师提问的高频问题](https://berserker287.github.io/2023/06/13/%E6%AF%95%E4%B8%9A%E7%AD%94%E8%BE%A9%E5%AF%BC%E5%B8%88%E6%8F%90%E9%97%AE%E7%9A%84%E9%AB%98%E9%A2%91%E9%97%AE%E9%A2%98/)

[50个高频答辩问题-技术篇](https://berserker287.github.io/2023/06/13/50%E4%B8%AA%E9%AB%98%E9%A2%91%E7%AD%94%E8%BE%A9%E9%97%AE%E9%A2%98-%E6%8A%80%E6%9C%AF%E7%AF%87/)

[计算机毕设答辩时都会问到哪些问题？](https://www.zhihu.com/question/31020988)

[计算机专业毕业答辩小tips](https://zhuanlan.zhihu.com/p/145911029)

#### 接JAVAWEB毕设，纯原创，价格公道，诚信第一

`网站建设、小程序、H5、APP、各种系统 选题+开题报告+任务书+程序定制+安装调试+项目讲解+论文+答辩PPT`

More info: [悲伤的橘子树](https://berserker287.github.io/)

<div align="center"><img align="center" src="./assets/chat_qr_code.png" alt="fankekeke" width=250 /></div>

<p><img align="center" src="./assets/wechat_group.png" alt="fankekeke" /></p>

**感谢查看**
