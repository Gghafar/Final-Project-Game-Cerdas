# 🧟‍♂️ [Final Project Game Cerdas] (Project TDS)

![Platform](https://img.shields.io/badge/Platform-PC%20(Windows)-blue)
![Engine](https://img.shields.io/badge/Engine-Unity%202021-black?logo=unity)
![Status](https://img.shields.io/badge/Status-Educational%20Project-green)

> *Sebuah purwarupa game Top-Down Shooter 3D untuk bertahan hidup dari serangan zombie, dibangun sebagai implementasi logika pathfinding dan manajemen objek di Unity.*

---

## 📖 Tentang Proyek
Proyek ini dikembangkan sebagai bagian dari pembelajaran pengembangan game 3D. Fokus utama dari proyek ini adalah membangun mekanik pertempuran yang solid (*combat mechanics*) dan sistem musuh yang responsif.

Berbeda dengan game balap, proyek ini mengeksplorasi penggunaan **Raycasting** untuk sistem penembakan presisi dan **NavMesh** untuk pergerakan AI musuh yang mengejar pemain secara *real-time*.

---

## 🚀 Fitur Utama

Fitur-fitur teknis yang diimplementasikan dalam proyek ini meliputi:

* **Wave Spawning System**: Musuh muncul secara bertahap dengan kesulitan yang meningkat, dikelola oleh script manager terpusat.
* **Raycast Shooting Mechanics**: Sistem penembakan menggunakan *Raycast* (sinar tak terlihat) untuk mendeteksi hit yang akurat dan instan, memberikan *feedback* visual berupa efek partikel.
* **Intelligent AI Tracking**: Musuh (Zombie) diprogram menggunakan **Unity NavMesh Agent** untuk mencari jalur terpendek menuju pemain, menghindari rintangan statis (tembok/objek).
* **Pickup & Resource Management**: Sistem *loot* sederhana di mana pemain harus memanajemen kesehatan (Health) dan amunisi melalui item pickup.

---

## 🎮 Preview Gameplay

*(Screenshot hasil pengembangan)*

<div align="center">
  <img width="815" height="460" alt="Screenshot 2025-12-16 215548" src="https://github.com/user-attachments/assets/b8cddee9-e41e-496e-8bbb-65d64bf41a4b" />
  <img width="815" height="460" alt="Screenshot 2025-12-16 215548" src="https://github.com/user-attachments/assets/acb97b52-2111-4c52-a25b-1fc1e8eab3fd" />
  <img width="819" height="461" alt="Screenshot 2025-12-16 215528" src="https://github.com/user-attachments/assets/57ce3949-d99f-4795-a6a3-487f8df9d3e9" />
  <img width="819" height="461" alt="Screenshot 2025-12-16 215528" src="https://github.com/user-attachments/assets/e11ade75-a411-4be3-811f-b8583a5e74eb" />
</div>

---

## 🕹️ Kontrol Permainan

Game dirancang untuk dimainkan menggunakan Mouse dan Keyboard dengan skema klasik:

| Input | Fungsi |
| :--- | :--- |
| **W-A-S-D** | Pergerakan Karakter |
| **Mouse Cursor** | Mengarahkan Pandangan (Aiming) |
| **Klik Kiri** | Menembak (Shoot) |
| **R** | Reload Senjata |
| **Numpad 1/2** | Ganti Senjata |

---

## 🛠️ Tech Stack & Implementasi

Berikut adalah rincian teknis yang digunakan dalam kode (C#):

1.  **AI Navigation**: Menggunakan komponen `NavMeshAgent` standar Unity.
2.  **Shooting Logic**:
    * Menggunakan `Physics.Raycast` untuk deteksi tembakan.
    * `LineRenderer` digunakan untuk visualisasi jejak peluru (tracer effect).
3.  **UI Management**: Menggunakan Canvas Scaler untuk menampilkan HP bar dan skor.
4.  **Finite State Machiine**: Digunakan untuk mengatur/mengontrol tingkah laku musuh.


---

* Developed by: **[Danial Rajiv Syahidan, Gandrung Ghafar, Dhafin Kurniawan]**
