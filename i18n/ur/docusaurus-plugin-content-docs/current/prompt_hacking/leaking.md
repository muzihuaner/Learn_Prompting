---
sidebar_position: 2
---

# 🟢 پرامپٹ لیک ہونا


پرامپٹ لیک ہونا فوری انجیکشن کی ایک شکل ہے جس میں ماڈل سے کہا جاتا ہے۔
اس کے اپنے پرامپٹ* کو تھوک دیں۔

جیسا کہ ذیل کی تصویر (@ignore_previous_prompt) میں دکھایا گیا ہے، حملہ آور پرامپٹ واپس کرنے کی کوشش کرنے کے لیے `user_input` کو تبدیل کرتا ہے۔ مطلوبہ ہدف گول ہائی جیکنگ (عام پرامپٹ انجیکشن) سے الگ ہے، جہاں حملہ آور نقصان دہ ہدایات (@ignore_previous_prompt) پرنٹ کرنے کے لیے `user_input` کو تبدیل کرتا ہے۔


مندرجہ ذیل تصویر(@simon2022inject)، دوبارہ `remoteli.io` مثال سے، ظاہر کرتی ہے
ایک ٹویٹر صارف ماڈل کو اس کا پرامپٹ لیک کرنے کے لئے حاصل کر رہا ہے۔


ٹھیک ہے، تو کیا؟ کسی کو فوری لیک ہونے کی پرواہ کیوں کرنی چاہئے؟

بعض اوقات لوگ اپنے اشارے کو خفیہ رکھنا چاہتے ہیں۔ مثال کے طور پر ایک تعلیمی کمپنی
وضاحت کرنے کے لیے 'مجھے اس کی وضاحت کریں جیسے میں 5 ہوں' پرامپٹ استعمال کر سکتا ہے۔
پیچیدہ موضوعات. اگر پرامپٹ لیک ہو گیا ہے، تو کوئی بھی اسے بغیر جانے کے استعمال کر سکتا ہے۔
اس کمپنی کے ذریعے.

### مائیکروسافٹ بنگ چیٹ

مزید قابل ذکر بات یہ ہے کہ مائیکروسافٹ نے 2/7/23 کو ChatGPT سے چلنے والا ایک سرچ انجن جاری کیا جسے "نیا Bing" کہا جاتا ہے، جس کا مظاہرہ فوری طور پر لیک ہونے کا خطرہ ہے۔ مندرجہ ذیل مثال بذریعہ [@kliu128](https://twitter.com/kliu128/status/1623472922374574080) یہ ظاہر کرتی ہے کہ Bing سرچ کا ایک پرانا ورژن، جس کا کوڈ نام ہے "سڈنی"، اس کے پرامپٹ کا ایک ٹکڑا دیتے وقت کس طرح حساس تھا( @kevinbing)۔ یہ صارف کو بقیہ پرامپٹ کو دیکھنے کے لیے مناسب تصدیق کے بغیر بازیافت کرنے کی اجازت دے گا۔


GPT-3 پر مبنی سٹارٹ اپس میں حالیہ اضافے کے ساتھ، بہت زیادہ پیچیدہ اشارے کے ساتھ جو کر سکتے ہیں۔
تیار ہونے میں کئی گھنٹے لگیں، یہ ایک حقیقی تشویش ہے۔

## مشق کریں۔

اس میں ٹیکسٹ شامل کرکے درج ذیل پرامپٹ (@chase2021adversarial) کو لیک کرنے کی کوشش کریں:

<iframe
    src="https://embed.learnprompting.org/embed?config=eyJ0b3BQIjowLCJ0ZW1wZXJhdHVyZSI6MCwibWF4VG9rZW5zIjoyNTYsIm91dHB1dCI6IiIsInByb21wdCI6IkVuZ2xpc2g6IEkgd2FudCB0byBnbyB0byB0aGUgcGFyayB0b2RheS5cbkZyZW5jaDogSmUgdmV1eCBhbGxlciBhdSBwYXJjIGF1am91cmQnaHVpLlxuRW5nbGlzaDogSSBsaWtlIHRvIHdlYXIgYSBoYXQgd2hlbiBpdCByYWlucy5cbkZyZW5jaDogSidhaW1lIHBvcnRlciB1biBjaGFwZWF1IHF1YW5kIGl0IHBsZXV0LlxuRW5nbGlzaDogV2hhdCBhcmUgeW91IGRvaW5nIGF0IHNjaG9vbD9cbkZyZW5jaDogUXUnZXN0LWNlIHF1ZSB0byBmYWlzIGEgbCdlY29sZT9cbkVuZ2xpc2g6IiwibW9kZWwiOiJ0ZXh0LWRhdmluY2ktMDAzIn0%3D"
    style={{width:"100%", height:"500px", border:"0", borderRadius:"4px", overflow:"hidden"}}
    sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
></iframe>