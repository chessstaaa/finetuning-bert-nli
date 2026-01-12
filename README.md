# Fine-tuning BERT for Natural Language Inference (MultiNLI)

Proyek ini merupakan implementasi fine-tuning **BERT-base-uncased** untuk tugas **Natural Language Inference (NLI)** menggunakan dataset **MultiNLI (MNLI)** dari GLUE Benchmark.

---

## 📌 Deskripsi Task

Natural Language Inference (NLI) bertujuan untuk menentukan hubungan antara sepasang kalimat (premise dan hypothesis) ke dalam tiga kelas:

- Entailment  
- Contradiction  
- Neutral  

Model dilatih untuk memprediksi apakah hipotesis merupakan konsekuensi logis dari premis, bertentangan, atau tidak dapat ditentukan.

---

## ⚙️ Konfigurasi Training

| Parameter | Nilai |
|----------|------|
| Model | bert-base-uncased |
| Max sequence length | 256 |
| Epochs | 3 |
| Learning rate | 2e-5 |
| Train batch size | 16 |
| Eval batch size | 32 |
| Weight decay | 0.01 |

---

## 📊 Ukuran Dataset

| Split | Jumlah Data |
|------|------------|
| Train | 392,702 |
| Validation (matched) | 9,815 |
| Validation (mismatched) | 9,832 |

---

## 📈 Hasil Evaluasi

| Split | Loss | Accuracy | Macro-F1 |
|------|-----|---------|----------|
| Validation (matched) | 0.5737 | 0.8446 | 0.8443 |
| Validation (mismatched) | 0.5500 | **0.8487** | 0.8481 |

---

## 🧠 Analisis Singkat

Model menunjukkan performa yang stabil baik pada domain yang sama (*matched*) maupun domain berbeda (*mismatched*).  
Perbedaan performa yang kecil menunjukkan kemampuan generalisasi yang baik pada data lintas domain.

---

## 📦 Teknologi yang Digunakan

- Python  
- PyTorch  
- HuggingFace Transformers  
- HuggingFace Datasets  
- Scikit-learn  

---

## 📌 Kesimpulan

Fine-tuning BERT pada dataset MultiNLI berhasil menghasilkan model inferensi bahasa alami dengan akurasi di atas 84%, membuktikan bahwa model mampu memahami hubungan semantik antar kalimat secara efektif.

## 🗂 Full Folder Link
https://drive.google.com/drive/folders/1KTsXJvW99pQiWfG9nfEpCYOAP_c5aNjq?usp=drive_link

The link contains:
1. Model folder
2. Notebook folder
3. Output folder
4. Reports folder
5. README.md
6. requirements.txt
