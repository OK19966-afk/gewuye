# 格物页 · 产品介绍页

AI 公考智能题训与评测平台「格物页」的单页官网，内容来自《格物页考生专享版》项目介绍 PPT，动效参考现代 SaaS 官网的滚动叙事风格。

## 预览

直接打开 `index.html`，或用任意静态服务器：

```bash
python3 -m http.server 8000
# 打开 http://127.0.0.1:8000
```

## 结构

```
index.html          单文件页面（内联 CSS / JS，无外部依赖）
assets/
  logo-mark.png     格物页标识
  logo-qingyun.png  青昀科创标识
  ui-dashboard.png  产品界面：学习工作台
  ui-library.png    产品界面：文章广场
  ui-report.png     产品界面：学习数据
  qr-wechat.png     微信二维码
```

## 动效

- 首屏标题遮罩逐行上浮，元素分级延迟入场
- 鼠标视差 + 产品截图 3D 倾斜
- 滚动揭示（IntersectionObserver 级联）
- 数字滚动
- 竖向钉住 + 横向推进的五步训练流程
- 卡片光斑跟随、marquee 跑马灯
- 导航毛玻璃 / 下滑隐藏 / 锚点高亮、顶部滚动进度条
- 支持 `prefers-reduced-motion` 降级

## 技术

纯静态，零构建、零依赖，兼容现代浏览器。响应式断点 1080 / 760。

---

广州青昀科创有限公司 · 格物页 · 2026.10
