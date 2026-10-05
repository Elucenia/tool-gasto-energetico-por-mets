<!-- ELUCENIA technical documentation · gasto-energetico-por-mets · ar · no clinical/professional/rights approval -->

# الإنفاق الطاقي حسب METs

[الشروط والمصادر والأذونات](https://elucenia.org/ar/tools/gasto-energetico-por-mets)

## كيفية الاستخدام

استخدم الأداة في البوابة أو افتح index.html عبر خادم HTTP محلي. اختر اللغة، وأكمل الحقول، ثم أجرِ الحساب.

## المدخلات والوحدات

### شدة النشاط (قيمة Compendium)

`met`

METs · النطاق: ١–٢٥

### الوزن

`peso`

kg · النطاق: ٢٠–٣٠٠

### مدة الجلسة

`min`

min · النطاق: ١–٦٠٠

### الجلسات أسبوعيًا

`sessoes`

اختياري · النطاق: ١–١٤

## إصدار الطريقة

MET معياري 3.5 mL O₂/kg/min؛ kcal/min=MET×3.5×kg/200؛ مرجع Compendium 2024

## المعادلة الموثقة

kcal/min = METs × 3.5 × الوزن (kg) ÷ 200 (1 MET = 3.5 mL O2/kg/min؛ نحو 5 kcal لكل لتر O2).

MET-min = METs × الدقائق. تقريب مكافئ: kcal ≈ METs × الوزن (kg) × الساعات.

## الحدود والفئة السكانية

تتعلق قيم MET في دليل الأنشطة للبالغين لعام 2024 بأنشطة بالغين بعمر 19–59 سنة؛ واستُبعدت بيانات الأشخاص بعمر ≥60 سنة من هذا الإصدار. لا تقيس القيم المعيارية، بما فيها القيم المقدرة، الإنفاق الفردي للطاقة. يتطلب الأطفال وكبار السن والحالات السريرية الخاصة مصادر وطرقًا ملائمة لهذه الفئات.

## المراجع

- [Herrmann SD et al. 2024 Adult Compendium of Physical Activities: a third update of the energy costs of human activities. J Sport Health Sci, 2024.](https://doi.org/10.1016/j.jshs.2023.10.010)

- [Garber CE et al. Quantity and quality of exercise for developing and maintaining cardiorespiratory, musculoskeletal, and neuromotor fitness in apparently healthy adults. Med Sci Sports Exerc, 2011.](https://doi.org/10.1249/MSS.0b013e318213fefb)

## إعادة إجراء الاختبارات التقنية

شغّل node test.cjs في المجلد الجذري لهذا المستودع لتكرار الحالات الاصطناعية المسجلة. تُحفظ المدخلات والنتائج المتوقعة وحدود التفاوت الأصلية. لا تُعدّ الاختبارات التقنية تحققًا سريريًا.

```sh
node test.cjs
```

يحتوي tool.json على المصادر والإصدار ونطاق المراجعة. يحتفظ examples.json بالمدخلات والنتائج المتوقعة للحالات الاصطناعية؛ ويسجل results.json النتائج التي تم الحصول عليها.

[السجل والمراجع](../tool.json) · [شيفرة JavaScript](../calculator.js) · [حالات مرجعية](../examples.json) · [results.json](../results.json)

## المراجعة وشروط الاستخدام

لم تُجرَ مراجعة سريرية مستقلة.

هذه الواجهة ترجمة أعدّها مؤلفوها، وليست إصدارًا رسميًا أو معتمدًا. لم تُجرَ مراجعة سريرية مستقلة أو مراجعة لغوية مهنية، ولم تُستكمل الموافقة على حقوق استخدام الأدوات.

نتيجة المعادلة أو التصنيف. يعتمد التفسير والتصرف ومدى الانطباق على التقييم المهني والمصدر المحدد.

## الترخيص ونسبة العمل إلى أصحابه

ينطبق Apache-2.0 على كود ELUCENIA فقط. تبقى حقوق الأدوات والمنشورات والترجمات والبيانات لأصحابها المعنيين. احتفظ بملفّي LICENSE وNOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
