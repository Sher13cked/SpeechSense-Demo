# SpeechSense Demo

An interactive audio demo for **SpeechSense: A Paralinguistic-Focused Dataset for Fine-Grained Speech Sentiment Analysis**, presented at **ACM Multimedia (ACM MM) 2026**.

This website showcases 16 curated speech samples across eight fine-grained interpersonal stances, allowing visitors to explore how vocal delivery conveys attitudes beyond lexical content.

## Interactive Audio Gallery

The demo features eight interpersonal stance categories:

- **Confident** / **Nervous**
- **Passionate** / **Impatient**
- **Warm** / **Apathetic**
- **Sarcastic** / **Neutral**

Each category includes two audio samples with corresponding transcripts.

Visitors can switch between categories, listen to individual recordings, and compare how different attitudes are expressed through vocal cues such as pitch, rhythm, and voice quality.

## Project Structure

```text
SpeechSense-Demo/
├── index.html
├── styles.css
├── app.js
├── samples.json
├── audio/
│   ├── confident/
│   ├── nervous/
│   ├── warm/
│   ├── apathetic/
│   ├── passionate/
│   ├── impatient/
│   ├── sarcastic/
│   └── neutral/
└── README.md
```

Audio paths and transcripts are managed through `samples.json`.

## Local Preview

Run a local HTTP server from the repository root:

```bash
python3 -m http.server 8000
```

Then open:

http://localhost:8000/

Opening `index.html` directly from the file system may prevent the browser from loading `samples.json` due to local file access restrictions.

## GitHub Pages

The website is designed for deployment through GitHub Pages.

1. Open the repository's **Settings → Pages**.
2. Select **Deploy from a branch**.
3. Choose the `main` branch and `/(root)` directory.
4. Save the configuration.

Once deployed, the website is accessible through the repository's GitHub Pages URL.

## Features

- Responsive interface for desktop and mobile devices.
- Eight selectable interpersonal stance categories.
- Two curated audio samples per category, with transcripts.
- Automatic pausing of other audio players when a new sample starts.
- Collapsible paper abstract, initially expanded on desktop and collapsed on mobile.
- Direct links to the research paper, source code, and dataset.
- Lightweight static implementation using HTML, CSS, and JavaScript, without external frameworks or backend services.

## Dataset and Annotation

The SpeechSense Test Set contains **669 human-validated audio clips**, covering eight fine-grained interpersonal stances and 30 voice profiles.

The audio examples featured in this demo are selected from the SpeechSense Test Set. Their category assignments follow the human-validated labels rather than the original TTS generation targets.

For the complete dataset, annotations, and research methodology, refer to the resources below.

## Resources

- **Paper Arxiv:** https://arxiv.org/abs/2608.17931
- **Source Code:** https://github.com/Sher13cked/SpeechSense
- **Test Dataset:** https://huggingface.co/datasets/BruceW13/SpeechSense
- **Training Dataset:** https://huggingface.co/datasets/BruceW13/SpeechSense-Training

## Authors

**Shicheng Ma, Wenqian Cui, and Irwin King**

The Chinese University of Hong Kong

**ACM Multimedia 2026 · Rio de Janeiro, Brazil**

## License

The SpeechSense dataset is released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license. Refer to the original dataset repository for licensing and attribution details.