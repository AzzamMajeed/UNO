# تشغيل 3 لمبات بواسطة Arduino UNO وأزرار

مشروع بسيط باستخدام Arduino UNO لمحاكاة تشغيل ثلاث لمبات LED عن طريق الضغط على ثلاثة أزرار منفصلة. تم تنفيذه على Tinkercad Circuits.

## ⚙️ المكونات

- Arduino UNO  
- 3 × LED (مثل: أحمر / أصفر / أخضر)  
- 3 × Push Button  
- 3 × مقاومة 220 Ω لللمبات  
- 3 × مقاومة 10 kΩ للأزرار (Pull-down)  
- أسلاك توصيل  
- Breadboard

## 🧠 الفكرة

عند الضغط على كل زر، تضيء اللمبة المرتبطة به. تُطفأ عند رفع الضغط عن الزر.

## *كود الUNO*
// C++ code
//
void setup()
{
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop()
{
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
}
