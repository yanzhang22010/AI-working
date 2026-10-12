# Trip.Pulse UI 跨电脑交接

## 项目入口

- 主页面：`examples/agui-weekend.html`
- 另一示例：`examples/md-hotspots.html`
- 页面素材：`assets/`
- 设计规则：`references/`
- Skill 入口：`SKILL.md`

主页面为独立静态 HTML。保持当前目录结构后，直接用浏览器打开
`examples/agui-weekend.html` 即可预览。

## 当前实现状态

- 375 × 812 移动端页面与长页面内容已完成。
- 页面头部和吸顶 Logo 使用 `assets/trip-pulse-logo.png`。
- 头部与吸顶导航共用 `#FFF4E4` 到 `#FFFFFF`、高度 216px 的渐变。
- 航班地图的 One-way、价格和目的地标签使用独立 DOM 元素。
- 视频封面含播放按钮。
- 活动、用户分享、导览卡和问答区均已实现。
- 导览卡高度随文字内容自适应。
- AI 星形和 POI 定位图标均与第一行文字垂直居中。
- 第三张浴场导览卡包含 `Suzhou` POI 信息。

详细尺寸、颜色和对齐规则以 `references/agui-page.md` 为准。

## 在另一台电脑继续

1. 解压整个 `trip-pulse-ui` 文件夹，保持文件层级不变。
2. 在 Codex 中把该文件夹添加为本地项目。
3. 新建任务，并让 Codex先阅读 `SKILL.md`、`HANDOFF.md` 和
   `references/agui-page.md`。
4. 用浏览器打开 `examples/agui-weekend.html`，继续通过页面评论校对。

可以直接使用下面的提示词：

> 继续完善 Trip.Pulse 页面。先阅读 SKILL.md、HANDOFF.md 和
> references/agui-page.md，再检查 examples/agui-weekend.html。
> 保留现有 375px 页面结构、素材和已确认的设计规则，根据我接下来的
> 页面评论逐项修改；每次修改后校验资源路径和 JavaScript，并更新交付包。

## 环境注意事项

- 页面优先使用本机安装的 Trip Geom 字体；另一台电脑未安装该字体时会回退到
  Avenir Next 或 Arial，视觉效果会有差异。请在许可允许的情况下安装同一字体。
- 当前交付包已包含页面使用的图片、SVG、Logo 和 Figma 参考截图。
- `trip-pulse-ui` 项目文件夹已初始化本地 Git。若需要长期在多台电脑间同步，
  用 GitHub Desktop 添加该文件夹并发布到私人远程仓库即可。

