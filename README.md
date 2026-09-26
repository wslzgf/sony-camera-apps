<h1 align="center">索尼 PlayMemories 老机型软件合集</h1>

<p align="center">
适用于可安装 PlayMemories 应用的索尼相机（2007–2016 年机型）的<br>
开源软件、工具与汉化项目导航
</p>

---

## 关于本合集

2016 年及更早发布的索尼相机（NEX、A6000/A6300/A6500、A7/A7 II 系列、RX100 早期型号等）内置一个 Android 子系统，可以通过 [Sony-PMCA-RE](https://github.com/ma1co/Sony-PMCA-RE) 安装第三方开源应用。索尼官方应用商店已于 2021 年关闭，本合集汇总目前仍可获取、可安装的社区开源项目。

> **机型判断**：相机菜单中存在 `MENU → 应用程序（Application）` 即支持安装。2016 年底之后发布的机型（A6400、A7 III、A6700 等）固件已签名，无法安装。

## 开始之前：安装工具

所有应用均通过 USB 线由电脑侧工具安装，无需在相机上操作商店：

- **[ma1co/Sony-PMCA-RE](https://github.com/ma1co/Sony-PMCA-RE)** — 索尼相机逆向与应用安装工具。Windows 下载 Releases 中的 `pmca-gui.exe`，运行后选择 **Install app from file** 即可安装 APK。
- 如安装时提示设置区只读，可配合 [ma1co/OpenMemories-Tweak](https://github.com/ma1co/OpenMemories-Tweak) 解锁受保护设置。

**通用安装步骤**：相机菜单 `设置 → USB连接` 改为 **海量存储器** → USB 连接电脑 → 运行 pmca-gui 安装 APK → 完成后关机再开机。

---

## 胶片色彩与模拟

| 项目 | 说明 |
|---|---|
| [**胶片坊 RecipeLab 中文汉化版**](https://github.com/wslzgf/recipe-lab-sony-pmca-chinese) | Recipe Lab 的简体中文汉化版，界面全中文，内置中文字体，修复汉字方框问题 |
| [voxivoid/recipe-lab-sony-pmca](https://github.com/voxivoid/recipe-lab-sony-pmca) | **Recipe Lab 原版**：77 种胶片色彩配方，实时预览并写入相机，照片/视频全模式生效 |
| [ukiki0718-netizen/sony-a5100-film-studio](https://github.com/ukiki0718-netizen/sony-a5100-film-studio) | **胶片工坊 Film Studio**：富士参考与理光风格预设，强度可调，含照片/视频控制 |
| [bonyback1/sony-pmca-ricoh-mod](https://github.com/bonyback1/sony-pmca-ricoh-mod) | 照片效果增强模组，新增理光 GR 色彩配置 |

## 手机连接与无线传输

| 项目 | 说明 |
|---|---|
| [BI2QFA/SonyConnect](https://github.com/BI2QFA/SonyConnect) | **SonyConnect**：为索尼老机型提供更方便的手机连接与传输功能（相机端 + 手机端） |
| [BI2QFA/SonyFTP](https://github.com/BI2QFA/SonyFTP) | 为可安装 APK 的索尼相机添加 FTP 功能 |
| [schnatterer/pmcaFilesystemServer](https://github.com/schnatterer/pmcaFilesystemServer) | 通过 HTTP 在局域网访问相机文件系统 |
| [Bostwickenator/STGUploader](https://github.com/Bostwickenator/STGUploader) | 将照片自动上传至 Google Photos |
| [Novex/pmca-livestream](https://github.com/Novex/pmca-livestream) | 为索尼运动相机（X3000/AS300）提供自定义 RTMP 直播 |

## 开发与示例

| 项目 | 说明 |
|---|---|
| [ma1co/PMCADemo](https://github.com/ma1co/PMCADemo) | 索尼相机示例应用，二次开发参考 |
| [ma1co/OpenMemories-Framework](https://github.com/ma1co/OpenMemories-Framework) | 相机应用开发框架与 API 参考 |

---

## 注意事项

1. **签名不同不能覆盖安装**：不同来源的 APK 签名不同，安装前需先卸载旧版本，再全新安装。
2. **卸载会清除应用数据**：卸载应用会清除其收藏、配置等本地数据，请提前记录。
3. **照片效果（PE）类功能需 JPEG**：使用照片效果类配方时画质必须为 JPEG，RAW 下相机会自动停用效果。
4. **设置 ID 因机型而异**：各项目多在特定机型上逆向得到设置地址，安装后请对照相机菜单核对参数，确认无误再正式使用。
5. **认准 `MENU → 应用程序`**：没有该菜单的机型（2016 年底之后发布）无法安装任何此类应用。

## 补充项目

如发现其他可用于索尼老机型的开源应用，欢迎在 Issues 中提供链接，核实可用后补充到本列表。
