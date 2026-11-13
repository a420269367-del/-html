# Leon Template – Landing Page

صفحة هبوط (Landing Page) بسيطة تم تنفيذها بناءً على شرح المحاضرة باستخدام **HTML** و **CSS** فقط.

## 📁 هيكل المشروع

```
Leon/
├── index.html        # هيكل الصفحة (المحتوى)
├── style.css         # تنسيق الصفحة
├── images/
│   └── landing.jpg   # صورة خلفية القسم الرئيسي
└── README.md         # هذا الملف
```

## 🧩 شرح الكود

### index.html
| الجزء | الوصف |
|-------|-------|
| `<head>` | ضبط الترميز، الـ viewport، عنوان الصفحة، خط Poppins من Google Fonts، وربط `style.css` |
| `header` | يحتوي على **الشعار** و**أيقونة القائمة** و**روابط التنقل** |
| `section.hero` | القسم الرئيسي: صورة الخلفية + العنوان `Hello There` + النص التوضيحي |
| `section#about` | قسم About (الرابط `#about` الظاهر في المحاضرة) |
| `section#contact` | قسم Contact |

> كل جزء في الكود مرفق بـ **comment** يوضح وظيفته.

### style.css
1. **المتغيرات `:root`**: الألوان وارتفاع الهيدر في مكان واحد لسهولة التعديل.
2. **تصفير الهوامش** `* { margin:0; padding:0 }` لتوحيد العرض بين المتصفحات.
3. **الهيدر**: `display:flex` لوضع الشعار يساراً والقائمة يميناً.
4. **الشعار**: مرسوم بالـ CSS (خط عمودي + دائرة بحدود ملونة) بدون صورة.
5. **القائمة**: تعمل بدون JavaScript عبر `input[type=checkbox]` مع الخاصية `:checked`.
6. **Hero**: `background: url(...) center bottom / cover` لتغطية القسم بالصورة، و`flex` لتوسيط المحتوى.
7. **Media Query**: تحسين العرض للشاشات الأقل من 600px.

## ▶️ طريقة التشغيل
افتح الملف `index.html` مباشرة في المتصفح.

## 🌐 الرفع على GitHub
```bash
git init
git add .
git commit -m "Add Leon landing page"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO-NAME.git
git push -u origin main
```
ولتفعيل رابط مباشر للموقع: **Settings → Pages → Branch: main → Save**.

## 🛠️ التقنيات المستخدمة
- HTML5
- CSS3 (Flexbox, Variables, Media Queries)
- Google Fonts (Poppins)
