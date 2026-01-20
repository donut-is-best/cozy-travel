  Cozy Travel  治愈系旅行助手

> A Healing Travel Assistant App based on Android & Bmob Cloud Backend.  
> 基于 Android 原生 + Bmob 云后端的治愈系旅行助手 App。

一、项目简介

Cozy Travel 是一款专为旅行爱好者设计的 Android 应用。不同于传统的工具类 App，本项目采用“治愈系”的 UI 设计风格（米色暖调 + 扁平化），旨在为用户提供从灵感发现、行程规划到旅途陪伴的一站式体验。

本项目采用 Android Native + H5 混合开发 模式，集成了 Bmob 后端云 实现数据同步，并引入 Three.js 实现 3D 地球可视化交互。

核心功能 (Key Features)

 1.  灵感发现与 3D 地球
 瀑布流列表：展示全球热门景点（京都、瑞士、大理等），支持流畅的滑动浏览。
 3D 地球漫游：集成 Three.js (WebGL)，实现可交互的 3D 地球模型。支持 3D 坐标转换与射线检测，点击地球热点即可跳转原生详情页。
 盲盒抽奖：多线程实现的趣味盲盒功能，随机抽取你的下一个旅行目的地。

 2.  沉浸式音乐陪伴
 全局音乐播放：基于 `MediaPlayer` + 单例模式封装，支持跨页面无缝播放。
 动态交互：实现黑胶唱片旋转动画 (`ObjectAnimator`)，动画状态与音乐播放/暂停逻辑实时同步。

 3.  云端数据同步 (Bmob)
 用户鉴权：支持用户注册、登录、自动登录（缓存机制）。
 行程管理：用户的旅行计划存储于 Bmob 云数据库，支持增删改查 (CRUD) 及多端实时同步。
 个人中心：展示用户头像、昵称及账户管理。


 开发语言: Java (Android SDK)
 架构模式: MVC, Singleton Pattern (单例), Adapter Pattern (适配器)
 前端/混合: WebView, JavaScript, Three.js (3D Rendering)
 后端服务: Bmob Backend Cloud (BaaS)  User & Data Management
 数据存储: SQLite (Local), SharedPreferences, Bmob Cloud Database
 动画技术: Property Animation (ObjectAnimator), Lottie (Loading)





如果需要使用项目请先在 Bmob 后台申请一个应用 ID，替换项目中的 `YOUR_BMOB_APP_ID`。
请前往 Application.java 或 MainActivity.java 中替换为你自己的 Application ID：

Bmob.initialize(this, "YOUR_BMOB_APP_ID");



⚠️ 免责声明 
本项目为课程设计/个人学习作品。

应用内的图片与音乐资源来源于网络，版权归原作者所有。

如有侵权，请联系删除。

请勿将本项目直接用于商业用途。






