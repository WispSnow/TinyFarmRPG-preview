# TinyFarmRPG Preview

这是 TinyFarmRPG Web 预览版发布仓库，仅用于少量玩家测试与 bug 反馈。

本仓库只包含网页游戏运行文件，不包含 TinyFarmRPG 主项目源码。主项目与教学文档会在之后使用独立仓库发布。

## 网页游戏

- 游戏入口：https://wispsnow.github.io/TinyFarmRPG-preview/
- 备用入口：https://wispsnow.github.io/TinyFarmRPG-preview/TinyFarmRPG-Web.html

建议使用 Chrome 或 Chromium 浏览器游玩。首次进入需要下载 WebAssembly 与资源包，加载时间会受网络影响。

## 操作说明

| 功能 | 按键 |
| --- | --- |
| 移动 / 菜单选择 | W A S D 或方向键 |
| 确认 | Enter 或 Space |
| 取消 / 暂停 | Esc |
| 互动 | F |
| 打开背包 | I |
| 背包页签：装备 / 任务 / 地图 / 设置 | C / J / M / O |
| 快捷栏 | 1 到 0 |
| 快捷栏切换 | Tab |
| 主操作 / 副操作 | 鼠标左键 / 鼠标右键 |
| 旋转目标方向 | Q / E |
| 重置相机缩放 | 鼠标中键 |
| 显示 / 隐藏提示栏 | F1 |

Web debug 预览版保留了调试面板：

| 功能 | 按键 |
| --- | --- |
| Engine Debug Panels | F5 或 Ctrl+Shift+5 |
| Game Debug Panels | F6 或 Ctrl+Shift+6 |

也可以在地址后添加 `?debug-ui=engine`、`?debug-ui=game` 或 `?debug-ui=all`，启动时自动打开对应调试面板。

## 测试重点

- 标题页、新游戏、读档是否能正常进入。
- 家园、室内、城镇、学校之间的地图切换是否正常。
- 战斗、商店、任务、招募、休息、衣柜、设置是否能正常完成。
- 保存后刷新页面，再从标题页读档，确认地图、任务、队伍、外观、背包与设置是否保持。
- 控制台是否出现持续报错、黑屏、资源加载失败或 WebGL 异常。

存档和设置保存在浏览器本地数据中。清除站点数据、换浏览器或换设备后，存档不会自动迁移。

## 反馈方式

请在本仓库的 Issues 中提交问题。反馈时尽量附上：

- 浏览器与系统版本。
- 问题发生的位置或流程。
- 能否稳定复现，以及复现步骤。
- 截图、录屏或 DevTools Console 中的错误信息。

