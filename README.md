# 毛泽东诗词 · 诗意墨韵

纯前端毛泽东诗词展示页面，宣纸长卷风格，逐首翻页浏览。

## 技术

- 纯 HTML/CSS/JS，零框架零依赖
- CSS Scroll Snap 实现逐首翻页
- IntersectionObserver + Scroll 双重监听同步右侧导航
- 响应式布局，适配桌面端和移动端

## 使用

1. 直接浏览器打开 `index.html`（需本地服务器，因为 fetch 加载 JSON）
2. 启动本地服务器：`python -m http.server 8080`
3. 浏览器访问 `http://localhost:8080`

## 添加新诗词

编辑 `poems.json`，按格式追加：

```json
{
  "id": 31,
  "title": "诗词标题",
  "date": "1970-01",
  "category": "诗",
  "content": [
    "第一行",
    "第二行"
  ],
  "background": "创作背景（可选）"
}
```

日期格式：`YYYY` / `YYYY-MM` / `YYYY-季节`，按时间自动排序。

## 项目结构

```
mao_verse/
├── index.html    # 主页面
├── poems.json    # 诗词数据（30首）
└── README.md
```
