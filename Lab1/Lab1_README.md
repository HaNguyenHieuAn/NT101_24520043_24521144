# Lab 01: Mật mã học Cổ điển (Classical Cryptography)

> **Môn học:** An toàn mạng máy tính (NT101)  
> **Khoa:** Mạng máy tính và Truyền thông  
> **Trường:** Đại học Công nghệ Thông tin – ĐHQG-HCM (UIT)

---

## 📑 Mục lục
- [Giới thiệu & Mục tiêu](#-giới-thiệu--mục-tiêu)
- [Cấu trúc thư mục](#-cấu-trúc-thư-mục)
- [Danh sách nhiệm vụ](#-danh-sách-nhiệm-vụ)
- [Yêu cầu môi trường & Cài đặt](#-yêu-cầu-môi-trường--cài-đặt)
- [Hướng dẫn thực thi](#-hướng-dẫn-thực-thi)
- [Báo cáo chi tiết](#-báo-cáo-chi-tiết)

---

## 🎯 Giới thiệu & Mục tiêu

Bài thực hành giúp làm quen với các khái niệm nền tảng trong mật mã hóa khóa đối xứng/cổ điển, cơ chế hoạt động của các thuật toán thay thế và hoán vị, cùng các phương pháp thám mã (cryptanalysis):
* Hiểu và cài đặt các hệ mật mã cổ điển: Caesar, Mono-alphabetic Substitution, Playfair, Vigenère.
* Ứng dụng kỹ thuật phân tích tần suất (Frequency Analysis) và các độ đo thống kê (Index of Coincidence, Kasiski Examination, n-gram).
* Xây dựng các thuật toán tìm kiếm tối ưu (Hill Climbing / Simulated Annealing) để tự động phá mã khi chỉ biết ciphertext (Ciphertext-only attack).

---

## 📂 Cấu trúc thư mục

```text
Lab1/
├── Lab1_GroupXX_Report.pdf     # Báo cáo chi tiết dạng PDF
├── Lab1_README.md                   # Tài liệu hướng dẫn bài Lab 1
├── data/                       # Dữ liệu kiểm thử & văn bản mẫu
│   ├── task2.1_cipher.txt
│   ├── task2.2_cipher.txt
│   ├── task2.4_cipher.txt
│   └── task2.6_cipher.txt
└── src/                        # Mã nguồn các bài tập
    ├── task2_1_caesar.py
    ├── task2_2_freq_analysis.py
    ├── task2_3_auto_mono.py
    ├── task2_4_playfair.py
    ├── task2_5_vigenere.py
    ├── task2_6_crack_vigenere.py