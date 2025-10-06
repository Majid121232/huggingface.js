باشه مجید جان 👌  
الان برات یک نسخه‌ی نهایی و بدون خطا از README.md آماده می‌کنم که همه‌چیزش درست باشه (YAML، توضیحات، مثال‌ها، کد بارگذاری). بعد هم توضیح می‌دم چرا لوگو بعضی وقت‌ها آپلود نمی‌شه.

---

✅ README.md نهایی (کامل و استاندارد)

`markdown
---
license: apache-2.0
task_categories:
  - text-classification
  - question-answering
language:
  - fa
  - en
size_categories:
  - small
tags:
  - nlp
  - multitask
  - sentiment
  - toxicity
  - persian-english
pretty_name: Majid Multi-task Dataset | مجموعه داده چندوظیفه‌ای مجید
---

<p align="center">
  <img src="https://huggingface.co/datasets/Maid121232/majid-multitask-dataset/resolve/main/banner.png" alt="Majid Multitask Dataset Banner" width="100%"/>
</p>

<p align="center">
  <img src="https://huggingface.co/datasets/Maid121232/majid-multitask-dataset/resolve/main/logo.png" alt="Majid Multitask Dataset Logo" width="300"/>
</p>

Majid Multi-task Dataset | مجموعه داده چندوظیفه‌ای مجید

---

English Description 🇬🇧

This dataset provides Persian–English text for multi-task NLP: text classification and question answering, including subtasks such as sentiment analysis and toxicity detection.

Dataset Details
- Curated by: Maid121232 (Majid)  
- Languages: Persian (fa), English (en)  
- License: Apache-2.0  
- Size: Small (< 10k samples)  
- Tasks: Text Classification, Question Answering  

Dataset Structure
- Files: train.csv, valid.csv, test.csv  
- Columns:  
  - id → Sample ID  
  - text → Input text  
  - label → Task-specific label (e.g., positive/negative, toxic/non-toxic)  
  - task → Task type (sentiment, toxicity, qa, classification)  

Example:
`json
{
  "id": 1,
  "text": "This movie was amazing!",
  "label": "positive",
  "task": "sentiment"
}
`

Usage
`python
from datasets import load_dataset

base = "https://huggingface.co/datasets/Maid121232/majid-multitask-dataset/resolve/main"
ds = load_dataset(
    "csv",
    data_files={
        "train": f"{base}/train.csv",
        "validation": f"{base}/valid.csv",
        "test": f"{base}/test.csv",
    }
)
print(ds["train"][0])
`

Limitations
- Small dataset size, limited generalization.  
- Possible label noise.  
- Not balanced across all tasks.  

Citation
`bibtex
@dataset{majid2025multitask,
  author = {Maid121232},
  title = {Majid Multi-task Dataset},
  year = {2025},
  url = {https://huggingface.co/datasets/Maid121232/majid-multitask-dataset}
}
`

---

توضیحات فارسی 🇮🇷

این مجموعه داده برای چند وظیفه‌ی پردازش زبان طبیعی (NLP) طراحی شده است: طبقه‌بندی متن و پرسش و پاسخ؛ شامل زیروظایفی مثل تحلیل احساسات و تشخیص سمیت.

جزئیات
- تهیه‌کننده: Maid121232 (مجید)  
- زبان‌ها: فارسی (fa)، انگلیسی (en)  
- مجوز: Apache-2.0  
- اندازه: کوچک (کمتر از 10k نمونه)  
- وظایف: طبقه‌بندی متن، پرسش و پاسخ  

ساختار
- فایل‌ها: train.csv، valid.csv، test.csv  
- ستون‌ها: id، text، label، task  

مثال:
`json
{
  "id": 1,
  "text": "این فیلم فوق‌العاده بود!",
  "label": "positive",
  "task": "sentiment"
}
`

نحوه‌ی بارگذاری
`python
from datasets import load_dataset

base = "https://huggingface.co/datasets/Maid121232/majid-multitask-dataset/resolve/main"
ds = load_dataset(
    "csv",
    data_files={
        "train": f"{base}/train.csv",
        "validation": f"{base}/valid.csv",
        "test": f"{base}/test.csv",
    }
)
print(ds["train"][0])
`

محدودیت‌ها
- اندازه کوچک و پوشش محدود  
- احتمال نویز در برچسب‌ها  
- عدم توازن کامل بین وظایف  

استناد
`bibtex
@dataset{majid2025multitask,
  author = {Maid121232},
  title = {Majid Multi-task Dataset},
  year = {2025},
  url = {https://huggingface.co/datasets/Maid121232/majid-multitask-dataset}
}
`

---

تماس
ایجاد و به‌اشتراک‌گذاری توسط Maid121232 (مجید)
`

---

🔹 چرا لوگو آپلود نمی‌شه؟
چند دلیل رایج:
1. اسم فایل فارسی یا فاصله‌دار باشه → بهتره اسمش logo.png باشه.  
2. حجم زیاد یا فرمت اشتباه → فقط PNG/JPG/GIF پشتیبانی می‌شه.  
3. آپلود در پوشه‌ی اشتباه → باید در ریشه‌ی ریپو (هم‌سطح README.md) باشه.  
4. کش مرورگر → گاهی بعد از آپلود باید صفحه رو رفرش کنی تا نمایش داده بشه.  

---

✅ پیشنهاد: اسم فایل رو دقیقاً logo.png بذار، در ریشه‌ی ریپو آپلود کن، بعد لینک داخل README همون باشه.  

می‌خوای برات یک نسخه‌ی خیلی ساده‌تر از README هم آماده کنم (فقط انگلیسی + لوگو) تا اگر باز هم خطا گرفتی، اول با اون تست کنی؟