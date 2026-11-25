# Lingo — AI Arabic Subtitle Translator for YouTube, Coursera & Udemy | No API Key Required

<p align="center">
  <strong>Translate video subtitles with ChatGPT Plus — No API Key Required.</strong><br>
  One learning experience. Three platforms. No language barriers.<br>
  <strong>ترجمة فيديوهات يوتيوب وكورسيرا ويوديمي بالذكاء الاصطناعي دون مفتاح API.</strong><br>
  <sub>Automatic mode is experimental; eligible ChatGPT Plus or Pro subscription and local helper required.</sub>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-22c55e?style=flat-square" alt="MIT License"></a>
  <img src="https://img.shields.io/badge/Status-Alpha-f59e0b?style=flat-square" alt="Alpha status">
  <img src="https://img.shields.io/badge/Chrome-Manifest%20V3-4285F4?style=flat-square&logo=googlechrome&logoColor=white" alt="Chrome Manifest V3">
  <img src="https://img.shields.io/badge/ChatGPT-Plus%20%2F%20Pro-10A37F?style=flat-square" alt="ChatGPT Plus or Pro for automatic subtitle translation">
  <img src="https://img.shields.io/badge/API%20Key-Not%20Required-10A37F?style=flat-square" alt="No personal API key required for automatic translation">
  <img src="https://img.shields.io/badge/Node.js-22%2B-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js 22+">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Coursera-Lingo-0056D2?style=for-the-badge&logo=coursera&logoColor=white" alt="Coursera Lingo">
  <img src="https://img.shields.io/badge/Udemy-Lingo-A435F0?style=for-the-badge&logo=udemy&logoColor=white" alt="Udemy Lingo">
  <img src="https://img.shields.io/badge/YouTube-Lingo-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube Lingo">
</p>

<p align="center">
  <a href="#supported-platforms">Platforms</a> ·
  <a href="#features">Features</a> ·
  <a href="#screenshots">Screenshots</a> ·
  <a href="#installation">Installation</a> ·
  <a href="#frequently-asked-questions">FAQ</a> ·
  <a href="#in-memory-of-hussein-abu-younis">Dedication</a> ·
  <a href="#العربية">العربية</a>
</p>

**Lingo** is an open-source Arabic subtitle translator for Chrome, designed to help you translate YouTube videos, Coursera lectures, and Udemy courses from English to Arabic. Its dedicated browser extensions display synchronized bilingual subtitles (English + Arabic), so you can understand educational content while following the original terminology.

> **Automatic AI translation without a personal API key:** With an eligible ChatGPT Plus or Pro subscription, Lingo is designed to translate video subtitles using your existing ChatGPT plan. Sign in with ChatGPT, connect the local helper, and start translating — no separate API billing setup or personal OpenAI API key is required. Automatic mode is experimental and subject to account eligibility and usage limits.

Lingo — إضافة ترجمة فيديوهات يوتيوب وكورسيرا ويوديمي إلى العربية، تدعم عرض الترجمة العربية والإنجليزية معًا والاستعانة بـ ChatGPT لترجمة النصوص المتاحة في الفيديو.

<p align="center">
  <img src="https://github.com/user-attachments/assets/8b2ec0f0-a241-440a-bd1c-43e27244d5c6" width="100%" alt="Coursera Lingo Chrome extension for English to Arabic video subtitle translation and bilingual captions">
</p>

## About Lingo

Learn programming, engineering, IT, languages, and other subjects without relying on English alone. Lingo reads available English subtitle tracks and displays synchronized Modern Standard Arabic captions alongside the original text.

The project offers dedicated browser extensions for **Coursera, Udemy, and YouTube**, built around the same core features, interface philosophy, and performance goals. This repository documents the **Coursera Lingo** edition.

Lingo supports a manual translation workflow using imported subtitle files and is designed to support automatic translation through a local ChatGPT OAuth connector for eligible accounts. No video downloading, audio transcription, or dubbing is included.

> [!IMPORTANT]
> **Alpha release:** The manual import/export workflow is available to try. Automatic ChatGPT sign-in and end-to-end translation require the complete local server and verification before distribution. The Coursera extension is not available on the Chrome Web Store.

## Supported platforms

| Extension | Platform | Experience |
| :--- | :--- | :--- |
| **Coursera Lingo** | Coursera | English-to-Arabic subtitle translator for lectures, courses, and professional certificates. |
| **Udemy Lingo** | Udemy | Arabic subtitles for Udemy courses, programming lessons, and tutorials. |
| **YouTube Lingo** | YouTube | English-to-Arabic subtitle translation for YouTube videos and educational content. |

All three editions are designed to deliver a consistent experience: synchronized Arabic and English captions, customizable subtitles, convenient translation workflows, and efficient local caching. Actual compatibility and performance may vary with the platform, subtitle format, video length, and translation provider.

### Translate YouTube videos to Arabic — YouTube Lingo

A dedicated YouTube subtitle translation extension for learners who want Arabic captions alongside the original English subtitles. Follow captioned tutorials, technical lessons, and educational videos without switching between the video and a separate translation window.

### Translate Coursera courses to Arabic — Coursera Lingo

A Chrome extension for translating Coursera lecture subtitles into Arabic while retaining the original English text. Designed for university courses, professional certificates, and technical subjects where bilingual terminology is useful.

### Translate Udemy courses to Arabic — Udemy Lingo

A dedicated Udemy course subtitle translator for Arabic-speaking learners, with the same core bilingual caption features and translation workflow as the other Lingo editions.

## Features

| Feature | Description |
| :--- | :--- |
| **Bilingual subtitles** | Display synchronized Arabic and English captions together. |
| **Customizable appearance** | Adjust subtitle font size and position. |
| **Manual ChatGPT workflow** | Export translation requests and import translated JSON files. |
| **Subtitle file support** | Import timed VTT and SRT files; export VTT. |
| **Translation validation** | Validate segment IDs to prevent missing or duplicated entries. |
| **Local caching** | Cache translations for up to eight lectures in the Coursera edition. |
| **Automatic translation** | Designed for batch translation with pause and resume through the local connector using an eligible ChatGPT Plus or Pro plan, without a personal API key (experimental). |
| **Arabic-first interface** | Arabic interface with support for Modern Standard Arabic. |

## Screenshots

<p align="center">
  <img src="https://github.com/user-attachments/assets/393c0d77-3bfe-4a18-9acf-6fee99d76dfd" width="44%" alt="Coursera Arabic subtitle translator Chrome extension Arabic user interface">
  &nbsp;
  <img src="https://github.com/user-attachments/assets/0cae309a-963a-4e61-8b32-c3fdb5d79a22" width="44%" alt="Coursera Lingo bilingual English Arabic video captions and translation controls">
</p>

<p align="center"><em>A closer look at the Arabic-first Coursera Lingo interface.</em></p>

## Installation

The following instructions apply to the Coursera edition. Use the corresponding extension files for Udemy or YouTube.

### 1. Install the extension

1. Download or clone this repository and extract it if necessary.
2. Open `chrome://extensions` in Chrome.
3. Enable **Developer mode**.
4. Select **Load unpacked** and choose the `extension/` directory containing `manifest.json`.
5. Open a Coursera lecture you are authorized to access that has English subtitles.

### 2. Choose a translation mode

#### Manual mode — no local server required

1. Click **Lingo · ترجمة**, then **قراءة النص الأصلي**.
2. Click **تصدير طلب لـ ChatGPT**.
3. Upload the generated request to ChatGPT and request a JSON file preserving every numeric `id`.
4. Click **استيراد ترجمة** and select the resulting JSON file. Alternatively, import a matching VTT or SRT file.
5. Play the lecture with synchronized bilingual subtitles.

> [!TIP]
> Long lectures may need to be split into smaller translation requests. Preserve all IDs and combine the translated entries before importing.

#### Automatic mode — experimental

Requires the complete `server/` implementation, Node.js 22 or newer, and an eligible **ChatGPT Plus or Pro subscription**. No personal OpenAI API key, API credits purchase, or separate API billing setup is required when using the supported Sign in with ChatGPT integration. These steps describe the intended workflow; they do not establish that the connector is working.

1. Install [Node.js](https://nodejs.org/).
2. On Windows, run `START.cmd` from the project root and leave the window open.
3. Open extension settings and enter the local connector key displayed by the helper.
4. Click **Continue with ChatGPT** and complete sign-in and consent on OpenAI's website.
5. Refresh the connection status, open a lecture, load its English subtitles, load the available models, and choose one.
6. Start translation.

Requests use the eligible account's ChatGPT plan usage limits. Unlimited translation is not guaranteed. The local connector key in step 3 is not an OpenAI API key. See the [official OpenAI integration documentation](https://developers.openai.com/siwc/token-sharing-open-source) for current requirements.

## Frequently asked questions

### How can I translate YouTube videos from English to Arabic?

Use the YouTube Lingo edition with a video that has a supported, accessible English caption track. Lingo is designed to display the translated Arabic subtitles with the original English captions.

### Is there a Chrome extension to translate Coursera and Udemy courses into Arabic?

Yes. Coursera Lingo and Udemy Lingo are dedicated editions for these platforms. This repository documents Coursera Lingo; the Udemy and YouTube editions require their corresponding extension files.

### Can I translate video subtitles with ChatGPT?

Yes. The Coursera edition supports exporting a translation request and importing the translated JSON file manually. Automatic ChatGPT translation through the local connector is experimental and requires a complete, verified helper and an eligible account.

### Do I need an OpenAI API key to translate videos automatically with ChatGPT Plus?

No. The intended automatic workflow uses Sign in with ChatGPT and an eligible ChatGPT Plus or Pro subscription. You do not need to create a personal API key or configure separate API billing. The local helper must be installed and working, and translation is subject to your plan’s usage limits.

### Is Lingo free and open source?

The project is released under the MIT License. Manual mode does not require the local server. Translation services may have their own fees, account requirements, and usage limits.

### Does Lingo translate videos without subtitles or dub the audio?

No. Lingo relies on supported subtitle tracks or matching imported subtitle files. It does not download videos, transcribe speech, or generate dubbed audio.

## Limitations

- Requires an accessible English subtitle track in a supported format; it does not transcribe or dub audio.
- Arabic is the fixed target language in this version.
- Picture-in-Picture and fullscreen on the video element itself do not display the extension overlay in the Coursera edition.
- Reloading a page stops subsequent translation batches; an in-flight request may still consume usage.
- Automatic mode requires a working local helper and an eligible account; sign-in and translation have not been independently verified in this release preparation.
- Subtitle accuracy depends on the translation model and should be reviewed for technical terminology.
- Platform-specific compatibility and performance may differ between editions.

## Privacy and security

The Coursera extension reads subtitle tracks from the course page and stores translations in Chrome extension-local storage. Automatic translation is intended to send subtitle text to OpenAI only when requested. Manual mode sends no translation requests directly to OpenAI.

The extension connects to a local helper at `127.0.0.1:43127` using a local connector key. Never enter your ChatGPT password into the extension or publish local keys, account records, OAuth tokens, or private subtitle files.

The local server's credential handling must be verified against its source before automatic mode is released. Users should only process content they are authorized to use and comply with the relevant platform terms.

## In memory of Hussein Abu Younis

<p align="center">
  <img src="https://img.shields.io/badge/IN%20LOVING%20MEMORY-Hussein%20Abu%20Younis-334155?style=for-the-badge" alt="In loving memory of Hussein Abu Younis">
</p>

<h3 align="center">إلى روح صديقي حسين أبو يونس</h3>

<p align="center" dir="rtl">
  رحل عن الدنيا، لكن للذكرى حياةٌ أخرى في كل خيرٍ يبقى.<br><br>
  أهدي هذا المشروع إلى روح صديقي <strong>حسين أبو يونس، رحمه الله</strong>،<br>
  راجيًا من الله أن يجعل كل معرفةٍ يكتسبها إنسان، وكل حاجزٍ لغوي يتجاوزه متعلّم،<br>
  علمًا نافعًا وصدقةً جاريةً في ميزان حسناته.<br><br>
  <strong>اللهم اغفر له وارحمه، واجعل أثره الطيب باقيًا لا ينقطع.</strong>
</p>

<p align="center">
  Dedicated to the memory of my friend, <strong>Hussein Abu Younis</strong>.<br>
  May every lesson understood and every barrier overcome through this project<br>
  become part of a lasting legacy of knowledge, kindness, and hope.
</p>

<p align="center"><em>Some legacies live on through the knowledge we share.</em><br>بعض الأثر لا ينقطع، ما دام العلم يُنتفع به.</p>

---

## Project structure

```text
coursera-lingo/
├── extension/           # Chrome Manifest V3 extension
├── server/              # Local helper (required for automatic mode)
├── scripts/             # Development checks
├── tests/               # Automated tests
├── START.cmd            # Windows launcher
├── package.json
├── package-lock.json
├── .gitignore
├── LICENSE
└── README.md
```

The server, scripts, and tests must be included in the repository before claiming a complete automatic-mode release.

## Development

Once the full source tree is available:

```bash
npm ci
npm run check
npm test
npm start
```

## Roadmap

- [ ] Verify complete OAuth login, consent, logout, and inference with an eligible test account.
- [ ] Test compatibility across Coursera, Udemy, and YouTube content and supported browsers.
- [ ] Benchmark performance and translation consistency across all three editions.
- [ ] Add installation screenshots and short demos using authorized content.
- [ ] Add more target languages and improve technical terminology consistency.
- [ ] Prepare Chrome Web Store releases after security and compatibility reviews.

## Contributing

Bug reports, feature requests, and pull requests are welcome. Please include browser and Node.js versions, the affected Lingo edition, reproducible steps, and sanitized error messages. Never include tokens, local connector keys, account details, or private transcripts in issues.

## العربية

<div dir="rtl" align="right">

### إضافة ترجمة فيديوهات يوتيوب وكورسيرا ويوديمي للعربية باستخدام ChatGPT — بدون مفتاح API

Lingo مشروع مستقل ومفتوح المصدر، يهدف إلى جعل المحتوى التعليمي الأجنبي أكثر سهولة للمتعلم العربي، من خلال عرض النص الإنجليزي والترجمة العربية المتزامنة مع الفيديو.

### إضافات Lingo

- **Coursera Lingo:** لترجمة المحاضرات والدورات على منصة كورسيرا.
- **Udemy Lingo:** لترجمة الدورات التعليمية على منصة يوديمي.
- **YouTube Lingo:** لترجمة الفيديوهات والمحتوى التعليمي على يوتيوب.

تقدم الإضافات الثلاث تجربة موحدة مبنية على الخصائص الأساسية نفسها، مع استهداف مستوى الأداء نفسه: عرض الترجمة الثنائية، تخصيص مظهر النص، استيراد وتصدير الترجمات، وحفظها محليًا. وقد تختلف سرعة التنفيذ والتوافق الفعلي باختلاف المنصة ومصدر الترجمة.

### كيفية ترجمة الفيديوهات والدورات باستخدام ChatGPT

يمكن استخدام الوضع اليدوي دون تشغيل المساعد المحلي: افتح الإضافة، اقرأ النص الأصلي، صدّر طلب الترجمة إلى ChatGPT، ثم استورد ملف الترجمة الناتج بصيغة JSON. كما يمكن استيراد ملفات VTT وSRT المتوافقة.

### الترجمة التلقائية باستخدام ChatGPT Plus بدون مفاتيح API

**لا تحتاج إلى إنشاء مفتاح OpenAI API أو إعداد فوترة API منفصلة.** يكفي من ناحية الاشتراك أن يكون لديك حساب ChatGPT Plus مؤهل (أو Pro)، مع تثبيت المساعد المحلي وتشغيله، ثم تسجيل الدخول بحساب ChatGPT والموافقة على الربط وبدء الترجمة.

تظل هذه الميزة تجريبية حتى التحقق من عمل الربط، وتخضع الترجمة لحدود استخدام اشتراكك. مفتاح الاتصال بالمساعد المحلي ليس مفتاح OpenAI API.

### أسئلة شائعة

**كيف أترجم فيديو يوتيوب إلى العربية؟** استخدم إصدار YouTube Lingo مع فيديو يحتوي على ترجمة إنجليزية متاحة ومدعومة.

**هل توجد إضافة لترجمة كورسات كورسيرا ويوديمي إلى العربية؟** نعم، يوفر المشروع إصدار Coursera Lingo وإصدار Udemy Lingo لعرض الترجمة العربية بجانب النص الإنجليزي. هذا المستودع يوثق إصدار كورسيرا، وتحتاج الإصدارات الأخرى إلى ملفاتها الخاصة.

**هل أحتاج إلى مفتاح API لترجمة فيديوهات يوتيوب أو كورسيرا أو يوديمي تلقائيًا؟** لا يحتاج مسار الربط المدعوم إلى مفتاح API شخصي؛ يعتمد الوضع التلقائي المصمم على اشتراك ChatGPT Plus أو Pro مؤهل ومساعد محلي يعمل بصورة صحيحة.

**هل الإضافة مجانية؟** المشروع مفتوح المصدر بترخيص MIT، لكن خدمات الترجمة الخارجية تخضع لشروطها وحدود استخدامها وتكاليفها المحتملة.

</div>

---

## License and disclaimer

Released under the **MIT License** — see [LICENSE](LICENSE).

Lingo is an independent community project. It is not affiliated with, endorsed by, or an official product of Coursera, Udemy, YouTube, Google, or OpenAI. All third-party names and trademarks belong to their respective owners. The software license does not grant rights to third-party content.
