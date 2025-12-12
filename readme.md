**YouTube Video Summarizer**
==============================
<p align="center">
  <img src="https://img.shields.io/badge/LLM-Llama3.3_70B-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Groq-LPU_Inference-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Python-3.10+-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Streamlit-App-red?style=for-the-badge" />
</p>

A **smart YouTube summarization tool** that fetches transcripts, analyzes content, and generates clean **Short Summaries**, **Key Bullet Points**, and **Actionable Insights**, all powered by **Groq’s ultra-fast llama-3.3-70b-versatile**.

---

## 🚀 **Features**

- Paste any **YouTube link or video ID**
  
- Automatically fetches:
  - Title  
  - Channel name  
  - Thumbnail  
  - Transcript
    
- Generates:
  - **Short Summary** (3–5 sentences)
  - **Key Bullet Points**
  - **Actionable Insights**
    
- Clean, styled UI with:
  - 5 organized tabs  
  - Scrollable transcript viewer  
  - Copy-to-clipboard buttons without page reload
    
- Download summary as **TXT**
  
- Fully built with Python + Streamlit

---

## 🧰 **Tech Stack**
| Component | Used For |
|----------|----------|
| **Python 3.10+** | Core logic |
| **Groq API (llama-3.3-70b-versatile)** | AI summarization |
| **YouTube Transcript API** | Transcript fetching |
| **Requests** | Video metadata |
| **Streamlit** | Beautiful UI |
| **Inline HTML + CSS** | Custom styling & copy buttons |

---

## 📂 **Project Structure**
```
youtube_summarizer/
│── app.py               
│── requirements.txt
│── README.md
```

---

## 🖥️ **How It Works**

### **1️⃣ Input a YouTube URL**
✔ Paste a link or video ID  
✔ Click **Summarize Video**  

---

### **2️⃣ Transcript Extraction**
The app attempts multiple transcript types in order:

1. Manually created  
2. Auto-generated  
3. Alternate English transcripts  
4. Fallback to any available transcript  

If none exist → user gets a clean error.

---

### **3️⃣ AI Summary**
The model generates three sections:

- **Short Summary**
- **Key Bullet Points**
- **Actionable Insights**

Each section is formatted and styled automatically.

---

### **4️⃣ Organized Streamlit UI**
Five tabs:

1. 📝 Short Summary  
2. 📌 Key Bullet Points  
3. 💡 Actionable Insights  
4. 🗒️ Full Transcript  
5. ⬇️ Download  

Each content block includes a **Copy Content** button.

---

## ▶️ **Run Locally**

### **Install Dependencies**
```
pip install -r requirements.txt
```

---

### **Launch the Streamlit App**
```
streamlit run app.py
```

---

## 🔑 **Setup Groq API Key**
</br>

>[!IMPORTANT]
>You must set your Groq API key as an environment variable.
>If you get any model error, you need to update the model version as they get decommissioned

</br>
Login to your groq dashborad and then create new API key. Copy that key and then set it as an environment variable using:

### **Mac/Linux (bash/zsh)**
```
export GROQ_API_KEY="your_api_key_here" 
```
### **Windows Powershell**
```
setx GROQ_API_KEY "your_api_key_here" 
```

After that Then restart your terminal and verify:
```
echo $env:GROQ_API_KEY
```
---

## 📝 **Example Input**
### YouTube URL
```
https://youtu.be/DylXv4J95Tg?si=tvHdQBeRSUjmD0yX
```

---

## ⭐ **Future Improvements**

* Chapter-wise summaries  
* Multi-language support  
* PDF export  
* More summary modes (Twitter thread, essay, ELI5, etc.)  
* Browser extension version  
* SaaS-ready authentication version  

---

## 🤝 **Contributing**

Pull requests welcome!\
If you want to help improve this tool or build a SaaS version, reach out.

---

## 📹 **Demo Video**

Coming soon on YouTube 📺

---

## 📬 **Contact**

For customization or freelance work, reach out anytime.

---

## 📄 **License**

MIT
