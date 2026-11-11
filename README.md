<p align="center"><img src="assets/brand-icon.svg" width="96" alt="映川 · 澄青川流精修 A 图标"></p>

# 映川 · 客户端下载

映川是一款多端视频客户端，提供站源浏览、搜索、播放、追剧、观看历史与下载管理。Windows 客户端也可在局域网内向手机、平板的浏览器提供访问入口。

正式品牌使用澄青川流精修 A（V2A），各平台统一采用深墨双青图标。可编辑[主标识](assets/brand-logo.svg)与[应用图标](assets/brand-icon.svg)随本仓库提供。

本仓库提供映川已发布客户端、功能说明与实际界面截图。安装文件位于 [Releases](https://github.com/yingchuan-media/yingchuan-releases/releases)。

## 下载

**当前版本：0.1.3 · Windows x64 / Android 三架构 · 固定签名预发布**

本次安装包从源码仓库 main 的 `3b1d9b0e2e096203cba6156b3aee241033ca4823` 本地构建，采用映川品牌、安装标识及固定 Android 发布证书。先在源码仓库发布并下载校验，再将相同文件发布到本仓库；仍为预发布版本。

### Windows

| 安装方式 | 下载 | 说明 |
| --- | --- | --- |
| 便携启动器 | [Windows x64 EXE](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.3-local-3b1d9b0e2e09/yingchuan-0.1.3-windows-x64.exe) | 下载后运行，包含完整运行资源 |
| 完整运行目录 | [Windows x64 ZIP](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.3-local-3b1d9b0e2e09/yingchuan-0.1.3-windows-x64.zip) | 全部解压后运行目录中的主程序，保留 DLL、`data` 与其他资源 |
| 文件校验 | [SHA256SUMS.txt](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.3-local-3b1d9b0e2e09/SHA256SUMS.txt) | 核对下载文件是否完整 |
| 构建信息 | [BUILD_METADATA.json](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.3-local-3b1d9b0e2e09/BUILD_METADATA.json) | 查看版本、构建来源与文件摘要 |

### Android

需要 Android 8.0 或更新版本。一般手机优先选择 ARM64；32 位 ARM 设备选择 ARMv7，x86_64 设备或相应模拟器选择 x86_64。

| 架构 | 下载 |
| --- | --- |
| ARM64（arm64-v8a） | [Android ARM64 APK](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.3-local-3b1d9b0e2e09/yingchuan-0.1.3-arm64-v8a.apk) |
| ARMv7（armeabi-v7a） | [Android ARMv7 APK](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.3-local-3b1d9b0e2e09/yingchuan-0.1.3-armeabi-v7a.apk) |
| x86_64 | [Android x86_64 APK](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.3-local-3b1d9b0e2e09/yingchuan-0.1.3-x86_64.apk) |
| 文件校验 | [Android SHA256SUMS.txt](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.3-local-3b1d9b0e2e09/SHA256SUMS.txt) |
| 构建信息 | [Android BUILD_METADATA.json](https://github.com/yingchuan-media/yingchuan-releases/releases/download/app-v0.1.3-local-3b1d9b0e2e09/BUILD_METADATA.json) |

**Android 包使用映川专用固定发布签名，属于预发布版本。** 三个 APK 均使用 Release 模式编译，包名为 `com.yingchuan.yingchuan`，后续正式发布复用同一证书。证书 SHA-256：`89b83acb459659edc357c742e76fdb8ee6f913a5d24877ff3eaf7bfb943470f0`。其他证书签名的旧测试 APK 无法直接覆盖升级，安装前请先备份需要保留的资料。

其他版本见 [Windows 0.1.0](https://github.com/yingchuan-media/yingchuan-releases/releases/tag/windows-v0.1.0) 或[全部发布](https://github.com/yingchuan-media/yingchuan-releases/releases)。iOS 暂无下载包。

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

此处提供的客户端采用本地构建，请从本仓库发布页手动下载更新。ZIP 中的 `data`、DLL 和其他资源属于运行所需文件，不要只复制其中的 EXE。

## 版本与验证

0.1.3 的 Android 三架构 APK、Windows 便携 EXE 和完整运行目录 ZIP 均由本次 main 源码在本机构建，未使用 GitHub Actions。发布附件包含统一的 `BUILD_METADATA.json` 与 `SHA256SUMS.txt`，记录源码、固定证书及各文件实际摘要；两个仓库的同名附件逐字节一致。

Windows 已通过包完整性、x64 PE 与实际版本、更新协议、隔离冷／热启动，以及 EXE 解包和 ZIP 两种运行目录的原生核心、媒体探测、转封装与本地合成视频播放检查。旧品牌程序和重复原生核心库未打入新包。

Android 三个架构分别核验实际固定签名、包名、版本、ABI、必需运行库、ZIP CRC 和局域网页面资源。51 项客户端更新测试通过；发布策略 46 项通过，2 项受 Windows 符号链接权限阻塞。尚未进行 Android 真机安装与播放验收。

本地验证未请求站源图片或真实媒体，未完成全部界面、真实站源、不同显卡驱动与跨设备验收。移动浏览器的物理手势、软键盘和全屏效果仍需设备验证；本页保留的用户实拍截图来自历史版本，不作为本次构建已通过这些场景的证明。

## 问题反馈

可在 [Issues](https://github.com/yingchuan-media/yingchuan-releases/issues) 反馈问题。请提供客户端版本、设备与系统版本、操作步骤、预期结果和实际表现；涉及画面问题时可附截图。

提交前请移除账号、令牌、配对码、个人文件路径和带授权参数的播放地址。第三方组件的许可证随运行包提供。
