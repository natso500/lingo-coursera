<h1 align="center">Coursera Lingo</h1>

<p align="center">
  <strong>Learn without language barriers.</strong><br>
  تعلّم دون حواجز لغوية.
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-green.svg" alt="MIT License"></a>
  <img src="https://img.shields.io/badge/status-alpha-orange" alt="Alpha status">
  <img src="https://img.shields.io/badge/Chrome-Manifest%20V3-blue" alt="Chrome Manifest V3">
  <img src="https://img.shields.io/badge/Node.js-22%2B-green" alt="Node.js 22+">
</p>

<p align="center">
  <a href="#features">Features</a> ·
  <a href="#screenshots">Screenshots</a> ·
  <a href="#installation">Installation</a> ·
  <a href="#roadmap">Roadmap</a> ·
  <a href="#العربية">العربية</a>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/8b2ec0f0-a241-440a-bd1c-43e27244d5c6" width="100%" alt="Coursera Lingo — main interface">
</p>

Coursera Lingo is an independent, open-source Chrome extension designed to make Coursera lectures more accessible to Arabic-speaking learners. It reads available English subtitle tracks and displays synchronized Modern Standard Arabic captions alongside the original English text.

The project is designed to support a local ChatGPT OAuth connector for eligible accounts, as well as a manual translation workflow using imported subtitle files. No video downloading or audio transcription is included.

> **Alpha status:** This is experimental software. Automatic ChatGPT sign-in and end-to-end translation must be verified with the complete local server before distribution. The extension can be tried using the manual import/export workflow. Not available on the Chrome Web Store.

## Features

- Synchronized Arabic and English captions.
- Adjustable subtitle font size and position.
- Manual ChatGPT translation request export and JSON import.
- Timed VTT and SRT import; VTT export.
- Validation of translated segment IDs to prevent missing or duplicated entries.
- Local translation cache for up to eight lectures.
- Designed for automatic translation in batches, with pause and resume via the local connector.
- Arabic user interface and support for Modern Standard Arabic.

## Screenshots

<p align="center">
  <img src="https://github.com/user-attachments/assets/393c0d77-3bfe-4a18-9acf-6fee99d76dfd" height="420" alt="Coursera Lingo interface — screenshot 1">
  &nbsp;&nbsp;
  <img src="https://github.com/user-attachments/assets/0cae309a-963a-4e61-8b32-c3fdb5d79a22" height="420" alt="Coursera Lingo interface — screenshot 2">
</p>

<p align="center"><em>A closer look at the Arabic-first extension interface.</em></p>

## Installation

### Manual translation mode (no local server required)

1. Download or clone the repository and extract it if necessary.
2. Open `chrome://extensions` in Chrome.
3. Enable **Developer mode**, select **Load unpacked**, and choose the `extension/` directory containing `manifest.json`.
4. Open a Coursera lecture you are authorized to access that has English subtitles.
5. Click **Lingo · ترجمة**, then **قراءة النص الأصلي**.
6. Click **تصدير طلب لـ ChatGPT**. Upload the generated request to ChatGPT and ask for a JSON file preserving every numeric `id`.
7. Click **استيراد ترجمة** and select the JSON file. Alternatively, import a matching VTT or SRT file.

Long lectures may need to be split into smaller translation requests. Keep all IDs intact and combine the translated entries before importing.

### Automatic translation mode (experimental)

Requires the complete `server/` implementation, Node.js 22 or newer, and an eligible ChatGPT account. The steps below describe the intended workflow; they do not establish that the connector is working.

1. Install [Node.js](https://nodejs.org/).
2. On Windows, run `START.cmd` from the project root and leave the window open.
3. Open the extension settings and enter the local connector key displayed by the helper.
4. Click **Continue with ChatGPT** and complete sign-in and consent on OpenAI's website.
5. Refresh the connection status, open a lecture, load its English subtitles, load the available models and choose one.
6. Start translation. Requests use the eligible account's usage limits; unlimited or free usage is not guaranteed.

See the [official OpenAI integration documentation](https://developers.openai.com/siwc/token-sharing-open-source) for current requirements.

## Limitations

- Requires an accessible English subtitle track in the supported Coursera format; it does not transcribe or dub audio.
- Arabic is the fixed target language in this version.
- Picture-in-Picture and fullscreen on the video element itself do not display the extension overlay.
- Reloading a page stops subsequent translation batches; an in-flight request may still consume usage.
- Automatic mode requires a working local helper and eligible account; sign-in and translation have not been independently verified in this release preparation.
- Subtitle accuracy depends on the translation model and should be reviewed for technical terminology.

## Privacy and security

The extension reads subtitle tracks from the Coursera page and stores translations in Chrome extension-local storage. Automatic translation is intended to send subtitle text to OpenAI only when requested; manual mode sends no translation requests directly to OpenAI. The extension connects to a helper at `127.0.0.1:43127` using a local connector key. Never enter your ChatGPT password into the extension or publish local keys, account records, OAuth tokens, or private subtitle files.

The local server's credential handling must be verified against its source before automatic mode is released. Users should only process educational content they are authorized to use and comply with the relevant platform terms.

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

- [ ] Verify complete OAuth login, consent, logout and inference with an eligible test account.
- [ ] Test across multiple Coursera courses and browsers.
- [ ] Add installation screenshots and a short demo using authorized content.
- [ ] Add more target languages and improve technical terminology consistency.
- [ ] Prepare a Chrome Web Store release after security and compatibility reviews.

## Contributing

Bug reports, feature requests and pull requests are welcome. Include browser and Node.js versions, reproducible steps and sanitized error messages. Never include tokens, local connector keys, account details or private course transcripts in issues.

## العربية

Coursera Lingo إضافة مستقلة ومفتوحة المصدر لمتصفح كروم، تساعد المتعلمين العرب على فهم المحاضرات من خلال عرض النص الإنجليزي والترجمة العربية المتزامنة مع الفيديو. تدعم استيراد JSON وVTT وSRT وتصدير VTT وحفظ الترجمات محليًا.

يمكن استخدام الوضع اليدوي دون تشغيل المساعد المحلي: افتح الإضافة، اقرأ النص الأصلي، صدّر طلب الترجمة إلى ChatGPT، ثم استورد ملف الترجمة الناتج. أما الوضع التلقائي فهو تجريبي ويتطلب استكمال ملفات المساعد والتحقق من تسجيل الدخول وأهلية الحساب.
هذا العمل عن روح صديقي حسين ابو يونس 

## License and disclaimer

MIT License — see [LICENSE](LICENSE).

This is an independent community project. It is not affiliated with, endorsed by, or an official product of Coursera or OpenAI. All third-party names and trademarks belong to their respective owners. The software license does not grant rights to third-party course content.
