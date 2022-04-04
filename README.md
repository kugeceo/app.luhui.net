# Create React App [![Build Status](https://dev.azure.com/facebook/create-react-app/_apis/build/status/facebook.create-react-app?branchName=main)](https://dev.azure.com/facebook/create-react-app/_build/latest?definitionId=1&branchName=main) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-green.svg)](https://github.com/facebook/create-react-app/blob/main/CONTRIBUTING.md)

<img alt="Logo" align="right" src="https://create-react-app.dev/img/logo.svg" width="20%" />

Create React apps with no build configuration.

- [Creating an App](#creating-an-app) – How to create a new app.
- [User Guide](https://facebook.github.io/create-react-app/) – How to develop apps bootstrapped with Create React App.

Create React App works on macOS, Windows, and Linux.<br>
If something doesn’t work, please [file an issue](https://github.com/facebook/create-react-app/issues/new).<br>
If you have questions or need help, please ask in [GitHub Discussions](https://github.com/facebook/create-react-app/discussions).

## Quick Overview

```sh
npx create-react-app my-app
cd my-app
npm start
```

If you've previously installed `create-react-app` globally via `npm install -g create-react-app`, we recommend you uninstall the package using `npm uninstall -g create-react-app` or `yarn global remove create-react-app` to ensure that npx always uses the latest version.

_([npx](https://medium.com/@maybekatz/introducing-npx-an-npm-package-runner-55f7d4bd282b) comes with npm 5.2+ and higher, see [instructions for older npm versions](https://gist.github.com/gaearon/4064d3c23a77c74a3614c498a8bb1c5f))_

Then open [http://localhost:3000/](http://localhost:3000/) to see your app.<br>
When you’re ready to deploy to production, create a minified bundle with `npm run build`.

<p align='center'>
<img src='https://cdn.jsdelivr.net/gh/facebook/create-react-app@27b42ac7efa018f2541153ab30d63180f5fa39e0/screencast.svg' width='600' alt='npm start'>
</p>

### Get Started Immediately

You **don’t** need to install or configure tools like webpack or Babel.<br>
They are preconfigured and hidden so that you can focus on the code.

Create a project, and you’re good to go.

## Creating an App

**You’ll need to have Node 14.0.0 or later version on your local development machine** (but it’s not required on the server). We recommend using the latest LTS version. You can use [nvm](https://github.com/creationix/nvm#installation) (macOS/Linux) or [nvm-windows](https://github.com/coreybutler/nvm-windows#node-version-manager-nvm-for-windows) to switch Node versions between different projects.

To create a new app, you may choose one of the following methods:

### npx

```sh
npx create-react-app my-app
```

_([npx](https://medium.com/@maybekatz/introducing-npx-an-npm-package-runner-55f7d4bd282b) is a package runner tool that comes with npm 5.2+ and higher, see [instructions for older npm versions](https://gist.github.com/gaearon/4064d3c23a77c74a3614c498a8bb1c5f))_

### npm

```sh
npm init react-app my-app
```

_`npm init <initializer>` is available in npm 6+_

### Yarn

```sh
yarn create react-app my-app
```

_[`yarn create <starter-kit-package>`](https://yarnpkg.com/lang/en/docs/cli/create/) is available in Yarn 0.25+_

It will create a directory called `my-app` inside the current folder.<br>
Inside that directory, it will generate the initial project structure and install the transitive dependencies:

```
my-app
├── README.md
├── node_modules
├── package.json
├── .gitignore
├── public
│   ├── favicon.ico
│   ├── index.html
│   └── manifest.json
└── src
    ├── App.css
    ├── App.js
    ├── App.test.js
    ├── index.css
    ├── index.js
    ├── logo.svg
    └── serviceWorker.js
    └── setupTests.js
```

No configuration or complicated folder structures, only the files you need to build your app.<br>
Once the installation is done, you can open your project folder:

```sh
cd my-app
```

Inside the newly created project, you can run some built-in commands:

### `npm start` or `yarn start`

Runs the app in development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will automatically reload if you make changes to the code.<br>
You will see the build errors and lint warnings in the console.

<p align='center'>
<img src='https://cdn.jsdelivr.net/gh/marionebl/create-react-app@9f6282671c54f0874afd37a72f6689727b562498/screencast-error.svg' width='600' alt='Build errors'>
</p>

### `npm test` or `yarn test`

Runs the test watcher in an interactive mode.<br>
By default, runs tests related to files changed since the last commit.

[Read more about testing.](https://facebook.github.io/create-react-app/docs/running-tests)

### `npm run build` or `yarn build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>

Your app is ready to be deployed.

## User Guide

You can find detailed instructions on using Create React App and many tips in [its documentation](https://facebook.github.io/create-react-app/).

## How to Update to New Versions?

Please refer to the [User Guide](https://facebook.github.io/create-react-app/docs/updating-to-new-releases) for this and other information.

## Philosophy

- **One Dependency:** There is only one build dependency. It uses webpack, Babel, ESLint, and other amazing projects, but provides a cohesive curated experience on top of them.

- **No Configuration Required:** You don't need to configure anything. A reasonably good configuration of both development and production builds is handled for you so you can focus on writing code.

- **No Lock-In:** You can “eject” to a custom setup at any time. Run a single command, and all the configuration and build dependencies will be moved directly into your project, so you can pick up right where you left off.

## What’s Included?

Your environment will have everything you need to build a modern single-page React app:

- React, JSX, ES6, TypeScript and Flow syntax support.
- Language extras beyond ES6 like the object spread operator.
- Autoprefixed CSS, so you don’t need `-webkit-` or other prefixes.
- A fast interactive unit test runner with built-in support for coverage reporting.
- A live development server that warns about common mistakes.
- A build script to bundle JS, CSS, and images for production, with hashes and sourcemaps.
- An offline-first [service worker](https://developers.google.com/web/fundamentals/getting-started/primers/service-workers) and a [web app manifest](https://developers.google.com/web/fundamentals/engage-and-retain/web-app-manifest/), meeting all the [Progressive Web App](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app) criteria. (_Note: Using the service worker is opt-in as of `react-scripts@2.0.0` and higher_)
- Hassle-free updates for the above tools with a single dependency.

Check out [this guide](https://github.com/nitishdayal/cra_closer_look) for an overview of how these tools fit together.

The tradeoff is that **these tools are preconfigured to work in a specific way**. If your project needs more customization, you can ["eject"](https://facebook.github.io/create-react-app/docs/available-scripts#npm-run-eject) and customize it, but then you will need to maintain this configuration.

## Popular Alternatives

Create React App is a great fit for:

- **Learning React** in a comfortable and feature-rich development environment.
- **Starting new single-page React applications.**
- **Creating examples** with React for your libraries and components.

Here are a few common cases where you might want to try something else:

- If you want to **try React** without hundreds of transitive build tool dependencies, consider [using a single HTML file or an online sandbox instead](https://reactjs.org/docs/try-react.html).

- If you need to **integrate React code with a server-side template framework** like Rails, Django or Symfony, or if you’re **not building a single-page app**, consider using [nwb](https://github.com/insin/nwb), or [Neutrino](https://neutrino.js.org/) which are more flexible. For Rails specifically, you can use [Rails Webpacker](https://github.com/rails/webpacker). For Symfony, try [Symfony's webpack Encore](https://symfony.com/doc/current/frontend/encore/reactjs.html).

- If you need to **publish a React component**, [nwb](https://github.com/insin/nwb) can [also do this](https://github.com/insin/nwb#react-components-and-libraries), as well as [Neutrino's react-components preset](https://neutrino.js.org/packages/react-components/).

- If you want to do **server rendering** with React and Node.js, check out [Next.js](https://nextjs.org/) or [Razzle](https://github.com/jaredpalmer/razzle). Create React App is agnostic of the backend, and only produces static HTML/JS/CSS bundles.

- If your website is **mostly static** (for example, a portfolio or a blog), consider using [Gatsby](https://www.gatsbyjs.org/) or [Next.js](https://nextjs.org/). Unlike Create React App, Gatsby pre-renders the website into HTML at build time. Next.js supports both server rendering and pre-rendering.

- Finally, if you need **more customization**, check out [Neutrino](https://neutrino.js.org/) and its [React preset](https://neutrino.js.org/packages/react/).

All of the above tools can work with little to no configuration.

If you prefer configuring the build yourself, [follow this guide](https://reactjs.org/docs/add-react-to-an-existing-app.html).

## React Native

Looking for something similar, but for React Native?<br>
Check out [Expo CLI](https://github.com/expo/expo-cli).

## Contributing

We'd love to have your helping hand on `create-react-app`! See [CONTRIBUTING.md](CONTRIBUTING.md) for more information on what we're looking for and how to get started.

## Supporting Create React App

Create React App is a community maintained project and all contributors are volunteers. If you'd like to support the future development of Create React App then please consider donating to our [Open Collective](https://opencollective.com/create-react-app).

## Credits

This project exists thanks to all the people who [contribute](CONTRIBUTING.md).<br>
<a href="https://github.com/facebook/create-react-app/graphs/contributors"><img src="https://opencollective.com/create-react-app/contributors.svg?width=890&button=false" /></a>

Thanks to [Netlify](https://www.netlify.com/) for hosting our documentation.

## Acknowledgements

We are grateful to the authors of existing related projects for their ideas and collaboration:

- [@eanplatter](https://github.com/eanplatter)
- [@insin](https://github.com/insin)
- [@mxstbr](https://github.com/mxstbr)

## License

Create React App is open source software [licensed as MIT](https://github.com/facebook/create-react-app/blob/main/LICENSE). The Create React App logo is licensed under a [Creative Commons Attribution 4.0 International license](https://creativecommons.org/licenses/by/4.0/).

Best App
----

*经常会有朋友想知道有哪些 Apps 或 服务 是值得付费来使用的，或者有哪些产品是可以提升生活品质的，
于是创建了 BestApp 项目，旨在让推荐变得有章可循*

## 总目录

欢迎大家推荐好的 App/产品 加入，请`Star`、`Pull Request`或在 [收集&提交页] 中提交 :)

1. [付费 Apps 推荐列表(macOS)](./README.md)
2. [付费 Apps 推荐列表(iOS & Cydia)](./Best-App-iOS.md)
3. [免费 Apps 推荐(macOS)](./Best-App-Mac-Free.md) - 整理中...
4. [免费 Apps 推荐列表(iOS & Cydia)](./Best-App-iOS-Free.md) - 整理中...
5. [苹果设备 周边&配件 推荐列表](./Best-Accessories-Apple.md)
6. [付费 Apps 推荐列表(Android)](./Best-App-Android.md) - 整理中...
7. [改善生活+提升幸福度物品 推荐列表](./Best-Life-Products.md) - 整理中...

====

>注1：以下功能简述中不再使用 `最好的`、`最强的`、`最完美的` 等主观性较强的表达，因为默认此列表中的 Apps 都是非常出色的。  
>注2：行末的 **#** 为相关 测评文章 或 同类横向对比文章 链接，请自行参阅。  
>注3：本项目 **不接受** 任何形式的捐赠、资助或广告。

## 1. 付费软件篇 (macOS)

`macOS`平台下有众多优秀的软件工具。
下面先就付费软件做一个推荐列表，希望供大家购买付费App时参考。

#### 1.1 效率工具类

评分   | 名称  | 功能简述 | 单价 | 测评
----- | ----- | ------ | ----- | -----
<a href="#Alfred" name="Alfred">★</a>★★★★ | [Alfred] | 效率软件 Top#1，不解释 | £17 | [#](https://www.macstories.net/reviews/alfred-2-rewritten-from-the-ground-up-workflows-themes-and-more/)
<a href="#MenubarX" name="MenubarX">★</a>★★★★ | [MenubarX] | 效率工具，强大的菜单栏浏览器 | 限免中 | [#](https://www.producthunt.com/posts/menubarx)
<a href="#1Password" name="1Password">★</a>★★★★ | [1Password] | 密码管理，自动登录，用过就离不开了 | $49.99 | [#](https://www.macstories.net/reviews/1password-4-for-mac-review/)
<a href="#Moom" name="Moom">★</a>★★★★ | [Moom] | 窗口管理，多屏切换工具 | $10 | [#](http://mac.appstorm.net/reviews/productivity-review/moom-window-management-rethought/)
<a href="#Magnet" name="Magnet">★</a>★★★★ | [Magnet] | 窗口管理，上架了AppStore | ￥12 | [#](https://medium.com/@davidmles/moom-vs-magnet-493fd2d31a77)
<a href="#iStat-Menus" name="iStat-Menus">★</a>★★★★ | [iStat Menus] | 实时显示系统状态、网速等 | $16 | [#](http://mac.appstorm.net/reviews/utilities/istat-menus-4-menubar-system-monitoring-improved/)
<a href="#Bartender" name="Bartender">★</a>★★★★ | [Bartender] | 自定义右上角 Menu 栏图标 | $15 | [#](http://www.macworld.com/article/2013739/mac-gems-bartender-helps-you-take-control-of-menu-bar-icons.html)
<a href="#Fantastical" name="Fantastical">★</a>★★★☆ | [Fantastical] | 基于日历的 GTD 提醒 | $19.99 | [#](http://www.macworld.com/article/2058681/fantastical-2-for-iphone-review-calendar-app-gets-more-fantastic-for-ios-7.html)
<a href="#Tweetbot" name="Tweetbot">★</a>★★★☆ | [Tweetbot] | Twitter 客户端 | $19.99 | [#](http://www.macworld.com/article/2012647/mac-gems-tweetbot-for-mac-is-exactly-what-youd-expect.html)
<a href="#Airmail" name="Airmail">★</a>★★★☆ | [Airmail] | Email 客户端新秀 | $9.99 | [#](http://mac.appstorm.net/reviews/communication-review/airmail-a-real-sparrow-alternative/)
<a href="#jitouch" name="jitouch">★</a>★★★☆ | [jitouch] | 触控板增强，画个字母B，打开浏览器 | $7.99 | [#](http://www.macworld.com/article/1151457/jitouch.html)
<a href="#OmniFocus" name="OmniFocus">★</a>★★★☆ | [OmniFocus] | 著名 GTD，上手之后秒杀同类 | $79.99 | [#](http://www.asianefficiency.com/technology/omnifocus-mac-review/)
<a href="#Keyboard-Maestro" name="Keyboard-Maestro">★</a>★★★☆ | [Keyboard Maestro] | 定制键盘快捷操作 | $36 | [#](http://mac.appstorm.net/how-to/productivity-how-to/how-to-become-a-mac-keyboard-maestro/)
<a href="#SteerMouse" name="SteerMouse">★</a>★★★☆ | [SteerMouse] | 鼠标和键盘组合按键，让鼠标替代触摸板手势 | $19.99 | [#](https://download.cnet.com/SteerMouse/3000-18491_4-76439.html)
<a href="#PopClip" name="PopClip">★</a>★★★☆ | [PopClip] | 类 iOS 文字选中弹出 Menu 扩展 | $4.99 | [#](http://mac.appstorm.net/reviews/productivity-review/popclip-the-unexpectedly-awesome-productivity-tool/)
<a href="#Clear" name="Clear">★</a>★★★☆ | [Clear] | 轻量级GTD工具、支持 iCloud 同步  | $9.99 | [#](https://www.macstories.net/reviews/clear-for-mac-review/)
<a href="#BreakTime" name="BreakTime">★</a>★★★☆ | [BreakTime] | 健康管理和休息提醒，番茄工作法 | $4.99 | [#](http://www.macworld.com/article/1164136/break_time_reminds_you_to_take_five.html)
<a href="#Timing" name="Timing">★</a>★★★☆ | [Timing] | 统计 Mac 使用习惯，每天做了什么 | $19.99 | [#](http://macdownload.informer.com/timing1/)
<a href="#CleanMyMac" name="CleanMyMac">★</a>★★★☆ | [CleanMyMac] | 系统清理优化，正如其名 | $39.95 | [#](http://www.macworld.com/article/2036159/review-cleanmymac-2-removes-unnecessary-files-to-free-up-storage-space.html)
<a href="#Hazel" name="Hazel">★</a>★★★☆ | [Hazel] | 自动化整理工具 | $28 | [#](http://www.macworld.com/article/1165835/hazel_the_standout_file_organizer_gets_even_smarter.html)
<a href="#Things" name="Things">★</a>★★★☆ | [Things] | 又一个 GTD | $49.99 | [#](http://www.lifehack.org/articles/productivity/battle-of-the-mac-and-ios-productivity-apps-omnifocus-vs-things-2-0.html)
<a href="#TextExpander" name="TextExpander">★</a>★★★☆ | [TextExpander] | 短语扩展，快速键入 | $34.95  | [#](http://mac.appstorm.net/reviews/productivity-review/head-to-head-text-expander-mac-software-compared/)
<a href="#GhostNote" name="GhostNote">★</a>★★★☆ | [GhostNote] | 基于文件的笔记 & 便签 | $4.99  | [#](https://zhuanlan.zhihu.com/pinapps/19971562)
<a href="#aText" name="aText">★</a>★★★☆ | [aText] | 同 TextExpander 快速键入 | $4.99  | [#](http://mac.appstorm.net/reviews/productivity-review/atext-a-text-expansion-contender/)
<a href="#Devonthink-Pro" name="Devonthink Pro">★</a>★★★☆ | [Devonthink Pro] | 文件管理/搜索工具，很强大 | $79.95 | [#](http://www.macworld.com/article/1161735/review_devonthink_pro_office_2_2_1_helps_manage_your_data.html)
<a href="#Ember" name="Ember">★</a>★★★☆  | [Ember] | 设计/素材订阅器及素材管理，如 Dribbble | $32.99 | [#](http://www.theverge.com/2013/7/23/4546974/ember-for-mac-app-evernote-alternative)
<a href="#Inboard" name="Inboard">★</a>★★★☆  | [Inboard] | 国产设计/素材订阅器及素材管理，如 Dribbble | ¥128 | [#](http://www.waerfa.com/inboard)
<a href="#Writer-Pro" name="Writer Pro">★</a>★★★☆ | [Writer Pro] | 写作利器，iA Writer的续作 | $19.99 | [#](http://mac.appstorm.net/reviews/office-review/writer-pro-is-an-exercise-in-disappointment/)
<a href="#BetterSnap-Tool" name="BetterSnap Tool">★</a>★★★☆ | [BetterSnap Tool] | 窗口管理工具，同 Moom、Divvy | €1.79 | [#](http://mac.appstorm.net/reviews/utilities/bettersnaptool-full-featured-window-management/)
<a href="#KeyCue" name="KeyCue">★</a>★★★☆ | [KeyCue] | 帮助你打开快捷大全菜单 | €19.99 | [#](http://www.osxtoy.com/?p=1054)
<a href="#Little-Snitch" name="Little Snitch">★</a>★★★  | [Little Snitch] | 防火墙、网络请求监控 | €29.95 | [#](http://www.macworld.com/article/2017161/mac-gems-little-snitch-snitches-on-misbehaving-apps.html)
<a href="#OmniGraffle" name="OmniGraffle">★</a>★★★  | [OmniGraffle] | 专业绘图制表工具，推荐v6.0 | $99.99 | [#](http://www.macworld.com/article/1136253/omnigrafflepro5.html)
<a href="#ForkLift" name="ForkLift">★</a>★★★  | [ForkLift] | Finder替代品兼FTP工具 | $19.95 | [#](http://mac.appstorm.net/reviews/forklift-the-fast-functional-ftp-client/)
<a href="#Scrapbook" name="Scrapbook">★</a>★★★  | [Scrapbook] | 剪切板历史记录 (注:Alfred 自带此功能) | $0.99 | [#](http://mac.appstorm.net/general/an-in-depth-look-at-ember-the-new-digital-scrapbook/)
<a href="#Xee" name="Xee">★</a>★★★  | [Xee] | 图片浏览工具，可替代原生 | $4.5 | [#](http://www.cultofmac.com/49171/review-xee-a-cute-little-image-browser/)
<a href="#PhotoDesk" name="PhotoDesk">★</a>★★★  | [PhotoDesk] | Instagram 客户端，功能齐全 | $4.99 | [#](http://noodlemac.com/2015/06/photodesk-is-mostly-instagram-on-a-mac/)
<a href="#Should-I-Sleep" name="Should-I-Sleep">★</a>★★★  | [Should I Sleep] | 让你的Mac不仅节能，而且智能 | $9.99 | [#](http://www.macworld.com/article/2044786/mac-gems-should-i-sleep-puts-your-mac-into-a-proper-sleep-routine.html)
<a href="#SaneDesk" name="SaneDesk">★</a>★★★  | [SaneDesk] | 高效的切换/隐藏桌面工作区 | $17.99 | [#](http://mac.appstorm.net/reviews/utilities/sanedesk-empower-your-mac-desktop/)
<a href="#Noizio" name="Noizio">★</a>★★★  | [Noizio] | 让人感觉置身大自然的白噪声音效模拟工具 | $4.99 | [#](http://www.appinn.com/noizio-for-os-x/)
<a href="#Entropy" name="Entropy">★</a>★★☆  | [Entropy] | 华丽高效快捷压缩工具 | $18.99 | [#](http://www.macupdate.com/app/mac/38116/entropy)
<a href="#Pixelmator" name="Pixelmator">★</a>★★☆  | [Pixelmator] | 不想用Photoshop？试试它 | $29.99 | [#](http://mac.appstorm.net/reviews/graphics/clash-of-the-image-editors-acorn-vs-pixelmator/)
<a href="#PaintCode" name="PaintCode">★</a>★★☆  | [PaintCode] | OC开发/设计工具 | $80 | [#](http://www.paintcodeapp.com/news/introducing-paintcode-2)
<a href="#ScreenFlow" name="ScreenFlow">★</a>★★☆  | [ScreenFlow] | 屏幕录制、视频剪辑 | $99 | [#](http://www.macworld.com/article/2039696/review-screenflow-4-a-great-but-quirky-video-capture-and-edit-tool.html)
<a href="#OmmWriter" name="OmmWriter">★</a>★★☆  | [OmmWriter] | 静心写作 | $4.99 | [#](http://www.macworld.com/article/1166079/ommwriter_dana_helps_you_focus_when_writing.html)
<a href="#Byword" name="Byword">★</a>★★☆  | [Byword] | 写博客App，支持Markdown语法 | $9.99 | [#](http://macreview.com/2013/02/keycard-review/)
<a href="#Parallels-Desktop" name="Parallels-Desktop">★</a>★★☆  | [Parallels Desktop] | 虚拟机 | $79.99 | [#](http://www.macworld.com/article/2010694/review-parallels-desktop-8-vs-vmware-fusion-5.html)
<a href="#Proxifier" name="Proxifier">★</a>★★☆  | [Proxifier] | 单App，规则代理工具 | $39.95 | [#](http://download.cnet.com/Proxifier/3000-2155_4-147076.html)
<a href="#Default-Folder-X" name="Default-Folder-X">★</a>★★☆  | [Default Folder X] | 快速定位/选择常用文件夹 | $34.94 | [#](http://mac.appstorm.net/reviews/productivity-review/default-folder-x-browse-file-dialogs-at-lightning-speed/)
<a href="#GhostTile" name="GhostTile">★</a>★★☆  | [GhostTile] | 隐藏 Dock 上的图标/进程 | $9.99 | [#](http://www.appinn.com/ghosttile-for-osx/)
<a href="#Growl" name="Growl">★</a>★★☆  | [Growl] | 消息提醒，原生提醒的鼻祖 | $3.99 | [#](http://mac.appstorm.net/reviews/utilities/meet-the-new-growl-improved-functionality-but-at-a-price/)
<a href="#iPack" name="iPack">★</a>★★☆  | [iPack] | 压缩/解压工具，兼容 Win 乱码问题 | $1.99 | [#](http://www.zhihu.com/question/20383279)
<a href="#Keka" name="Keka">★</a>★★☆  | [Keka] | 压缩/解压工具 | $1.99 | [#](http://www.engadget.com/2011/12/06/daily-mac-app-keka/)
<a href="#Quiver" name="Quiver">★</a>★★☆   | [Quiver](http://happenapps.com/#quiver) | 程序员的记事本 | $9.99 | [#](http://happenapps.com/#quiver)
<a href="#Aperture" name="Aperture">★</a>★★☆  | [Aperture] | 专业的摄影相关软件 | $79.99 | [#](http://www.digitalcameraworld.com/2013/01/28/apple-aperture-3-4-3-review/)
<a href="#Keycard" name="Keycard">★</a>★★☆  | [Keycard] | 蓝牙设备锁屏，人走屏锁 | $6.99 | [#](http://macreview.com/2013/02/keycard-review/)
<a href="#Geekbench" name="Geekbench">★</a>★★☆  | [Geekbench] | 性能测试、硬件跑分 | $9.99 | [#](http://www.macrumors.com/2013/08/16/geekbench-3-with-15-new-benchmark-tests-released-for-mac-ios-and-more/)
<a href="#LockScreen" name="LockScreen">★</a>★★   | [LockScreen] | iOS风格锁屏、触摸板解锁 | $1.99 | [#](https://www.youtube.com/watch?v=aFpbSGasq2A)
<a href="#DaisyDisk" name="DaisyDisk">★</a>★★   | [DaisyDisk] | 磁盘容量占用分布一目了然 | $9.95 | [#](http://mac.appstorm.net/reviews/utilities/daisydisk-3-beta-is-here-with-a-revamped-interface-and-new-tools/)
<a href="#Gemini" name="Gemini">★</a>★★   | [Gemini] | 重复文件查找删除 | $9.99 | [#](http://www.macworld.com/article/1167669/gemini_finds_and_removes_your_duplicate_files.html)
<a href="#plup" name="plup">★</a>★★   | [plup] | 新闻阅读器 | $9.99 | [#](http://mac.appstorm.net/reviews/internet-reviews/pulp-an-innovative-way-to-read-the-news-on-your-mac/)
<a href="#Readkit" name="Readkit">★</a>★★   | [Readkit] | RSS客户端，支持feedly/pocket等服务  | ￥45 | [#](http://geekbeat.tv/review-readkit-for-os-x/)
<a href="#Reeder" name="Reeder">★</a>★★   | [Reeder] | 简洁强大的 RSS 订阅器 Mac 版，支持feedbin/feedly/readability等  | ￥68 | [#](http://reederapp.com/mac/)
<a href="#Play-by-Play" name="Play-by-Play">★</a>★★   | [Play by Play] | Dribbble 客户端 | $4.99 | [#](http://mac.appstorm.net/general/dribbble-on-your-desktop-with-play-by-play/)
<a href="#Scrivener" name="Scrivener">★</a>★★   | [Scrivener] | 专业写作工具 | $45 | [#](http://mac.appstorm.net/reviews/office-review/scrivener-a-writers-best-friend/)
<a href="#OmniOutliner" name="OmniOutliner">★</a>★★   | [OmniOutliner] | 写PPT、文档的好帮手 | $39.99 | [#](http://www.lifehack.org/articles/technology/30-days-with-omnioutliner-professional.html)
<a href="#Ulysses" name="Ulysses">★</a>★★   | [Ulysses] | 专业文本编辑工具，支持 Markdown | $44.99 | [#](http://mac.appstorm.net/reviews/productivity-review/ulysses-iii-a-markdown-writing-app-like-no-other/)
<a href="#iExplorer" name="iExplorer">★</a>★★   | [iExplorer] | 管理iOS设备 | $34.99 | [#](http://www.techrepublic.com/blog/windows-and-office/review-get-direct-access-to-your-iphones-files-with-iexplorer/)
<a href="#Promotee" name="Promotee">★</a>★★   | [Promotee] | Apps官网素材，设备更新还算即时 | $4.99 | [#](http://5key.net/post/promotee-for-mac/)
<a href="#Overflow" name="Overflow">★</a>★★   | [Overflow] | 归类摆放 App Icon | $14.95 | [#](http://www.macworld.com/article/1060201/overflow.html)
<a href="#Instacast" name="Instacast">★</a>★★   | [Instacast] | 出色的 Podcast 应用 | $20 | [#](http://aoxuis.me/posts/2013/06/18/instacast-for-mac)
<a href="#Picatext" name="Picatext">★</a>★★   | [Picatext] | 简单易用的 OCR 软件 | $3.99 | [#](http://mac.appstorm.net/reviews/utilities/picatext-an-attempt-at-ocr-on-the-mac/)
<a href="#RescueTime" name="RescueTime">★</a>★★   | [RescueTime] | 时间管理跟踪分析 | $72/y | [#](http://mac.appstorm.net/reviews/office-review/rescuetime-what-have-you-been-up-to/)
<a href="#Instashare" name="Instashare">★</a>★★   | [Instashare] | 基于 蓝牙/WiFi 文件互传(iOS/Mac)  | $2.99 | [#](http://www.imore.com/instashare-iphone-and-ipad-review)
<a href="#WiFi-Explorer" name="WiFi-Explorer">★</a>★★   | [WiFi Explorer] | 深度解读身边 WiFi 信号，了如指掌 | $2.99 | [#](http://mac.appstorm.net/reviews/utilities/wifi-explorer-the-wireless-swiss-army-knife/)
<a href="#WiFi-Scanner" name="WiFi-Scanner">★</a>★★   | [WiFi Scanner] | 同上，另一款 WiFi 工具 | $0.99 | [#](http://download.cnet.com/WiFi-Scanner/3000-18508_4-75017924.html)
<a href="#Moneywiz" name="Moneywiz">★</a>★★   | [Moneywiz] | 记账软件，支持 iOS 平台 | $24.99 | [#](http://mac.appstorm.net/reviews/productivity-review/moneywiz-simple-yet-powerful-mac-money-management/)
<a href="#Calcbot" name="Calcbot">★</a>★★   | [Calcbot] | 计算器，可单位换算、实时汇率转换 | $24.99 | [#](http://www.imore.com/calcbot-mac-calculator-unit-converter-flare)
<a href="#Paste" name="Paste">★</a>★★   | [Paste] | 高颜值的剪贴板工具 | $5.99 | [#](http://sspai.com/t/7421)
<a href="#Unclutter" name="Unclutter">★★</a>★   | [Unclutter] | 存储剪贴板内容，临时文件及笔记 | ￥40 | [#](https://unclutterapp.com)
<a href="#Synergy" name="Synergy">★★</a>★   | [Synergy] | 全平台鼠标键盘共享软件 | $19 | [#](https://symless.com/synergy)
<a href="#One" name="One">★</a>★☆   | [One](https://itunes.apple.com/cn/app/yi-lan/id941552500?mt=12) | 一览要闻 | ￥6 | [#](https://itunes.apple.com/cn/app/yi-lan/id941552500?mt=12)

#### 1.2 开发类

评分   | 名称  | 功能简述 | 单价 | 测评
----- | ----- | ------ | ----- | -----
<a href="#Dash" name="Dash">★</a>★★★★ | [Dash] | 全语言文档手册速查 | $19.99 | [#](http://brettterpstra.com/2013/04/26/mac-app-review-dash-for-developers/)
<a href="#xScope" name="xScope">★</a>★★★★ | [xScope] | 8 合一开发标尺神器 | $29.99 | [#](http://mac.appstorm.net/general/xscope-3-big-improvements-to-the-designers-best-friend/)
<a href="#Kaleidoscope" name="Kaleidoscope">★</a>★★★☆ | [Kaleidoscope] | 精美强大的 Diff 对比工具 | $69.99 | [#](http://mac.appstorm.net/reviews/utilities/easily-compare-file-versions-with-kaleidoscope/)
<a href="#MAMP-PRO" name="MAMP-PRO">★</a>★★★☆ | [MAMP PRO] | PHP+Mysql 开发集成环境，本地站点 | $59 | [#](http://mac.appstorm.net/reviews/internet-reviews/running-a-local-server-with-mamp/)
<a href="#CodeRunner" name="CodeRunner">★</a>★★★☆ | [CodeRunner] | 各编程语言快速测试集成环境 | $9.99 | [#](http://brettterpstra.com/2011/10/28/app-review-coderunner/)
<a href="#Charles" name="Charles">★</a>★★★☆ | [Charles] | 抓包代理调试工具、类 Fiddler | $50 | [#](http://www.99css.com/1272)
<a href="#LiveReload" name="LiveReload">★</a>★★★☆ | [LiveReload] | 调试工具：浏览器自刷新、前端代码编译等 | $6.99 | [#](http://brettterpstra.com/2011/12/02/app-review-livereload/)
<a href="#CodeKit" name="CodeKit">★</a>★★★☆ | [CodeKit] | 前端项目编译工具合集 | $28 | [#](http://www.stalecoffee.com/2012/12/codekit-app-review/)
<a href="#Sublime-Text" name="Sublime-Text">★</a>★★★  | [Sublime Text] | 编辑器 | $80/Free | [#](http://mac.appstorm.net/roundups/web-dev/the-best-code-editors-for-your-mac-in-2013/)
<a href="#Slack" name="Slack">★</a>★★★  | [Slack] | 团队合作沟通工具 | Free | [#](http://mac.appstorm.net/reviews/productivity-review/slack-team-collaboration-made-simple/)
<a href="#Intellij-IDEA" name="Intellij-IDEA">★</a>★★★  | [Intellij IDEA] | IDE(集成开发环境) | $199 | [#](http://development-software.findthebest.com/l/19/IntelliJ-IDEA)
<a href="#Atom" name="Atom">★</a>★★★  | [Atom] | Github 自家出的编辑器 | Free | [#](http://www.techspot.com/news/55845-github-unveils-atom-text-editor-for-developers.html)
<a href="#Brackets" name="Brackets">★</a>★★★  | [Brackets] | Adobe 出的开源编辑器 | Free | [#](http://www.iplaysoft.com/brackets.html)
<a href="#Coda" name="Coda">★</a>★★★  | [Coda] | 编辑器 | $74.99 | [#](http://mac.appstorm.net/reviews/web-dev-review/coda-2-its-here-and-its-awesome/)
<a href="#Textastic" name="Textastic">★</a>★★★  | [Textastic] | 编辑器，iOS 同步/友好 | $8.99 | [#](http://mac.appstorm.net/reviews/web-dev-review/textastic-the-ios-code-editor-to-beat-now-on-the-mac/)
<a href="#Tower" name="Tower">★</a>★★★  | [Tower] | Git 客户端，支持GitHub、Bitbucket等 | $59 | [#](http://mac.appstorm.net/reviews/utilities/tower-gits-it-done/)
<a href="#Versions" name="Versions">★</a>★★★  | [Versions] | SVN 版本控制工具 | $59 | [#](http://stackoverflow.com/questions/899/best-subversion-client-for-mac-os)
<a href="#Cornerstone" name="Cornerstone">★</a>★★★  | [Cornerstone] | 同样是 SVN 管理工具 | $59 | [#](http://www.taylorjasko.com/2011/02/cornerstone-2-review-the-best-version-control-system/)
<a href="#Paw" name="Paw">★</a>★★★  | [Paw] | HTTP、REST客户端 | $29.99 | [#](https://luckymarmot.com/paw)
<a href="#ColorSchemer" name="ColorSchemer">★</a>★★★  | [ColorSchemer] | 专业的配色、调色软件 | $49.99 | [#](http://mac.appstorm.net/general/colorschemer-studio-2-instant-color-schemes/)
<a href="#Sketch" name="Sketch">★</a>★★★  | [Sketch] | 图像处理设计工具，获2012苹果设计大奖 | $99 | [#](http://mac.appstorm.net/general/sketch-2-a-simple-powerful-vector-graphics-app/)
<a href="#Sparkbox" name="Sparkbox">★</a>★★   | [Sparkbox] | 图片、设计素材收集管理 | $19.99 | [#](http://mac.appstorm.net/reviews/productivity-review/keep-your-digital-inspiration-organized-with-sparkbox/)
<a href="#Frank-DeLoupe" name="Frank-DeLoupe">★</a>★★   | [Frank DeLoupe] | 精美拾色器、可Photoshop联动 | $0.99 | [#](http://mac.appstorm.net/general/frank-deloupe-your-color-picking-friend/)
<a href="#ColorSnapper" name="ColorSnapper">★</a>★★   | [ColorSnapper] | 屏幕取色，只做一件事，做到极致 | $4.99 | [#](http://mac.appstorm.net/reviews/utilities/colorsnapper-a-slick-simple-color-picker-for-the-mac/)
<a href="#CodeBox" name="CodeBox">★</a>★★   | [CodeBox] | 代码片段收集 | $9.99 | [#](http://mac.appstorm.net/reviews/utilities/codebox-manage-your-snippets-effectively-and-efficiently/)
<a href="#Slicy" name="Slicy">★</a>★★   | [Slicy] | 快速切图 PSD->IMG，支持@2x | $29 | [#](http://mac.appstorm.net/general/layer-cake-exporting-from-photoshop-was-never-this-tasty/)

#### 1.3 服务订阅类

评分   | 名称  | 推荐理由 | 单价 | 详细
----- | ----- | ------ | ----- | -----
<a href="#MacUpdate-Desktop" name="MacUpdate-Desktop">★</a>★★☆  | [MacUpdate Desktop] | 管理/更新/下载App，跟踪优惠信息 | $29.99/year | [#](http://www.macworld.com/article/1143823/macupdate_desktop_5.html)
<a href="#Spotify-Pro" name="Spotify-Pro">★</a>★★   | [Spotify Pro] | 音乐服务 | $9.99/month | [#](http://www.cultofmac.com/104703/spotify-is-everything-that-itunes-in-the-cloud-should-be-review/)
<a href="#Rdio-Pro" name="Rdio-Pro">★</a>★★   | [Rdio Pro] | 音乐服务 | $9.99/month | [#](http://www.rdio.com/features/)
<a href="#iTunes-Match" name="iTunes-Match">★</a>★★   | [iTunes Match] | iTunes 音乐服务 | $24.99/year | [#](http://www.maclife.com/article/reviews/itunes_match_review)
<a href="#Google-Music" name="Google-Music">★</a>★★   | [Google Music] | Google 音乐服务 | $9.99/month | [#](https://play.google.com/about/music/)
<a href="#Evernote-Pro" name="Evernote-Pro">★</a>★★   | [Evernote Pro] | 笔记服务 | $45/year | [#](http://www.pcworld.com/article/2033479/become-an-evernote-power-user-10-must-know-tips.html)
<a href="#Github-Pro" name="Github-Pro">★</a>★★   | [Github Pro] | 基于 Git 的代码托管服务 | $7/month | [#](https://github.com/features)
<a href="#Dropbox-Pro" name="Dropbox-Pro">★</a>★★   | [Dropbox Pro] | 云存储/分享服务 | $9.99/month | [#](https://www.dropbox.com/upgrade)
<a href="#Droplr-Pro" name="Droplr-Pro">★</a>★★   | [Droplr Pro] | 分享文件，支持自定义短链和统计 | $30/year | [#](http://web.appstorm.net/reviews/storage-reviews/i-switched-to-droplr-pro-heres-why/)
<a href="#CloudApp-Pro" name="CloudApp-Pro">★</a>★★   | [CloudApp Pro] | 云存储/分享服务 | $45/year | [#](http://store.getcloudapp.com/)

#### 2.1 不断更新中...

## 购买建议

* 建议尽量选择`打折促销`时购入，可在 [数码荔枝](https://partner.lizhi.io/mactips/cp) 这类正版软件销售平台购入
* `家庭装促销包授权`适合家里人一起使用
* 关注和参与`个人`或`集体`组织的团购`活动`，如：[BundleHunt] 家的促销包活动
* 选择购买`Mac App Store`的版本通常升级后续版本会 Free
* 部分 Apps **只有**`Mac App Store` 版会有`iCloud`同步功能
* 如果官方有非沙盒版，建议不要选择`Mac App Store`的阉割版，购入原版

## macOS App 优惠&促销信息媒体

* [数码荔枝](https://store.lizhi.io/site/index/cid/skdrzvap)
* [StackSocial](https://stacksocial.com/?aid=a-9j496mje)
* [BundleHunt](https://bundlehunt.com/?ap_id=macosx)
* [MacUpdate](http://www.macupdate.com/)
* [AppShopper](http://appshopper.com/)
* [V2EX MacOS](http://v2ex.com/go/macosx)
* [hzlzh/Best-App](https://github.com/hzlzh/Best-App)
* [“反”斗限免](http://free.apprcn.com/)
* [Macheist](https://macheist.com/)

## 关于

#### 评分说明：

评分   | 推荐度
----- | -----
★★★★★ | 必装神器
★★★★☆ | 十分出色
★★★★  | 值得购入
★★★☆  | 亮点突出
★★★   | 同类出众

*注1：排名怎么可能不分先后*  
*注2：此列表客观公正，绝无广告或推广*  
*注3：此列表维护有个人感情色彩，如遇不适者，欢迎`Fork`一份进行修改*  

#### 支持正版：

软件开发者和作家一样，有的只是代码和文字。
在条件允许的情况下，请支持正版，有了良好的生态环境，App 开发者们会做出更多好玩的东西。

#### 感谢所有参与推荐的朋友

本推荐 List 会不断更新维护，会有更多分类和利器加入推荐。
感谢此处\[[收集&提交页]\]参与提交和讨论的朋友们

[<< 查看总目录]

#### License

Released under [MIT] LICENSE

#### 扩展阅读

@hzlzh 创立了一个微信公众号：[MacTips](http://mactips.io/)  
 -- 专注于分享 Mac 使用经验和技巧，打造 Mac 神兵利器。  --
![MacTips](http://ww4.sinaimg.cn/large/644eac00gw1evn89qmu5aj20by0byaav.jpg)

[<< 查看总目录]: ./README.md
[issue]: https://github.com/hzlzh/Best-App/issues
[收集&提交页]: https://github.com/hzlzh/Best-App/issues
[反馈]: https://github.com/hzlzh/Best-App/issues/new
[MIT]: https://rem.mit-license.org/

[Alfred]: https://www.macupdate.com/app/mac/34344/alfred
[MenubarX]: https://menubarx.app/
[1Password]: https://1password.com/features
[iStat Menus]: https://bjango.com/mac/istatmenus/
[Keyboard Maestro]: http://www.keyboardmaestro.com/main/
[Little Snitch]: https://www.obdev.at/products/littlesnitch/
[PopClip]: http://pilotmoon.com/popclip/
[Clear]: http://realmacsoftware.com/clear/
[Versions]: http://versionsapp.com/
[Bartender]: https://www.macbartender.com/
[BreakTime]: http://breaktimeapp.com/
[Timing]: http://timingapp.com/
[Day One]: http://dayoneapp.com/
[Should I Sleep]: http://www.mrmilk.com.br/
[CleanMyMac]: http://macpaw.com/cleanmymac
[LockScreen]: https://itunes.apple.com/us/app/lock-screen-2/id445423011?mt=12
[Moom]: http://manytricks.com/moom/
[SteerMouse]: http://plentycom.jp/en/steermouse/index.html
[OmmWriter]: http://www.ommwriter.com/
[SaneDesk]: http://www.sanedeskapp.com/
[Entropy]: http://www.eigenlogik.com/entropy/
[Parallels Desktop]: http://www.parallels.com/products/desktop/
[Proxifier]: http://www.proxifier.com/
[ColorSchemer]: http://www.colorschemer.com/
[DaisyDisk]: https://daisydiskapp.com/
[iExplorer]: https://www.macroplant.com/iexplorer/
[Growl]: http://growl.info/
[Frank DeLoupe]: http://jumpzero.com/frank/
[Fantastical]: http://flexibits.com/fantastical
[aText]: http://www.trankynam.com/atext/
[Dash]: https://kapeli.com/dash
[ForkLift]: http://www.binarynights.com/
[CodeRunner]: https://coderunnerapp.com
[Charles]: http://www.charlesproxy.com/
[Scrapbook]: http://www.ariessolutions.de/sites/scrapbook/
[ScreenFlow]: http://www.telestream.net/screenflow/
[Sparkbox]: http://www.icyblaze.com/sparkbox/
[Tweetbot]: http://tapbots.com/tweetbot/mac/
[Xee]: http://xee.c3.cx/
[PhotoDesk]: http://www.photodesk-app.com/
[Pixelmator]: http://www.pixelmator.com/
[xScope]: http://xscopeapp.com/
[plup]: http://www.acrylicapps.com/pulp/
[Things]: https://culturedcode.com/things/
[Aperture]: http://www.apple.com/hk/en/osx/photos/
[jitouch]: http://www.jitouch.com/
[OmniFocus]: https://www.omnigroup.com/products/omnifocus/
[Devonthink Pro]: http://www.devontechnologies.com/products/devonthink/overview.html
[TextExpander]: https://smilesoftware.com/TextExpander/index.html
[CodeBox]: http://www.codeboxapp.com
[Slicy]: http://macrabbit.com/slicy/
[Gemini]: http://macpaw.com/gemini
[Keycard]: http://www.appuous.com/products/mac/keycard.html
[Geekbench]: http://browser.primatelabs.com/mac-benchmarks
[Noizio]: http://noiz.io/
[iPack]: http://ipackapp.com/
[LiveReload]: http://livereload.com/‎
[Kaleidoscope]: http://www.kaleidoscopeapp.com/
[Moneywiz]: http://moneywizapp.com/
[MAMP PRO]: https://www.mamp.info/
[Play by Play]: http://playbyplayapp.com/
[Intellij IDEA]: http://www.jetbrains.com/idea/
[Sublime Text]: http://www.sublimetext.com/
[Slack]: https://slack.com
[Short Menu]: https://floschliep.com/short-menu-mac/
[Picatext]: http://www.picatext.com/
[BetterSnap Tool]: https://www.boastr.net/
[KeyCue]: http://www.ergonis.com/products/keycue/
[PaintCode]: http://www.paintcodeapp.com/
[Airmail]: http://airmailapp.com/
[CodeKit]: http://incident57.com/codekit/
[Tower]: https://www.git-tower.com/
[Instacast]: http://vemedio.com/products/instacast-mac
[Sketch]: http://www.sketchapp.com/
[ColorSnapper]: http://colorsnapper.com
[Scrivener]: http://www.literatureandlatte.com/
[Ulysses]: http://www.ulyssesapp.com/
[OmniGraffle]: https://www.omnigroup.com/omnigraffle
[Promotee]: http://www.netwalkapps.com/app/promotee
[Spotify Pro]: https://www.spotify.com/
[Droplr Pro]: https://droplr.com/
[DEFAULT FOLDER X]: http://www.stclairsoft.com/DefaultFolderX/
[GhostTile]: http://ghosttile.kernelpanic.im/
[MacUpdate Desktop]: https://www.macupdate.com/
[OmniOutliner]: https://www.omnigroup.com/omnioutliner
[Calcbot]: http://tapbots.com/calcbot/
[Ember]: https://www.realmacsoftware.com/ember
[Inboard]: http://www.inboardapp.com
[Coda]: https://panic.com/coda/
[Hazel]: https://www.noodlesoft.com/
[Paw]: https://luckymarmot.com/paw
[GhostNote]: http://www.ghostnoteapp.com/
[Byword]: https://metaclassy.com/
[Cornerstone]: https://www.zennaware.com/cornerstone/
[Evernote Pro]: https://evernote.com/
[Overflow]: http://stuntsoftware.com/overflow/
[iTunes Match]: http://www.apple.com/itunes/itunes-match/
[Textastic]: http://www.textasticapp.com/
[Dropbox Pro]: https://www.dropbox.com/pricing
[Github Pro]: https://github.com/features
[CloudApp Pro]: http://store.getcloudapp.com/
[Readkit]: http://readkitapp.com/
[Rdio Pro]: http://www.rdio.com/
[Google Music]: https://play.google.com/about/music/
[RescueTime]: https://www.rescuetime.com/plans
[Instashare]: http://instashareapp.com/
[Writer Pro]: https://ia.net/writer
[WiFi Explorer]: https://www.adriangranados.com/
[WiFi Scanner]: https://itunes.apple.com/us/app/wifi-scanner/id411680127?mt=12
[Atom]: https://atom.io/
[Brackets]:http://brackets.io
[Keka]: http://www.kekaosx.com/
[mou.li]: http://mou.li/
[Paste]: http://pasteapp.me
[reeder]: http://reederapp.com/mac/
[Unclutter]: https://unclutterapp.com
[Magnet]: http://magnet.crowdcafe.com
[Synergy]: https://symless.com/synergy
# AndroidLibs

收集Android开发中优秀的开源组件库，方便大家查询，欢迎 PR 和 star~

---

### 目录 Catalogue


- [列表List](https://github.com/XXApple/AndroidLibs/tree/master/%E5%88%97%E8%A1%A8List) 
- [动画Animation](https://github.com/XXApple/AndroidLibs/tree/master/%E5%8A%A8%E7%94%BBAnimation)
- [图标Icon](https://github.com/XXApple/AndroidLibs/tree/master/%E5%9B%BE%E6%A0%87Icon)
- [图片框架Image](https://github.com/XXApple/AndroidLibs/tree/master/%E5%9B%BE%E7%89%87%E6%A1%86%E6%9E%B6Image)
- [图表Chart](https://github.com/XXApple/AndroidLibs/tree/master/%E5%9B%BE%E8%A1%A8Chart)
- [完整开源项目Project](https://github.com/XXApple/AndroidLibs/tree/master/%E5%AE%8C%E6%95%B4%E5%BC%80%E6%BA%90%E9%A1%B9%E7%9B%AEProject)
- [布局Layout](https://github.com/XXApple/AndroidLibs/tree/master/%E5%B8%83%E5%B1%80Layout)
- [开发框架Framework](https://github.com/XXApple/AndroidLibs/tree/master/%E5%BC%80%E5%8F%91%E6%A1%86%E6%9E%B6Framework)
- [弹框Dialog](https://github.com/XXApple/AndroidLibs/tree/master/%E5%BC%B9%E6%A1%86Dialog)
- [按钮Button](https://github.com/XXApple/AndroidLibs/tree/master/%E6%8C%89%E9%92%AEButton)
- [文本Label](https://github.com/XXApple/AndroidLibs/tree/master/%E6%96%87%E6%9C%ACLabel)
- [特效Effect](https://github.com/XXApple/AndroidLibs/tree/master/%E7%89%B9%E6%95%88Effect)
- [网络框架Network](https://github.com/XXApple/AndroidLibs/tree/master/%E7%BD%91%E7%BB%9C%E6%A1%86%E6%9E%B6Network)
- [自定义控件Custom](https://github.com/XXApple/AndroidLibs/tree/master/%E8%87%AA%E5%AE%9A%E4%B9%89%E6%8E%A7%E4%BB%B6Custom) (其他分类找不到的，大部分都在这个分类里面)
- [菜单Menu](https://github.com/XXApple/AndroidLibs/tree/master/%E8%8F%9C%E5%8D%95Menu)
- [辅助工具类Utils](https://github.com/XXApple/AndroidLibs/tree/master/%E8%BE%85%E5%8A%A9%E5%B7%A5%E5%85%B7%E7%B1%BBUtils)
- [进度条Progressbar](https://github.com/XXApple/AndroidLibs/tree/master/%E8%BF%9B%E5%BA%A6%E6%9D%A1Progressbar)
- [音视频Audio_Video](https://github.com/XXApple/AndroidLibs/tree/master/%E9%9F%B3%E8%A7%86%E9%A2%91Audio_Video)
- [面试Interview](https://github.com/XXApple/AndroidLibs/tree/master/%E9%9D%A2%E8%AF%95Interview)
- [RxJava](https://github.com/XXApple/AndroidLibs/tree/master/RxJava)
- [AI/VI](https://github.com/XXApple/AndroidLibs/tree/master/AI_VI)
- [Gradle](https://github.com/XXApple/AndroidLibs/tree/master/Gradle)
- [ReactNative](https://github.com/XXApple/AndroidLibs/tree/master/React_Native)
- [Kotlin](https://github.com/XXApple/AndroidLibs/tree/master/Kotlin)
- :fire:[Flutter](https://github.com/XXApple/AndroidLibs/tree/master/Flutter)
- :fire:[Jetpack_Compose](https://github.com/XXApple/AndroidLibs/tree/master/Jetpack_Compose)


---

For better Android developing~

Please Pull Request~

希望各位能帮忙添加一些优秀的内容，为开源做一份贡献~ ^ ^ 
快来PR吧~

ad:  阿里巴巴淘系技术部招客户端开发、前端开发、后端JAVA开发、算法工程开发，欢迎投递简历 devislee.lb@alibaba-inc.com（封羽）

---


Thanks to :

- http://gank.io/
- https://github.com/wasabeef/awesome-android-ui
- http://www.jcodecraeer.com/

