# Selfstarter ماهو
تم بناء هذا المشروع لتسهيل إطلاق المشاريع التي تعتمد على التمويل الجماعي ، يمكنك إعداد هذا المشروع بكل سهولة فقط بتحميل المشروع ومن ثم تغيير الإعدادت من ملف  ```config/settings.yml```
يمكن مشاهدة نسخة العرض لهذا التطبيق من الرابط التالي
<br/>
<a href="http://arselfstarter.herokuapp.com" target="blank">http://arselfstarter.herokuapp.com</a>


<br/>
أو من الموقع الرئيسي

<a href="http://selfstarter.us" target="blank">http://selfstarter.us</a>


## نظرة على المشروع
...

## كيف أبدء ؟
#### ملاحظة هامة: قبل البدء يجب التأكد من إعداد
* Ruby 1.9.2 or later
* توفر بعض المعرفة بأساسيات RubyGems

Terminal أولا  قم بإنشاء نسخة من المشروع ومن ثم تحميلها على جهازك بإستخدام الامر التالي من

```bash
git clone https://github.com/moh-alsheikh/selfstarter.git
```

Terminal ثانيا تحميل الجيمات او المكتبات التي سنحتاج لها في هذا التطبيق بتنفيذ الامر التالي 

```bash
bundle install --without production
```

ثالثا تنفيذ الامر التالي لإنشاء قاعدة البيانات
```bash
rake db:migrate
```

Terminal وأخيرا نقوم بتشغيل الخادم لمشاهدة المشروع بتنفيذ الامر التالي من  

```bash
rails s
```

يمكننا الآن تصفح التطبيق من الرابط التالي 

[http://0.0.0.0:3000](http://0.0.0.0:3000)

### التعديل على المشروع 

يمكن تغيير إعدادات التطبيق من ملف 

```
config/settings.yml
```

ينقسم الملف إلى عدة أقسام يحتوي كل قسم على إعدادت معينة مثلا اسم المنتج او المشروع ورابط الفيديو الذي يظهر في الصفحة الرئيسية والمبلغ المستهدف وتاريخ إطلاق المشروع .


يمكن تغيير بعض الإعدادات مثل ألوان الخطوط المختلفة - ألوان الخلفيات وغيرها بسهولة من ملف

```
app/assets/stylesheets/variables.css.scss
```

يمكن الإطلاع على كود المشروع من الملف

```
app/controllers/preorder_controller.rb
```

### Heroku نشر المشروع على منصة 

Terminal من أسهل وأسرع الطرق لنشر هذا التطبيق هي إستخدام منصة هيروكو وذلك بتنفيذ الاوامر التالية من 

```bash
gem install heroku
heroku create
git push heroku master
heroku run rake db:migrate
heroku open
```
## المشاركة والمساهمة في المشروع

....


### التقارير

..

### موفري خدمات الدفع 





