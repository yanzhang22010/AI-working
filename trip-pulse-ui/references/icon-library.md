# Trip 图标素材映射

Trip Icon & Illustration 图标库：Figma 文件 `uMtVOhUlX83eY1KNXHA6uL`，用户指定的节点 `7119:14408` 为 `account_filled`。此文件的 `03_General` 页面包含常用箭头、定位、分享、更多、键盘、发送图标。根据目标画板的 `get_design_context` 确定所需图标，再从图标组件或页面实例导出原素材；不要用 Unicode 符号冒充图标。

当前 `assets/` 中的本地图标已从 Figma 导出，可离线用于 `examples/`。HTML 以 `<img>` 明确设置宽高并给纯装饰图标空 `alt`；可交互按钮本身保留文字或 `aria-label`。

| 用途 | 本地素材 | 对应节点 | 当前呈现尺寸 |
| --- | --- | --- | --- |
| 返回 | `icon-back.svg` | AGUI `2550:12579` | 12 × 21，透明 SVG |
| 分享 | `icon-share.png` | MD `7564:82711` | 24 × 24 |
| 更多 | `icon-more.png` | MD `7564:82712` | 24 × 24 |
| 定位 | `icon-location.png` | 图标库 `7119:14373` | 地点信息中 14 × 14 |
| 下拉 | `icon-down-mask.svg` | MD `7564:82772` | 12 × 12 插槽，透明 SVG 等比居中 |
| 圆形下拉 | `icon-down-circle.png` | MD `7564:82766` | 12 × 12 |
| 更多入口箭头 | `icon-right.png` | AGUI `7563:81426` | 14 × 14，`#102846` |
| 键盘 | `icon-keyboard.png` | 图标库 `13018:358` | 24 × 24 |
| 提问发送 | `icon-ask.svg` | AGUI `7563:81663` | 16 × 16 |
| 视频播放 | `icon-play.svg` | AGUI `7563:81436` | 20 × 20，置于 40 × 40 黑色半透明圆形底中 |
| AI 星形 | `icon-ai-star.png` | 图标库 `10918:322` | 14 × 14，左到右 `#59C8FF` → `#6D4DF8` |
| 浏览量 | `icon-view-mask.svg` | AGUI `7563:81584` | 12 × 12 插槽，`#4F5563`，保持 24 × 24 viewBox 比例 |
| 用户头像 | `agui-user-avatar.png` | AGUI `7563:81581` 对应图片填充 | 18 × 18 |
| iOS 状态栏 | `ios-cellular.svg`、`ios-wifi.svg`、`ios-battery.svg` + HTML 时间文本 | AGUI `7563:81351` | 375 × 62 容器，矢量渲染 |

Figma 的个别组件实例导出会生成 1 × 1 的空白 PNG；遇到这种情况，应从图标库组件取得截图或其原始 SVG，并核验最终文件的实际尺寸与图形。状态栏属于系统组件，保留为单独的 375 × 62 素材，不用整页截图代替内容。新增图标先核对节点名称和轮廓是否匹配，再下载原素材入包；素材链接短期有效，不能直接写在交付 HTML 中。

需要对图标应用规范色或渐变时，使用 Figma 导出的透明 SVG 轮廓（`*-mask.svg`）作为 CSS `mask`，由 `background` 提供精确颜色。禁止将带不透明背景的 PNG 用作蒙版，否则背景会渲染成方块。图标的 SVG viewBox 必须等比缩放并居中，不能把方形 viewBox 强行压成非等比矩形，否则眼睛、星形等轮廓会变形。卡片通用的 `img` 尺寸规则不得覆盖内联图标尺寸；必要时使用更具体的组件选择器限定图标大小。
