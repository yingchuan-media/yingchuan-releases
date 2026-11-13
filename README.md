<p align="center"><img src="assets/brand-icon.svg" width="88" alt="映川"></p>

# 映川 · 客户端下载

映川（YingChuan）支持站源浏览、搜索、播放、追剧、历史与下载，也可由 Windows 客户端向局域网内的手机浏览器提供访问。当前统一采用映川 V2A 品牌；本页截图来自用户提供的历史客户端，版本以各自发布记录为准。

| 仓库 | 用途 |
| --- | --- |
| [站源订阅](https://github.com/yingchuan-media/yingchuan-sources) | 四类可选站源配置及检测结果 |
| 本仓库 | 安装包、功能说明、实际截图与公开反馈 |

## 下载

[当前发布](https://github.com/yingchuan-media/yingchuan-releases/releases)。0.1.4 的 Android 三架构、Windows x64、macOS ARM64 和 iOS 统一放在下方同一个发布页。macOS 使用 ad-hoc 签名且未经公证；iOS 提供未签名 IPA／应用 ZIP，需自行签名后安装。普通 Android 手机优先选择 arm64-v8a，32 位 ARM 选择 armeabi-v7a，x86_64 设备选择 x86_64。

<!-- release-stable:start -->

### 正式版 0.1.4

[版本与更新说明](https://github.com/yingchuan-media/yingchuan-releases/releases/tag/app-v0.1.4-unified) · 提交 `f1969f8bc7bfbf943e2444dfc18108a9b883d811` · 云端运行 #43205737464，尝试 1

| 文件 | 下载 |
| --- | --- |
| BUILD_METADATA.json | [下载](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.4-unified/BUILD_METADATA.json) |
| SHA256SUMS.txt | [下载](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.4-unified/SHA256SUMS.txt) |
| yingchuan-0.1.4-arm64-v8a.apk | [下载](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.4-unified/yingchuan-0.1.4-arm64-v8a.apk) |
| yingchuan-0.1.4-armeabi-v7a.apk | [下载](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.4-unified/yingchuan-0.1.4-armeabi-v7a.apk) |
| yingchuan-0.1.4-ios-unsigned-app.zip | [下载](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.4-unified/yingchuan-0.1.4-ios-unsigned-app.zip) |
| yingchuan-0.1.4-ios-unsigned.ipa | [下载](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.4-unified/yingchuan-0.1.4-ios-unsigned.ipa) |
| yingchuan-0.1.4-macos-arm64.dmg | [下载](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.4-unified/yingchuan-0.1.4-macos-arm64.dmg) |
| yingchuan-0.1.4-macos-arm64.zip | [下载](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.4-unified/yingchuan-0.1.4-macos-arm64.zip) |
| yingchuan-0.1.4-windows-x64.exe | [下载](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.4-unified/yingchuan-0.1.4-windows-x64.exe) |
| yingchuan-0.1.4-windows-x64.zip | [下载](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.4-unified/yingchuan-0.1.4-windows-x64.zip) |
| yingchuan-0.1.4-x86_64.apk | [下载](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.4-unified/yingchuan-0.1.4-x86_64.apk) |

#### 功能改动

- 红果优先使用官方单集播放协议，补齐官方系列剧／合集、动态筛选和弹幕 cursor 分页，保留权限与 Windows 播放边界。
- 历史与追剧页接入 B站云端记录，统一已加载记录搜索、分页和本地／云端显示；本地追剧统一为一个列表。
- 新增产品官网与跨端介绍、启动投影及滚动动效。
- 云端统一构建 Android 三架构、Windows x64、macOS ARM64 和 iOS；Apple 产物独立发布，macOS 使用 ad-hoc 签名且未经公证，iOS 提供需自行签名的未签名构建。

#### Bug 修复

- 修复奈飞同日重名分集导致详情失败、影视2旧协议排除重名线路，以及通用采集重排后的分集和画质错配；不跨线路猜配。
- 移除红果第三方备用取流，保留进程内注册会话及明确拒绝后停止的策略；取消和撤权后的迟到响应不再提交。
- 修复本地／云端记录切换时布局跳动、背景和卡片不一致、工具缺失及封面方向猜测，不将云端进度写入本地记录。
- 修复官网首次访问启动动画前正文闪现，保留跳过、减少动态效果与失败后的正文回退。
- 接入 macOS 包内 Go 核心与最低系统版本校验，补齐 iOS 全新构建所需的局域网页面资源和未签名产物验证。

发布整理：本页将同批 0.1.4 云端产物汇总至一个发布，没有重新编译。源码提交 f1969f8bc7bfbf943e2444dfc18108a9b883d811，构建运行 #43205737464，尝试 1。共九个安装包及两份共用清单；原始两份构建元数据及其摘要保存在聚合元数据中。

安装方式：原始 Actions 运行因跨仓同步 HTTP 401，整体结论仍为失败，未满足客户端可信自动安装条件。请从本页手动下载、安装；保留固定 Android 证书和现有校验条件。macOS 为 ad-hoc 签名且未经公证，iOS 为需自行签名的未签名包。构建和包校验不代表全功能或物理设备验收。

<!-- release-stable:end -->

<!-- release-preview:start -->

### 预览版

当前没有单独的预览发布。

<!-- release-preview:end -->

## 功能

| 功能 | 使用说明 |
| --- | --- |
| 浏览与搜索 | 按站源及实际分类浏览内容，使用关键词搜索、联合搜索、筛选和排序；内置 B站、红果、影视、影视2、奈飞入口 |
| 应用内播放 | 查看详情、选集播放、切换实际可用的画质和线路，支持进度定位、倍速、音量、画面比例、全屏及 Windows 小窗 |
| 追剧与历史 | 管理想看、在看、已看等追剧状态，通过观看历史继续播放，支持搜索和批量管理 |
| 下载与离线 | 选择剧集和实际可下载画质，管理下载队列、暂停、继续、取消和重试，查看下载记录及本地媒体 |
| 字幕与弹幕 | 选择媒体提供的字幕或导入本地字幕；支持已适配站源的弹幕及显示、字号、密度等设置，具体能力随来源而异 |
| 局域网浏览器 | 在客户端开启网页访问，其他设备使用浏览器完成配对后访问；站源请求与媒体处理由主机客户端承担 |
| 主题与布局 | 浅色、深色主题及横竖布局；宽屏使用侧边导航，竖屏提供发现、追剧、历史、设置四个入口，下载位于设置中 |
| 播放诊断 | 查看媒体信息、缓冲和读取状态，并在更多诊断中查看当前播放请求地址；可获得的指标取决于平台和后端 |

可用内容与画质取决于来源实际返回结果，以及账号、会员、地区和媒体权限。客户端不提供内容授权，不绕过登录、付费或加密保护。

## 实际截图

以下为用户提供的实际客户端截图，依次展示宽屏首页、播放器、下载管理、深色竖屏、浅色竖屏与设置。保留原图，未作界面重绘、裁剪或效果合成；尺寸和文件摘要见[截图信息](screenshots/metadata.json)。

### 宽屏浏览

![深色宽屏首页](screenshots/desktop-home.png)

### 播放器

![实际客户端播放器](screenshots/desktop-player.png)

### 下载管理

![下载管理实际页面](screenshots/downloads.png)

### 竖屏与主题

<table>
  <tr>
    <th>深色竖屏</th>
    <th>浅色竖屏</th>
    <th>设置</th>
  </tr>
  <tr>
    <td><img src="screenshots/portrait-dark.png" width="260" alt="竖屏深色主题"></td>
    <td><img src="screenshots/portrait-home.png" width="260" alt="竖屏浅色主题"></td>
    <td><img src="screenshots/portrait-settings.png" width="260" alt="竖屏设置及下载入口"></td>
  </tr>
</table>

## 开始使用

1. Windows 下载 EXE，或将 ZIP 完整解压后启动；Android 下载对应架构的 APK，按系统提示安装后打开。
2. 在发现页选择站源，浏览分类或搜索内容；选择视频后查看详情、选集并播放。
3. 需要离线观看时，从内容菜单选择下载；竖屏可从设置进入下载管理。
4. 需要用其他设备的浏览器访问时，在设置的数据同步分类开启局域网页面，按客户端显示的地址与配对流程连接。主机客户端需保持运行。

从本仓库发布页或客户端检查更新下载安装包，按实际签名与发布身份选择安装方式。ZIP 中的 `data`、DLL 和其他资源属于运行所需文件，不要只复制其中的 EXE。

## 发布与更新说明

云端构建先在源码仓库发布完整安装包，验证源码标签并逐附件下载校验成功后，再同步本仓库；两边附件字节、版本、签名和说明保持一致。每次说明记录该版本的功能改动与 Bug 修复，公开附件再次下载验证后更新上方对应渠道，保留实际截图；同版本全部平台使用同一发布页和共用清单。

同步失败时保留已成功的源码 Release 和可能的目标草稿，不删除旧发布，不自动覆盖同名标签。提交、PR 或合并不会自动触发构建。历史本地发布按元数据明确标记来源，不能据此推断新的云端流程已经验收。

## 版本与验证

0.1.4 的安装包来自源码提交 `f1969f8bc7bfbf943e2444dfc18108a9b883d811`、GitHub Actions #43205737464，尝试 1。本次将原同批文件汇总至一个 Release，没有重新编译；两仓全部十一附件均逐项下载并核对文件大小和 SHA-256，原始两份构建元数据及摘要保存在聚合元数据中。Android 使用既定固定证书，Windows 提供便携 EXE 和完整运行目录 ZIP。

原构建运行在跨仓同步阶段因 HTTP 401 失败，后续已手动完成发布并更新发布凭据；原运行失败状态保留。本次请手动下载、安装；聚合不改变已有自动安装的校验条件。macOS 未经公证，iOS 需自行签名。

构建、包身份及摘要校验不代表全功能或物理设备验收；全量 Flutter 预检有断言失败及超时，Android／TV、macOS 和 iOS 的物理设备、本版 Windows 安装包运行验收尚未完成。本地验证使用合成资料并禁用站源图片；本页保留的历史截图不能作为本次设备验收证明。

## 问题反馈

可在 [Issues](https://github.com/yingchuan-media/yingchuan-releases/issues) 反馈问题。请提供客户端版本、设备与系统版本、操作步骤、预期结果和实际表现；涉及画面问题时可附截图。

提交前请移除账号、令牌、配对码、个人文件路径和带授权参数的播放地址。第三方组件的许可证随运行包提供。
