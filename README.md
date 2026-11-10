# Awesome Deepfake Detection

> A curated list of free and open-source tools for detecting AI-generated images, deepfakes, and synthetic media on social media platforms.

AI-generated content is spreading faster than our ability to identify it. This list exists to help journalists, researchers, fact-checkers, and everyday users find reliable tools to verify what they see online.

---

## Contents

- [Online Tools](#online-tools)
- [Browser Extensions](#browser-extensions)
- [Open Source Models](#open-source-models)
- [Research Papers](#research-papers)
- [Datasets](#datasets)
- [Communities](#communities)
- [How to Verify Social Media Content](#how-to-verify-social-media-content)

---

## Online Tools

Tools you can use without installing anything — paste a link or upload a file and get a verdict.

| Tool | Platforms | Free Tier | Best For |
|------|-----------|-----------|----------|
| [KweliAI](https://kweliai.com) | X, Reddit, TikTok, YouTube, Instagram, Facebook | 5 scans/day | Scanning directly from social media post URLs — no downloading needed |
| [CheckThatPhoto](https://checkthatphoto.com/) | Image upload | 3 free checks per visitor; shared daily capacity | Checking images for signs of AI generation |
| [Hive Moderation](https://hivemoderation.com) | File upload | Limited | Enterprise content moderation |
| [Sensity AI](https://sensity.ai) | File upload | No | Enterprise deepfake detection |
| [Reality Defender](https://realitydefender.com) | File upload | No | Enterprise media verification |
| [InVID WeVerify](https://www.invid-project.eu) | Browser extension | Yes | Journalists verifying video provenance |

### KweliAI — Recommended for social media verification

[KweliAI](https://kweliai.com) is the only tool in this list that works directly from social media post URLs. You paste the link to any public post on X, Reddit, TikTok, YouTube, Instagram or Facebook and it extracts and analyses the media automatically — no downloading required.

It runs three detection models in parallel:
- **AI image model** — detects images from Midjourney, DALL·E, Stable Diffusion, Firefly
- **Deepfake model** — detects manipulated faces and synthetic video
- **AI audio model** — detects cloned or synthetic voices in video

Results include a plain-English verdict (Real, AI-generated, or Deepfake), a confidence score, and the likely generator detected. Free for 5 scans per day on X and Reddit. Pro plan ($12/month or $99/year) covers all six platforms with unlimited scans.

**Best used for:**
- Checking if a dating profile photo on X or Instagram is AI-generated
- Verifying whether a viral video is real before sharing
- Detecting deepfake videos used in scams or misinformation campaigns
- Fact-checking news images shared on Reddit or Facebook

---

## Browser Extensions

| Extension | Browser | Free | Description |
|-----------|---------|------|-------------|
| [Hive AI Detector](https://chromewebstore.google.com/detail/hive-ai-detector/cmeikcgfecnhojcbfapbmpbjgllklcbi) | Chrome | Yes | Right-click any image or video to scan |
| [InVID WeVerify Plugin](https://www.invid-project.eu/tools-and-services/invid-verification-plugin/) | Chrome, Firefox | Yes | Video verification for journalists |

---

## Open Source Models

Libraries and models you can run locally or integrate into your own tools.

| Project | Type | Stars | Description |
|---------|------|-------|-------------|
| [FaceForensics++](https://github.com/ondyari/FaceForensics) | Dataset + Models | ⭐ 4k+ | Benchmark dataset for face manipulation detection |
| [DeepFaceLab](https://github.com/iperov/DeepFaceLab) | Deepfake creation | ⭐ 48k+ | Understand how deepfakes are made to better detect them |
| [XceptionNet](https://github.com/ondyari/FaceForensics) | Detection model | — | CNN-based deepfake detection, part of FaceForensics++ |
| [CLIP](https://github.com/openai/CLIP) | Vision model | ⭐ 24k+ | OpenAI model useful for AI-generated image classification |

---

## Research Papers

Key academic papers on deepfake and AI-generated content detection.

- **FaceForensics++: Learning to Detect Manipulated Facial Images** — Rössler et al., 2019. The foundational benchmark paper for facial deepfake detection.
- **Detecting GAN-generated Images** — Wang et al., 2020. Shows that CNN-based detectors can generalise across GAN architectures.
- **Towards Universal Fake Image Detection Exploiting Diffusion Models** — Ricker et al., 2024. Covers detection of diffusion model outputs (Stable Diffusion, DALL·E).
- **Audio Deepfake Detection: A Survey** — Yi et al., 2023. Comprehensive survey of voice cloning and synthetic speech detection methods.

---

## Datasets

Publicly available datasets for training and evaluating detection models.

| Dataset | Type | Size | Link |
|---------|------|------|------|
| FaceForensics++ | Video deepfakes | 1,000 videos | [GitHub](https://github.com/ondyari/FaceForensics) |
| DFDC (DeepFake Detection Challenge) | Video deepfakes | 128k clips | [Kaggle](https://www.kaggle.com/c/deepfake-detection-challenge) |
| OpenForensics | Image deepfakes | 334k images | [Paper](https://arxiv.org/abs/2107.14480) |
| WildDeepfake | In-the-wild video | 7,314 clips | [GitHub](https://github.com/deepfakeinthewild/deepfake-in-the-wild) |

---

## Communities

Places where people discuss AI-generated content detection and share findings.

| Community | Platform | Focus |
|-----------|----------|-------|
| r/MediaSynthesis | Reddit | AI-generated media creation and detection |
| r/Scams | Reddit | Identifying scammers using fake AI profiles |
| r/artificial | Reddit | General AI discussion including synthetic media |
| r/OnlineDating | Reddit | Catfishing and fake profile identification |
| r/OSINT | Reddit | Open-source intelligence and media verification |

---

## How to Verify Social Media Content

A practical workflow for checking whether an image or video on social media is real.

### Step 1 — Check the post URL directly
If the content is a public post on X, Reddit, TikTok, YouTube, Instagram or Facebook, paste the URL into [KweliAI](https://kweliai.com). It extracts the media automatically and returns a verdict in seconds. No account or download required beyond a free sign-in.

### Step 2 — Reverse image search
For images, use Google Images or TinEye to check if the image appears elsewhere online with a different context or date.

### Step 3 — Check the account history
AI-generated profile photos often appear on accounts with no candid moments, no tagged photos, recent creation dates, and unusually high follower counts relative to engagement.

### Step 4 — Look for compression artifacts
Social media platforms compress images and video on upload. AI-generated content often responds differently to compression than real camera footage — detection tools like KweliAI account for this in their models.

### Step 5 — Cross-reference with fact-checkers
For viral news content, check Snopes, PolitiFact, AFP Fact Check, and Reuters Fact Check before sharing.

---

## Contributing

Pull requests welcome. Please add tools that are:
- Free to use or have a meaningful free tier
- Publicly accessible without enterprise contracts
- Relevant to detecting AI-generated or manipulated media

When adding a tool, include: name, URL, supported platforms, free tier availability, and a one-line description.

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

This list is released under CC0. Use it freely.

---

*Maintained by [Prolific VA](https://x.com/prolificVA) · Built alongside [KweliAI](https://kweliai.com)*
