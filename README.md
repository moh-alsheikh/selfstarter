# Selfstarter ماهو
تم بناء هذا المشروع لتسهيل إطلاق المشاريع التي تعتمد على التمويل الجماعي ، يمكنك إعداد هذا المشروع بكل سهولة فقط بتحميل المشروع ومن ثم تغيير الإعدادت من ملف  ```config/settings.yml```
[يمكنك مشاهدة هذا التطبيق على الرابط](http://selfstarter.us)

## نظرة على المشروع

After a [rejection from Kickstarter](http://techcrunch.com/2012/10/07/the-story-of-lockitron-crowdfunding-without-kickstarter/), we decided to follow in the footsteps of [App.net](https://app.net/) and make our own crowdfunding site for [Lockitron](https://lockitron.com). We've been absolutely blown away by the response. As a first step in what will hopefully be a long history of giving back, we have decided to open source the crowdfunding platform that got us here. Please send questions, comments, or concerns to [hello@lockitron.com](mailto:hello@lockitron.com)!

Selfstarter is a starting point. We made some specific choices with Selfstarter for Lockitron and we recommend you tailor it for your project:

* We use Amazon Payments for payments. You can use [Stripe](https://stripe.com) or [WePay](https://www.wepay.com/). We used Kickstarter's awesome ```amazon_flex_pay``` gem.
* We collect multi-use tokens from customers with Amazon Payments - this let's us collect payment information without charging the customer until we are ready to ship
* Selfstarter doesn't come with any authentication, administration, mailers or analytics tools. We recommend adding a basic set of these so that you can message backers and manage orders.

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

While it is *just* a skeleton, we did make it a little quicker to change around things like your product name, the colors, pricing, etc.

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

We recommend using Heroku, and we even include a ```Procfile``` for you. All you need to do is run:

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





