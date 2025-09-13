#Call Quality Analyzer
The Call Quality Analyzer is an end-to-end pipeline that evaluates customer call recordings to extract insights about **communication quality, engagement, and sentiment**. It combines **speech processing, diarization, and NLP** to deliver structured analysis from raw audio.

---

## 🔑 Features

* 🎧 **Audio Preprocessing** → resampling, normalization, noise reduction
* 🗣️ **Speaker Diarization** → separates customer vs. representative using `pyannote.audio`
* ✍️ **Automatic Speech Recognition (ASR)** → transcribes speech with Whisper
* 🧑‍🤝‍🧑 **Conversation Structuring** → maps transcripts to speakers with timestamps
* 📊 **Metrics Extracted**:

  * Talk-time ratio (rep vs. customer)
  * Longest monologue
  * Number of questions asked
  * Sentiment per speaker (positive/neutral/negative)
  * Keyword-based speaker validation
* 📝 **Insights Report** → interprets communication quality and coaching opportunities

---

## 🛠️ Tech Stack

* **Python**
* [yt-dlp](https://github.com/yt-dlp/yt-dlp) (audio download)
* [pydub](https://github.com/jiaaro/pydub), [noisereduce](https://github.com/timsainb/noisereduce) (audio processing)
* [pyannote.audio](https://github.com/pyannote/pyannote-audio) (speaker diarization)
* [Whisper](https://github.com/openai/whisper) (speech-to-text)
* [Transformers](https://huggingface.co/transformers) (sentiment analysis)

---

## 🚀 How It Works

1. Provide a YouTube call recording link or upload audio.
2. Audio is preprocessed and cleaned.
3. Speakers are separated and transcribed.
4. NLP pipeline extracts conversation metrics.
5. A structured **report + transcript** is generated.

---

## 📂 Output Example

* **Talk-Time Ratio**: Rep (65%) vs Customer (35%)
* **Sentiment**: Rep – Neutral, Customer – Negative
* **Insight**: “Rep dominated conversation. Few discovery questions asked. Customer sentiment indicates dissatisfaction.”

---

## 📌 Use Cases

* Sales call coaching
* Customer support quality analysis
* Conversation intelligence

---

## 🤝 Contributing

Pull requests and feature suggestions are welcome!

---

## 📜 License

This project is licensed under the MIT License.

---

👉 Do you want me to also add a **Setup & Installation guide (with pip commands + Colab support)** so that anyone can directly run your notebook?
