# 💖 Y2K BMI Calculator (JavaFX MVC Application)
> Aplikasi kalkulator Indeks Massa Tubuh (BMI)
---
## 📸 Tampilan Aplikasi
<img width="320" height="512" alt="WhatsApp Image 2026-11-02 at 13 14 51" src="https://github.com/user-attachments/assets/02940b98-44c0-4096-bec9-8c0c9abe6078" />

- Video
https://github.com/user-attachments/assets/86709be7-3c5a-47c6-9d56-d43326897008
---
# 📍 Cara Menjalankan :

Pra-Syarat :
- JDK 17
- Apache Maven
- Git

clone repo:

git clone https://github.com/jezzyaa/Y2K-BMI-CALCULATOR.git

cd bmiCal

Run:
mvn clean javafx:run

## 📌 Deskripsi Proyek

**Y2K BMI Calculator** adalah aplikasi desktop interaktif yang membantu pengguna menghitung Indeks Massa Tubuh (BMI) berdasarkan input nama, gender, berat badan (kg), dan tinggi badan (cm).
---

## 🛠️ Penerapan Konsep Model-View-Controller (MVC)
   - **Model (`model.BmiCalc`)**: Menyimpan state data (nama, gender, berat, tinggi), mengisolasi rumus matematika BMI, serta menentukan kategori status tubuh.
   - **View (`BmiCalView.fxml`)**: Mendefinisikan antarmuka visual UI berbasis XML, komponen tata letak (`VBox`, `HBox`, `AnchorPane`), elemen SVG, dan CSS styling.
   - **Controller (`controller.BmiController`)**: Menghubungkan View dan Model, menangani event aksi tombol (`#handleCalculate`, `#handleReset`), serta mengelola dynamic styling.
---
## 📂 Struktur Direktori Proyek
```text
bmiCal/
├── src/
│   └── main/
│       ├── java/
│       │   ├── controller/
│       │   │   └── BmiController.java      # Controller penangan event & CSS
│       │   ├── main/
│       │   │   └── MainApp.java            # Entry point aplikasi JavaFX
│       │   └── model/
│       │       └── BmiCalc.java            # Logika bisnis & kalkulasi BMI
│       └── resources/
│           └── BmiCalView.fxml             # Tata letak UI (JavaFX FXML)
├
├── .gitignore                              # Konfigurasi pengabaian file Git
├── pom.xml                                 # Dependensi & konfigurasi Maven
└── README.md                               # Dokumentasi proyek
