---
title: Create a dummy file with a specific size
localeTitle: قم بإنشاء ملف وهمي بحجم معين
---
## كيفية إنشاء ملفات وهمية بحجم معين باستخدام الأمر "dd":

يمكن استخدام الأمر "dd" لإنشاء ملف بحجم معين. هذا مفيد إذا كنت ترغب في اختبار سرعة التنزيل ، أو أي اختبارات أخرى ، وتحتاج إلى ملف بحجم معين.

 `dd if=/dev/zero of=file_name.txt bs=1024k count=10 
` 

سيؤدي ذلك إلى إنشاء ملف بحجم 1 ميغابايت يسمى file\_name.txt.

bs هو حجم البايت الخاص بك والعد يمثل عدد الكتل. طريقة سهلة للنظر هي 1024 كيلو X 10.

إليك طريقة أكثر بساطة لإنشاء ملف 1MB:

 `dd if=/dev/zero of=file_name.txt bs=1MB count=1 
`