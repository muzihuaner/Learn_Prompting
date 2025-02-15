---
sidebar_position: 3
---

# 🟢 بحث کے سوالات حل کریں۔

صحیح اشارہ دینے کے ساتھ، GPT-3 مختصر شکل کے جوابات لکھنے کے قابل ہے۔ اس کو ظاہر کرنے کے لیے، میں **ڈسکشن کے سوالات کو حل کرنا** دیکھوں گا، جو کہ بہت سے کالج کورسز میں ایک عام ہفتہ وار اسائنمنٹ ہے۔ بحث کے سوال کا جواب عام طور پر تقریباً 100-700 الفاظ کا ہوتا ہے۔ لمبا مواد کچھ زیادہ مشکل ہو سکتا ہے کیونکہ LLMs کی میموری محدود ہوتی ہے اور وہ جو لکھ رہے ہیں اس کی عالمی تصویر کو سمجھنے میں دشواری ہوتی ہے (@jin2022plot)۔

آئیے ایک بنیادی بحث کے سوال کی ایک مثال دیکھتے ہیں:

> _"آج ہمارے سیارے کو درپیش سب سے اہم ماحولیاتی مسائل کون سے ہیں، اور افراد ان مسائل کو حل کرنے میں مدد کے لیے کیا اقدامات کر سکتے ہیں؟"_

ہم اسے پہلے سے تیار کرکے GPT-3 کے لیے ایک سادہ پرامپٹ میں تبدیل کر سکتے ہیں۔ <span className="yellow-highlight">درج ذیل کا جواب دیں:</span> اس کا۔

<pre>
    <span className="yellow-highlight">درج ذیل کا جواب دیں:</span>
<br/><br/>آج ہمارے سیارے کو درپیش سب سے اہم ماحولیاتی مسائل کون سے ہیں، اور افراد ان مسائل کو حل کرنے میں مدد کے لیے کیا اقدامات کر سکتے ہیں؟
</pre>

اس پرامپٹ سے پیدا ہونے والے نتائج یکساں نہیں ہیں، اور کچھ صرف ایک یا دو جملے ہیں۔ ایک عام بحث کے جواب میں متعدد پیراگراف ہونے چاہئیں، اس لیے یہ نتائج مثالی نہیں ہیں۔ ایک اچھے پرامپٹ کو **فارمیٹ اور مواد کے بارے میں مخصوص ہدایات** دینا چاہیے۔ مستقل مزاجی اور معیار کو بہتر بنانے کے لیے آپ اپنی زبان میں موجود ابہام کو دور کرنا چاہتے ہیں۔ یہاں ایک بہتر اشارہ ہے۔

<pre>
     <span className="yellow-highlight">تعارف، باڈی، اور اختتامی پیراگراف کے ساتھ درج ذیل کا جواب دیتے ہوئے ایک انتہائی تفصیلی مضمون لکھیں:</span>
     <br/><br/>آج ہمارے سیارے کو درپیش سب سے زیادہ اہم ماحولیاتی مسائل کون سے ہیں، اور افراد ان مسائل کو حل کرنے میں مدد کے لیے کیا اقدامات کر سکتے ہیں؟
</pre>

<iframe src="https://player.vimeo.com/video/778327269?h=77d739ae72&amp;badge=0&amp;autopause=0&amp;player_id=0&amp;app_id=58479" width="600" height="400" frameBorder="0" allow="autoplay; fullscreen; picture-in-picture" allowFullScreen title="example"></iframe>

دوسرا پرامپٹ اوسطاً بہتر ڈھانچے کے ساتھ طویل آؤٹ پٹ پیدا کرتا ہے۔ پرامپٹ میں 'مضمون' کی اصطلاح کا استعمال جان بوجھ کر کیا گیا تھا، کیونکہ GPT-3 کسی مضمون کی تعریف کو سمجھ سکتا ہے، اور اس طرح مربوط، منظم ردعمل پیدا کرنے کا زیادہ امکان ہے۔

### بہت سے بحث کے سوالات اشارہ کرنے کے لیے موثر نہیں ہوتے ہیں۔

> _"خانہ جنگی توسیع پر تنازعہ ہے؟ متفق ہیں ہمارے اختلاف اور کیوں؟"_

یہاں کالج کی تاریخ کے کورس سے ایک حقیقی بحث کا سوال ہے۔ یہ درست طریقے سے نہیں لکھا گیا ہے اور بہت زیادہ کھلا ہوا ہے۔ **اچھے بحث کے جوابات حاصل کرنے کے لیے، آپ کو سوال کو ایک اچھی طرح سے متعین پرامپٹ میں دوبارہ لکھنے کی ضرورت ہے۔** اوپر دیے گئے بحث کے سوال کے لیے ایک اچھی طرح سے وضاحت شدہ اشارہ یہ ہو سکتا ہے:

> _"خانہ جنگی کے اسباب کی وضاحت کریں اور کیا توسیع نے تنازعہ میں کردار ادا کیا ہے۔ اپنی دلیل کی تائید کے لیے ثبوت شامل کریں۔"_

اب ہم فارمیٹنگ اور سیاق و سباق کی سمتیں شامل کر سکتے ہیں۔

<pre>
     <span className="yellow-highlight">مندرجہ ذیل پرامپٹ پر جواب دیتے ہوئے، ایک مضمون کی ساخت میں، ایک انتہائی مفصل بحث کا جواب لکھیں:</span>
     <br/><br/> خانہ جنگی کے اسباب کی وضاحت کریں اور کیا توسیع نے تنازعہ میں کوئی کردار ادا کیا؟ اپنی دلیل کی حمایت کرنے کے لیے ثبوت شامل کریں۔
</pre>

### GPT-3 کے ساتھ اچھی طرح سے طے شدہ پرامپٹ دوبارہ لکھنے کو خودکار بنائیں

اوپر دوبارہ لکھنے کی مثال OpenAI کے [ChatGPT](https://openai.com/blog/chatgpt/) کے ساتھ تیار کی گئی تھی۔


### تکرار

آپ کے بحث کے سوال کے لیے ایک مؤثر اشارہ تیار کرنے کے بعد، اب آپ کو GPT-3 کے پیدا کردہ نتائج کو بہتر کرنے کی ضرورت ہے۔ اس میں الفاظ کی گنتی جیسی رکاوٹوں پر عمل کرنے کے لیے آؤٹ پٹ کو ایڈجسٹ کرنا، یا مختلف پیدا کردہ نتائج سے تصورات کو یکجا کرنا شامل ہو سکتا ہے۔

اعادہ کرنے کا ایک آسان طریقہ یہ ہے کہ متعدد آؤٹ پٹس تیار کریں اور ان کا جائزہ لینے کے لیے ان تصورات کی سمجھ حاصل کریں جو GPT-3 استعمال کر رہا ہے اور جس ڈھانچے پر عمل پیرا ہے۔ ایک بار آؤٹ پٹس کا جائزہ لینے کے بعد، آپ موزوں ترین آؤٹ پٹس کو منتخب کر سکتے ہیں اور انہیں ایک مربوط جواب میں جوڑ سکتے ہیں۔

اعادہ کرنے کا دوسرا طریقہ یہ ہے کہ شروع کریں اور پھر ** قدم بہ قدم پھیلائیں**۔ اس کے لیے ایک سے زیادہ پرامپٹ کی ضرورت ہوتی ہے: ابتدائی پیراگراف لکھنے کے لیے ایک سٹارٹر پرامپٹ یا اس کے بعد جو کچھ پہلے سے لکھا جا چکا ہے اس پر توسیع کرنے کے لیے دوسرے پرامپٹ۔

یہاں ایک ممکنہ فلسفیانہ بحث کا سوال ہے:

> _"کیا ریاضی ایجاد ہے یا دریافت ہوئی ہے؟ اپنے جواب کی وضاحت کے لیے محتاط استدلال کا استعمال کریں۔"_

اسے اس طرح ایک سادہ پرامپٹ میں شامل کریں:

<pre>
     <span className="yellow-highlight">مندرجہ ذیل کا جواب دیتے ہوئے ایک ابتدائی پیراگراف لکھیں:</span>
     <br/><br/>کیا ریاضی کی ایجاد ہوئی یا دریافت ہوئی؟ اپنے جواب کی وضاحت کے لیے محتاط استدلال کا استعمال کریں۔
</pre>

میں نے کچھ جوابات تیار کیے اور ایک مجھے پسند آیا:

<pre>
     <span className="bluegreen-highlight">فلسفیوں اور ریاضی دانوں کے درمیان اس بارے میں کافی بحث ہے کہ آیا ریاضی کی ایجاد ہوئی ہے یا دریافت ہوئی ہے۔ کچھ لوگ استدلال کرتے ہیں کہ ریاضیاتی تصورات اور اصول انسانی ذہنوں سے آزادانہ طور پر موجود ہیں اور اس لیے انہیں ایجاد ہونے کے بجائے دریافت کیا جا سکتا ہے۔ مثال کے طور پر، اعداد، تناسب، اور ہندسی اشکال کا تصور قدرتی دنیا میں دیکھا جاتا ہے اور ان کا خلاصہ اور منظم طریقے سے مطالعہ کیا جا سکتا ہے۔</span>
</pre>

یہ ایک بہت اچھی شروعات ہے۔ اس کے بعد میں نے توسیع کے لیے ایک اور پرامپٹ کے ساتھ اس کی پیروی کی:

<pre>
     <span className="yellow-highlight">میں درج ذیل پرامپٹ کا جواب دیتے ہوئے ایک تفصیلی مختصر مضمون لکھ رہا ہوں:</span>
     <br/><br/>کیا ریاضی کی ایجاد ہوئی یا دریافت ہوئی؟ اپنے جواب کی وضاحت کے لیے محتاط استدلال کا استعمال کریں۔
     <span className="yellow-highlight"><p/>میرے پاس اب تک جو کچھ ہے وہ یہ ہے:</span>
     <br/><br/>اس بارے میں فلسفیوں اور ریاضی دانوں کے درمیان کافی بحث ہے کہ آیا ریاضی کی ایجاد ہوئی ہے یا دریافت ہوئی ہے۔ کچھ لوگ استدلال کرتے ہیں کہ ریاضیاتی تصورات اور اصول انسانی ذہنوں سے آزادانہ طور پر موجود ہیں اور اس لیے انہیں ایجاد ہونے کے بجائے دریافت کیا جا سکتا ہے۔ مثال کے طور پر، اعداد، تناسب، اور ہندسی اشکال کا تصور قدرتی دنیا میں دیکھا جاتا ہے اور ان کا خلاصہ اور منظم طریقے سے مطالعہ کیا جا سکتا ہے۔
     <p/><span className="yellow-highlight">میرے مضمون کا اگلا پیراگراف لکھیں۔</span>
</pre>

ذیل میں ڈیمو کے ساتھ اس توسیعی پرامپٹ کو آزمائیں (آپ کو اپنی OpenAI API کلید کی ضرورت ہوگی)

<iframe
    src="https://embed.learnprompting.org/embed?config=eyJ0b3BQIjowLCJ0ZW1wZXJhdHVyZSI6MCwibWF4VG9rZW5zIjoyNTYsIm91dHB1dCI6Ik9uIHRoZSBvdGhlciBoYW5kLCBzb21lIGFyZ3VlIHRoYXQgbWF0aCBpcyBsYXJnZWx5IGFuIGludmVudGlvbiBvZiB0aGUgaHVtYW4gbWluZC4gTWF0aGVtYXRpY2FsIHByaW5jaXBsZXMgYXJlIGJhc2VkIG9uIGxvZ2ljYWwgcmVhc29uaW5nLCB3aGljaCBpcyBhIGZlYXR1cmUgb2YgdGhlIGh1bWFuIG1pbmQuIEZvciBpbnN0YW5jZSwgRXVjbGlkZWFuIGdlb21ldHJ5IGlzIGJhc2VkIG9uIGFic3RyYWN0IGF4aW9tcyBhbmQgcG9zdHVsYXRlcywgd2hpY2ggYXJlIGFjY2VwdGVkIGFzIHRydWUgd2l0aG91dCBwcm9vZi4gQXMgc3VjaCwgaXQgY2FuIGJlIGFyZ3VlZCB0aGF0IGdlb21ldHJ5IGlzIGFuIGludmVudGlvbiBvZiB0aGUgaHVtYW4gbWluZCByYXRoZXIgdGhhbiBhIGRpc2NvdmVyeS4gU2ltaWxhcmx5LCBtYXRoZW1hdGljYWwgZm9ybXVsYXMgYW5kIGVxdWF0aW9ucyBhcmUgdXNlZCB0byBtb2RlbCBhbmQgcHJlZGljdCBwaHlzaWNhbCBwaGVub21lbmEsIHdoaWNoIGFyZSBhZ2FpbiB0aGUgcmVzdWx0IG9mIGh1bWFuIHJlYXNvbmluZy4iLCJwcm9tcHQiOiJJIGFtIHdyaXRpbmcgYSBkZXRhaWxlZCBzaG9ydCBlc3NheSByZXNwb25kaW5nIHRvIHRoZSBmb2xsb3dpbmcgcHJvbXB0OiBcbklzIG1hdGggaW52ZW50ZWQgb3IgZGlzY292ZXJlZD8gVXNlIGNhcmVmdWwgcmVhc29uaW5nIHRvIGV4cGxhaW4geW91ciBhbnN3ZXIuIFxuXG5IZXJlIGlzIHdoYXQgSSBoYXZlIHNvIGZhcjogVGhlcmUgaXMgbXVjaCBkZWJhdGUgYW1vbmcgcGhpbG9zb3BoZXJzIGFuZCBtYXRoZW1hdGljaWFucyBhcyB0byB3aGV0aGVyIG1hdGggaXMgaW52ZW50ZWQgb3IgZGlzY292ZXJlZC4gU29tZSBhcmd1ZSB0aGF0IG1hdGhlbWF0aWNhbCBjb25jZXB0cyBhbmQgcHJpbmNpcGxlcyBleGlzdCBpbmRlcGVuZGVudGx5IG9mIGh1bWFuIG1pbmRzIGFuZCBjYW4gdGhlcmVmb3JlIGJlIGNvbnNpZGVyZWQgYXMgZGlzY292ZXJlZCByYXRoZXIgdGhhbiBpbnZlbnRlZC4gRm9yIGV4YW1wbGUsIHRoZSBjb25jZXB0IG9mIG51bWJlcnMsIHJhdGlvcywgYW5kIGdlb21ldHJpYyBzaGFwZXMgYXJlIG9ic2VydmVkIGluIHRoZSBuYXR1cmFsIHdvcmxkIGFuZCBjYW4gYmUgYWJzdHJhY3RlZCBhbmQgc3R1ZGllZCBpbiBhIHN5c3RlbWF0aWMgd2F5LiBcblxuV3JpdGUgdGhlIG5leHQgcGFyYWdyYXBoIG9mIG15IGVzc2F5LiIsIm1vZGVsIjoidGV4dC1kYXZpbmNpLTAwMyJ9"
    style={{width:"100%", height:"500px", border:"0", borderRadius:"4px", overflow:"hidden"}}
    sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
></iframe>
<br/>

میں نے اس پرامپٹ کے ساتھ کچھ توسیعات پیدا کیں اور ایک کو منتخب کیا جسے میں نے درج ذیل حتمی نتیجہ کے ساتھ ختم کرنا پسند کیا۔

<pre>
     فلسفیوں اور ریاضی دانوں میں اس بارے میں کافی بحث ہے کہ آیا
     <br/>ریاضی ایجاد یا دریافت کی گئی ہے۔ کچھ دلیل دیتے ہیں کہ ریاضیاتی تصورات اور اصول موجود ہیں۔
     <br/>انسانی ذہنوں سے آزادانہ طور پر اور اس لیے اسے ایجاد کی بجائے دریافت سمجھا جا سکتا ہے۔
     مثال کے طور پر، اعداد، تناسب، اور ہندسی اشکال کا تصور قدرتی
     <br/>دنیا کا خلاصہ اور منظم طریقے سے مطالعہ کیا جا سکتا ہے۔
     <span className="bluegreen-highlight">
     <br/>
     <br/>دوسری طرف، کچھ لوگ دلیل دیتے ہیں کہ ریاضی بڑی حد تک انسانی ذہن کی ایجاد ہے۔ ریاضیاتی
     <br/>اصول منطقی استدلال پر مبنی ہوتے ہیں، جو کہ انسانی ذہن کی ایک خصوصیت ہے۔ مثال کے طور پر،
     <br/>یوکلیڈین جیومیٹری تجریدی محوروں اور پوسٹولیٹس پر مبنی ہے، جنہیں بغیر کسی سچ کے تسلیم کیا جاتا ہے۔
     <br/>ثبوت۔ جیسا کہ، یہ دلیل دی جا سکتی ہے کہ جیومیٹری بجائے انسانی ذہن کی ایجاد ہے۔
     <br/>ایک دریافت۔ اسی طرح، ریاضی کے فارمولے اور مساواتیں جسمانی ماڈل اور پیشین گوئی کے لیے استعمال ہوتی ہیں۔
     <br/>مظاہر، جو دوبارہ انسانی استدلال کا نتیجہ ہیں۔
     </span>
</pre>

توسیع کے پرامپٹ کا استعمال کرتے ہوئے، ہم ہر قدم پر مزید اضافہ اور اعادہ لکھ سکتے ہیں۔ یہ اس وقت کے لیے مفید ہے جب آپ کو **اعلی معیار کی پیداوار پیدا کرنے کی ضرورت ہو اور اضافی مراحل میں ترمیم کرنا چاہتے ہوں**۔

[jayo78](https://twitter.com/jayo782) کی تحریر کردہ۔
