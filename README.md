# SoloPicture v1.0

> ویرایشگر تصویر real-time با Canvas API و CSS Filter

## قابلیت‌ها
- **پردازش تصویر** با استفاده از `Canvas 2D Context`
- **فیلترهای زنده** شامل brightness, contrast, saturate, blur, rotate
- **فیلترهای ترکیبی** (grayscale, sepia, invert, hue-rotate)
- **رابط کاربری واکنش‌گرا** با Flexbox و Grid

## معماری فنی

### هسته پردازش
```javascript
ctx.filter = `brightness(${b}%) contrast(${c}%) saturate(${s}%) blur(${bl}px) ${filter}`;
ctx.drawImage(img, -w/2, -h/2);
```

### رندرینگ

· State Management: DOM-based (Slider + Filter)

· Render Loop: Event-driven (oninput/onclick)

· Transform: ctx.save() / ctx.restore() با rotate


### بهینه‌سازی

· Cache: نگهداری originalImage برای جلوگیری از re-render

· Throttling: نداشتن (مناسب برای پروژه تمرینی)

## اجرا

```bash
# Clone
git clone https://github.com/AmirmahdiGhorbani2000/solo-picture.git

# Open
open index.html   # یا دابل‌کلیک در مرورگر
```

## وابستگی‌ها

· Zero Dependencies (Vanilla JS)

· Polyfill: None (ES6+)

## تست

```bash
# Browser Support
✅ Chrome 90+
✅ Firefox 88+
✅ Safari 14+
```
## لایسنس


## حمایت 
اگر این پروژه رو دوست داشتید، لطفاً ستاره بدید!
