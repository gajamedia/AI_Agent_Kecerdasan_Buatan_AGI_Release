Download Link: https://github.com/gajamedia/AI_Agent_Kecerdasan_Buatan_AGI_Release/releases/download/hAI/hAI-v2.5.zip

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

🤖 Apakah Ini AI Generatif dan Adaptif? sistem ini bersifat semi-generatif, karena:

Tidak sekadar mencocokkan pertanyaan
Mampu menggabungkan info dari berbagai sumber
Output disesuaikan gaya dan konteks pengguna
bersifat adaptif, karena belajar dari pengalaman dan menyesuaikan strategi pencarian berdasarkan input pengguna yang terus berubah.
