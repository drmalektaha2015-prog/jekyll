---
عنوان: Quickstart
رابط دائم: /docs/
إعادة التوجيه من:
  - /docs/home/
  - /docs/quickstart/
  - /docs/extras/
---
جيكيل هو مولد مواقع ثابتة. يأخذ النص المكتوب بلغة الترميز المفضلة لديك
ويستخدم التخطيطات لإنشاء موقع ويب ثابت. يمكنك
تعديل مظهر الموقع ووظائفه، وعناوين URL، والبيانات المعروضة على الصفحة، وغير ذلك الكثير. 

## المتطلبات الأساسية

يتطلب برنامج جيكل ما يلي:

* إصدار روبي **{{ site.data.ruby.min_version }}** أو أعلى
* روبي جيمز
* مجلس التعاون الخليجي وصنع

يرى [متطلبات]({{ '/docs/installation/#requirements' | relative_url }}) للحصول على الأدلة والتفاصيل.

## تعليمات

1. قم بتثبيت الكل [المتطلبات الأساسية]({{ '/docs/installation/' | relative_url }}).
2. قم بتثبيت جيكيل وباندلر [الأحجار الكريمة]({{ '/docs/ruby-101/#gems' | relative_url }}).
```sh
gem install jekyll bundler
```
3. أنشئ موقع Jekyll جديد في `./myblog`.
```sh
مدونتي الجديدة جيكل
```
4. انتقل إلى دليلك الجديد.
```sh
cd مدونتي
```
5. قم ببناء الموقع واجعله متاحًا على خادم محلي.
```sh
bundle exec jekyll serve
```
6. تصفح إلى [http://localhost:4000](http://localhost:4000){:target="_blank"}

{: .note .warning}
إذا كنت تستخدم إصدار Ruby 3.0.0 أو أعلى، فقد تفشل الخطوة 5.(https://github.com/github/pages-gem/issues/752). يمكنك حل المشكلة بإضافة `webrick` إلى تبعياتك: `bundle add webrick`

{: .note .info}
مرّر الخيار `--livereload` إلى الأمر `serve` لتحديث الصفحة تلقائيًا مع كل تغيير تُجريه على ملفات المصدر: `bundle exec jekyll serve --livereload`

إذا واجهت أي أخطاء أثناء هذه العملية، فتأكد من تثبيت جميع المتطلبات الأساسية في [المتطلبات]]({{ '/docs/installation/#requirements' | relative_url }}). 
إذا استمرت المشكلة، راجع [استكشاف الأخطاء وإصلاحها]({{ '/docs/troubleshooting/#configuration-problems' | relative_url }}).

{: .note .info}
تختلف طريقة التثبيت باختلاف نظام التشغيل الخاص بك. راجع [أدلتنا]({{ '/docs/installation/#guides' | relative_url }}) للحصول على تعليمات خاصة بنظام التشغيل.
