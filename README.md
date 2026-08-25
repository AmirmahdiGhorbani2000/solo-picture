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

فایل را دانلود کرده و روی آن دابل کلیک کنید.

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

GNU General Public License v3.0
## حمایت 
اگر این پروژه رو دوست داشتید، لطفاً ستاره بدید!
