---
sidebar_position: 3
locale: en-us
style: chicago
---

# 🟢 چین آف تھاٹ پرمپٹنگ

چین آف تھاٹ (CoT) پرامپٹنگ (@wei2022chain) حال ہی میں تیار کیا گیا اشارہ ہے۔
طریقہ، جو LLM کو اس کی استدلال کی وضاحت کرنے کی ترغیب دیتا ہے۔ نیچے کی تصویر (@wei2022chain)
سوچ کے پرامپٹ (دائیں) کی زنجیر کے مقابلے میں %% چند شاٹ اسٹینڈرڈ پرامپٹ| چند شاٹ اسٹینڈرڈ پرامپٹ%% (بائیں) دکھاتا ہے۔


CoT کا بنیادی خیال یہ ہے کہ LLM کو کچھ شاٹ دکھا کر %%exemplars|exemplars%% جہاں استدلال
عمل کی وضاحت مثالوں میں کی گئی ہے، LLM استدلال کا عمل بھی دکھائے گا۔
پرامپٹ کا جواب دیتے وقت استدلال کی یہ وضاحت اکثر زیادہ درست ہونے کی طرف لے جاتی ہے۔
نتائج

## مثال

یہاں چند ڈیمو ہیں۔ پہلا دکھاتا ہے GPT-3 (davinci-003)
ایک سادہ لفظ کا مسئلہ حل کرنے میں ناکام۔ دوسرا GPT-3 (davinci-003) کو اسی مسئلے کو کامیابی سے حل کرتا ہے، CoT پرامپٹنگ کا استعمال کرتے ہوئے۔

#### غلط

<iframe
    src="https://embed.learnprompting.org/embed?config=eyJ0b3BQIjowLCJ0ZW1wZXJhdHVyZSI6MCwibWF4VG9rZW5zIjoyNTYsIm91dHB1dCI6Ik9wdGlvbiAxIGlzIGEgZmFzdGVyIHdheSB0byBnZXQgdG8gd29yay4iLCJwcm9tcHQiOiJXaGljaCBpcyBhIGZhc3RlciB3YXkgdG8gZ2V0IHRvIHdvcms%2FXG5PcHRpb24gMTogVGFrZSBhIDEwMDAgbWludXRlIGJ1cywgdGhlbiBhIGhhbGYgaG91ciB0cmFpbiwgYW5kIGZpbmFsbHkgYSAxMCBtaW51dGUgYmlrZSByaWRlLlxuT3B0aW9uIDI6IFRha2UgYW4gODAwIG1pbnV0ZSBidXMsIHRoZW4gYW4gaG91ciB0cmFpbiwgYW5kIGZpbmFsbHkgYSAzMCBtaW51dGUgYmlrZSByaWRlLiIsIm1vZGVsIjoidGV4dC1kYXZpbmNpLTAwMyJ9"
    style={{width:"100%", height:"500px", border:"0", borderRadius:"4px", overflow:"hidden"}}
    sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
></iframe>

#### درست

<iframe
    src="https://embed.learnprompting.org/embed?config=eyJ0b3BQIjowLCJ0ZW1wZXJhdHVyZSI6MCwibWF4VG9rZW5zIjoyNTYsIm91dHB1dCI6Ik9wdGlvbiAxIHdpbGwgdGFrZSAxMDAwKzMwKzEwID0gMTA0MCBtaW51dGVzLlxuT3B0aW9uIDIgd2lsbCB0YWtlIDgwMCs2MCszMCA9IDg5MCBtaW51dGVzLlxuU2luY2UgT3B0aW9uIDIgdGFrZXMgODkwIG1pbnV0ZXMgYW5kIE9wdGlvbiAxIHRha2VzIDEwNDAgbWludXRlcywgT3B0aW9uIDIgaXMgZmFzdGVyLiIsInByb21wdCI6IldoaWNoIGlzIGEgZmFzdGVyIHdheSB0byBnZXQgaG9tZT9cbk9wdGlvbiAxOiBUYWtlIGFuIDEwIG1pbnV0ZXMgYnVzLCB0aGVuIGFuIDQwIG1pbnV0ZSBidXMsIGFuZCBmaW5hbGx5IGEgMTAgbWludXRlIHRyYWluLlxuT3B0aW9uIDI6IFRha2UgYSA5MCBtaW51dGVzIHRyYWluLCB0aGVuIGEgNDUgbWludXRlIGJpa2UgcmlkZSwgYW5kIGZpbmFsbHkgYSAxMCBtaW51dGUgYnVzLlxuT3B0aW9uIDEgd2lsbCB0YWtlIDEwKzQwKzEwID0gNjAgbWludXRlcy5cbk9wdGlvbiAyIHdpbGwgdGFrZSA5MCs0NSsxMD0xNDUgbWludXRlcy5cblNpbmNlIE9wdGlvbiAxIHRha2VzIDYwIG1pbnV0ZXMgYW5kIE9wdGlvbiAyIHRha2VzIDE0NSBtaW51dGVzLCBPcHRpb24gMSBpcyBmYXN0ZXIuXG5cbldoaWNoIGlzIGEgZmFzdGVyIHdheSB0byBnZXQgdG8gd29yaz9cbk9wdGlvbiAxOiBUYWtlIGEgMTAwMCBtaW51dGUgYnVzLCB0aGVuIGEgaGFsZiBob3VyIHRyYWluLCBhbmQgZmluYWxseSBhIDEwIG1pbnV0ZSBiaWtlIHJpZGUuXG5PcHRpb24gMjogVGFrZSBhbiA4MDAgbWludXRlIGJ1cywgdGhlbiBhbiBob3VyIHRyYWluLCBhbmQgZmluYWxseSBhIDMwIG1pbnV0ZSBiaWtlIHJpZGUuIiwibW9kZWwiOiJ0ZXh0LWRhdmluY2ktMDAzIn0%3D"
    style={{width:"100%", height:"500px", border:"0", borderRadius:"4px", overflow:"hidden"}}
    sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
></iframe>

## نتائج

CoT جیسے کاموں پر نتائج کو بہتر بنانے میں موثر ثابت ہوا ہے۔
ریاضی، کامن سینس، اور علامتی استدلال کے کام (@wei2022chain)۔
خاص طور پر، حوصلہ افزائی کی گئی PaLM 540B(@chowdhery2022palm) 57% حل حاصل کرتی ہے
GSM8K(@cobbe2021training) (اس وقت SOTA) پر شرح کی درستگی۔

<div style={{textAlign: 'center'}}>
GSM8K بینچ مارک پر ماڈلز کا موازنہ (Wei et al.)
</div>

## حدود

اہم بات یہ ہے کہ Wei et al. کے مطابق، "CoT صرف اس وقت کارکردگی میں اضافہ کرتا ہے جب ∼100B پیرامیٹرز کے ماڈلز کے ساتھ استعمال کیا جائے"۔ چھوٹے ماڈلز نے سوچ کی غیر منطقی زنجیریں لکھیں، جس کی وجہ سے معیاری اشارہ کرنے سے بدتر درستگی ہوئی۔ ماڈلز کو عام طور پر ماڈل کے سائز کے ٹیکسٹاسب طریقے سے CoT پرامپٹ سے کارکردگی میں اضافہ ہوتا ہے۔

## نوٹس

اس باب کو لکھنے کے عمل میں زبان کے کسی ماڈل کو ~~ چوٹ~~ ٹھیک نہیں کیا گیا 😊