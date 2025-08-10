Download Latest Update Link: https://github.com/gajamedia/Kecerdasan_Buatan/releases/download/hAI-v2.5.32/hAI-v2.5.32.zip

Ini adalah project Kecerdasan Buatan Tahap awal yang saya kembangkan berbasis console mode, berikut penjelasan mengenai fitur-fitur apa saja di tahap awal ini (Console Base):

🧠 AI Agent: Adaptif, Generatif, dan Belajar Mandiri AI Agent ini adalah sistem pencarian jawaban cerdas berbasis Python yang menggabungkan pendekatan retrieval (berbasis kemiripan teks) dan generative response untuk memberikan jawaban yang alami, kontekstual, dan bisa berkembang melalui interaksi pengguna.

✨ Fitur Utama ✅ Adaptif terhadap Input Pengguna Menggunakan berbagai teknik kemiripan:

Jaccard Similarity
Semantic Weighted Matching
Levenshtein Distance
BERT Embedding (dengan retrain otomatis) Sistem akan memilih jawaban terbaik berdasarkan kombinasi skor dan tingkat kemiripan adaptif terhadap panjang pertanyaan.
✨ Generatif dan Responsif terhadap Nada (Tone) Jawaban tidak hanya diambil mentah, tetapi diproses ulang melalui generate_response() yang akan:

Memparafrase secara ringan
Menyesuaikan gaya bahasa (formal, santai, humor, bijak)
Menambahkan konteks tambahan bila ada
Menggabungkan jawaban dari beberapa sumber
📚 Multi-layer Response Generator Dapat menghasilkan:

Jawaban paragraf
Bullet list (multi-point)
Ringkasan padat
Gabungan dari lokal + Firebase
🔒 Mode Privat Dengan private_mode on, Anda bisa mencegah penyimpanan jawaban ke Firebase secara otomatis.

📖 Auto-Learning Jika sistem tidak tahu jawabannya, AI akan bertanya ke user dan menyimpannya secara lokal (dan Firebase jika diizinkan). Jawaban baru ini otomatis dilatih ulang pada model BERT agar bisa dipahami ke depannya.

📈 Logging & Debug Mode Setiap interaksi terekam dalam log_agent.txt secara transparan dan dapat dianalisis.

🚀 Teknologi yang Digunakan Python (>=3.10) Transformers (HuggingFace) Safetensors SentenceTransformer / BERT Firebase Realtime Database Custom NLP pipeline (tokenizer, normalizer, similarity scoring)

🤖 Apakah Ini AI Generatif dan Adaptif? 

sistem ini masih bersifat semi-generati walau sudah Tidak sekadar mencocokkan pertanyaan, Mampu menggabungkan info dari berbagai sumber, Output disesuaikan gaya dan konteks pengguna
bersifat adaptif, karena belajar dari pengalaman dan menyesuaikan strategi pencarian berdasarkan input pengguna yang terus berubah.

ROADMAP:

Level	        Fitur / Ide	Deskripsi	Status

🟢 Dasar	    Rule-based Response	Jawaban berdasarkan keyword & intent manual	✅ 
	            TF-IDF Matching	Pencocokan makna pakai TF-IDF manual	✅ 
	            Logging Interaksi	Simpan riwayat pertanyaan & jawaban	✅ 
	            Sinonim & Normalisasi	Ubah kata ke bentuk umum	✅

🟡 Menengah	  🔄 Feedback Loop Auto-Retrain	Otomatisasi pembelajaran dari user feedback	
	            📌 Saran Pertanyaan Mirip	Saat tidak ketemu intent, beri saran mirip	
	            📊 Visualisasi Log	Dashboard Flask atau Matplotlib
	            📂 UUID & Metadata	Logging + analisa berdasarkan pertanyaan unik	✅

🔵 Lanjut	    🎯 Intent Classifier	Deteksi intent otomatis pakai ML (FastText, sklearn)
	            🤖 Fallback GPT API	External sebagai jawaban fallback
	            🧠 Memory Reasoning	Beri jawaban berdasarkan riwayat sesi
	            🔍 Dense Embedding IR	Pencarian dokumen pakai vector dense (BERT/FAISS)
               		Auto-Retrain (BERT Embedding) ✅

🟣 Advanced	  🔗 RAG-style Retrieval	Kombinasi IR + LLM (RAG atau LangChain)
	            💬 RLHF-style Feedback	Reward jawaban berdasarkan user feedback
	            🎯 Context-aware Response	Jawaban dengan konteks diskusi sebelumnya
	            📷 OCR & Image Caption	Jawab pertanyaan dari gambar atau tulisan



