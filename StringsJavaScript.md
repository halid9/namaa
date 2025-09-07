### ملخص لسلاسل النصوص (Strings) في JavaScript

سلاسل النصوص في JavaScript تُستخدم لتخزين ومعالجة النصوص. إليك ملخص لأهم المفاهيم الموجودة في صفحة W3Schools:

-----

#### إنشاء سلاسل النصوص

يمكنك إنشاء سلسلة نصية باستخدام علامات التنصيص المفردة (`'`) أو المزدوجة (`"`):

```javascript
let name1 = "Ahmad";  // باستخدام علامات التنصيص المزدوجة
let name2 = 'Ali';    // باستخدام علامات التنصيص المفردة
```

-----

#### طول السلسلة النصية

يمكنك الحصول على عدد الأحرف في السلسلة النصية باستخدام خاصية `length`:

```javascript
let text = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
let length = text.length; // ستكون القيمة 26
```

-----

#### الأحرف الخاصة (Escape Characters)

إذا كنت بحاجة إلى استخدام علامات التنصيص داخل سلسلة نصية، يجب عليك استخدام الشرطة المائلة العكسية (`\`) لتجنب حدوث أخطاء:

```javascript
let text = "We are the so-called \"Vikings\" from the north.";
```

-----

#### استخراج أجزاء من السلسلة النصية

هناك ثلاث دوال رئيسية لاستخراج جزء من سلسلة نصية:

  * **`slice(start, end)`**: تستخرج جزءًا من السلسلة النصية وتعيده كسلسلة نصية جديدة.
  * **`substring(start, end)`**: تشبه `slice` ولكن لا يمكنها قبول القيم السالبة.
  * **`substr(start, length)`**: تشبه `slice` ولكن المعامل الثاني يحدد طول الجزء المراد استخراجه.

<!-- end list -->

```javascript
let str = "Apple, Banana, Kiwi";
let part = str.slice(7, 13); // سيُعيد "Banana"
```

-----

#### استبدال محتوى السلسلة النصية

تُستخدم دالة `replace()` لاستبدال قيمة محددة بقيمة أخرى في السلسلة النصية. بشكل افتراضي، تقوم باستبدال أول تطابق فقط:

```javascript
let text = "Please visit Microsoft!";
let newText = text.replace("Microsoft", "W3Schools"); // سيُعيد "Please visit W3Schools!"
```

-----

#### تحويل حالة الأحرف

يمكنك تحويل السلسلة النصية إلى أحرف كبيرة أو صغيرة باستخدام:

  * **`toUpperCase()`**: لتحويل النص إلى أحرف كبيرة.
  * **`toLowerCase()`**: لتحويل النص إلى أحرف صغيرة.

<!-- end list -->

```javascript
let text1 = "Hello World!";
let text2 = text1.toUpperCase(); // سيُعيد "HELLO WORLD!"
```

-----

#### البحث عن النصوص

هناك عدة دوال للبحث عن نصوص داخل سلسلة نصية:

  * **`indexOf()`**: تُعيد موضع (index) أول ظهور لنص محدد.
  * **`lastIndexOf()`**: تُعيد موضع آخر ظهور لنص محدد.
  * **`search()`**: تبحث عن نص محدد وتُعيد موقعه.
  * **`includes()`**: تُعيد `true` إذا كانت السلسلة النصية تحتوي على نص محدد.
  * **`startsWith()`**: تُعيد `true` إذا كانت السلسلة النصية تبدأ بنص محدد.
  * **`endsWith()`**: تُعيد `true` إذا كانت السلسلة النصية تنتهي بنص محدد.

<!-- end list -->

```javascript
let str = "Please locate where 'locate' occurs!";
let pos = str.indexOf("locate"); // سيُعيد 7
```
