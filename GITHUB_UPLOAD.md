# GitHub'a Yükleme Talimatları

## Proje Yapısı (GitHub'a Yüklenecek)

```
Consumer-Complaints-Classification/
├── notebooks/
│   └── COMPLETE_ANALYSIS.ipynb           # Tam analiz notebook
│
├── results/
│   ├── 04_model_comparison_4models.png
│   ├── learning_curves.png
│   ├── confusion_matrix.png
│   └── 05_optimization_comparison.png
│
├── data/                                 # (opsiyonel - boş olabilir)
│
├── README.md                             # Proje açıklaması
├── FINAL_RESULTS.md                      # Detaylı sonuçlar
├── QUICKSTART.md                         # Hızlı başlangıç
├── requirements.txt                      # Bağımlılıklar
└── .gitignore                            # Git yok saydığı dosyalar
```

---

## 1. Git Repository Oluştur

### GitHub'da yeni repository oluştur:
1. https://github.com/new adresine git
2. Repository adı: `Consumer-Complaints-Classification`
3. Description: "Text classification with machine learning optimization"
4. Public seç
5. "Create repository" tıkla

### Aldığın komutlar şöyle görünecek:
```bash
git config --global user.name "Serhat Aslan"
git config --global user.email "your.email@example.com"
```

---

## 2. Proje Klasöründe Git'i İnit Et

```bash
cd c:\Users\serha\Desktop\Wum Project

# Git repository başlat
git init

# Remote repository ekle (YOUR_USERNAME ve YOUR_REPO_NAME değiştir)
git remote add origin https://github.com/YOUR_USERNAME/Consumer-Complaints-Classification.git

# Ana branch ismi ayarla
git branch -M main
```

---

## 3. Dosyaları Hazırlayıp Yükle

```bash
# Tüm dosyaları ekle
git add .

# Değişiklikleri kontrol et
git status

# Commit et
git commit -m "Initial commit: Complete text classification project with optimization"

# GitHub'a push et
git push -u origin main
```

---

## 4. GitHub'da Kontrol Et

- https://github.com/YOUR_USERNAME/Consumer-Complaints-Classification adresine git
- Dosyaları gözden geçir
- README.md'nin düzgün göründüğünü kontrol et

---

## İçinde Olacaklar

✅ **COMPLETE_ANALYSIS.ipynb**
- 22 hücre
- Tüm analiz bir notebook'ta
- 4-model karşılaştırması
- 3 optimizasyon tekniği
- Sonuçlar ve görselleştirmeler

✅ **Sonuç Grafikleri** (`results/`)
- 4-model karşılaştırması
- Learning curves
- Confusion matrix
- Optimizasyon karşılaştırması

✅ **Dokümantasyon**
- README.md - Proje özeti
- FINAL_RESULTS.md - Detaylı analiz
- QUICKSTART.md - Kurulum & çalıştırma

---

## GitHub URL Yapısı

```
https://github.com/YOUR_USERNAME/Consumer-Complaints-Classification
```

Örnek:
```
https://github.com/serhahaslan/Consumer-Complaints-Classification
```

---

## İpuçları

1. **SSH Key Kullan** (Opsiyonel):
   ```bash
   git remote set-url origin git@github.com:YOUR_USERNAME/Consumer-Complaints-Classification.git
   ```

2. **Eğer Yanlış Yapılırsa Reset**:
   ```bash
   git reset --hard HEAD~1
   ```

3. **Branch Kontrol**:
   ```bash
   git branch -a
   git log --oneline
   ```
