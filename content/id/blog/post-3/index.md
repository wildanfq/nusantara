---
title: "Roadmap Hardware: Transformasi Arus Menjadi Logika"
description: "Panduan teknis membangun SBC RISC-V dari desain sirkuit hingga produksi PCB."
summary: "Pelajari bagaimana mengubah aliran listrik menjadi unit logika yang bisa berhitung hingga merancang arsitektur CPU berbasis RISC-V."
date: 2026-02-03T02:00:00+07:00
lastmod: 2026-02-03T02:00:00+07:00
draft: false
weight: 80
categories: ["Roadmap"]
tags: ["Hardware", "FPGA", "RISC-V", "PCB"]
contributors: ["Wildan FQ"]
pinned: false
homepage: true
seo:
  title: "Roadmap Hardware Engineer - Nusantara Labs"
  description: "Dari elektronika analog, digital, desain FPGA, hingga arsitektur komputer RISC-V dan layouting PCB."
  canonical: ""
  noindex: false
---

Roadmap ini adalah kelanjutan dari fondasi sains sebelumnya. Di sini, kita akan fokus pada penerapan teknis, mulai dari menyentuh kabel hingga merancang sirkuit komputer yang kompleks secara mandiri.

### 1. Elektronika Analog: Kendali Energi dan Sinyal Fisik

Segala sesuatu di komputer dimulai dari tegangan listrik. Tahap ini mengajarkanmu bagaimana cara menjinakkan energi tersebut agar bisa digunakan untuk membawa informasi tanpa merusak perangkat.

- **Analisis Kelistrikan Dasar:** Belajar cara menggunakan Multimeter untuk mengukur tegangan dan arus. Di sini kamu harus khatam Hukum Ohm ($V=IR$) agar bisa menghitung kebutuhan komponen secara presisi.
- **Karakteristik Komponen Pasif:** Memahami Resistor (pengerem arus), Kapasitor (penampung tegangan), dan Induktor (penyaring gangguan). Kamu belajar bagaimana ketiga benda ini menstabilkan aliran listrik.
- **Dioda dan Penyearah Arus:** Belajar cara mengubah arus AC (dari PLN) menjadi arus DC yang stabil untuk sirkuit elektronik.
- **Transistor sebagai Saklar:** Fokus pada BJT dan MOSFET. Kamu harus paham bagaimana sebuah kaki kecil (*Gate*) bisa memutus atau menyambung aliran listrik besar. Inilah momen di mana Fisika berubah menjadi Logika.



### 2. Elektronika Digital: Bahasa dan Logika Mesin

Setelah mahir mengendalikan listrik lewat transistor, saatnya menyusun miliaran transistor tersebut menjadi unit yang bisa berhitung. Di sini, listrik tidak lagi dilihat sebagai Volt, melainkan sebagai angka 0 dan 1.

- **Gerbang Logika Fisik:** Mempelajari IC (Integrated Circuit) seri 7400 untuk melihat bagaimana gerbang AND, OR, dan NOT bekerja di dunia nyata.
- **Sirkuit Kombinasional:** Belajar membangun unit penambah angka (*Adder*) dan pemilih jalur data (*Multiplexer*).
- **Sirkuit Sekuensial (Memori):** Belajar membangun *Flip-Flop* dan *Registers*. Ini adalah tahap di mana kamu memahami bagaimana listrik bisa "disimpan" menjadi data.
- **Hardware Description Language (HDL):** Mulai menggunakan **SystemVerilog**. Kamu tidak lagi menggambar jalur kabel secara manual, melainkan menulis kode yang mendefinisikan struktur sirkuit di dalam chip.

### 3. Prototyping Hardware: Menghidupkan Logika dengan FPGA

Sebelum membuat chip permanen, kamu butuh "laboratorium" virtual. FPGA (Field Programmable Gate Array) memungkinkan kamu membuat "chip kustom" yang bisa diprogram ulang berkali-kali tanpa risiko kerusakan fisik yang besar.

- **Pengenalan Ekosistem FPGA:** Memahami perbedaan mikrokontroler vs FPGA. Mempelajari struktur internal FPGA seperti *Look-Up Tables* (LUT), *Flip-Flops*, dan *Interconnects*.
- **Implementasi Logika pada Silikon:** Belajar menggunakan *Toolchain* (Vivado, Quartus, atau Yosys) untuk mengubah kode SystemVerilog menjadi aliran bit (*bitstream*) yang dikirim ke chip FPGA.
- **Simulasi dan Testbench:** Belajar cara menguji desain hardware di komputer sebelum dijalankan di alat nyata untuk memastikan tidak ada kesalahan logika (*bug*).
- **Debugging Hardware:** Belajar menggunakan *Logic Analyzer* (fisik maupun virtual) untuk melihat aliran data 0 dan 1 yang bergerak sangat cepat di dalam chip secara *real-time*.



### 4. Arsitektur Komputer: Desain Otak dan Sistem (RISC-V)

Ini adalah puncak rekayasa hardware. Kamu menggunakan FPGA sebagai media untuk membangun arsitektur CPU yang akan menjadi otak dari Single Board Computer (SBC) milikmu.

- **Set Instruksi (ISA):** Belajar "kamus" perintah yang dimengerti mesin, yaitu **RISC-V**. Kamu belajar bagaimana perintah "Tambah" atau "Simpan" diterjemahkan oleh hardware.
- **Implementasi RISC-V Core:** Menulis atau mengimplementasikan desain CPU RISC-V ke dalam FPGA. Di sini kamu akan melihat CPU buatanmu mulai menjalankan instruksi pertama (seperti menyalakan LED lewat kode mesin).
- **Datapath dan Control Unit:** Belajar mendesain jalur lalu lintas data di dalam CPU dan unit pengatur yang bertugas seperti polisi lalu lintas di dalam chip.
- **Pipelining dan Cache:** Mempelajari cara mempercepat kerja CPU agar bisa memproses banyak data sekaligus tanpa mengalami hambatan (*bottleneck*).


### 5. Rekayasa Sistem dan Produksi Fisik (PCB)

Setelah rancangan otak komputer (RISC-V) selesai diuji di FPGA, kamu harus meletakkannya di papan sirkuit yang nyata, aman, dan efisien agar bisa digunakan sebagai perangkat mandiri.

- **Manajemen Daya (Power Delivery):** Belajar menurunkan tegangan baterai menjadi tegangan mikro yang sangat stabil untuk inti prosesor melalui regulator voltase.
- **Layouting PCB (High-Speed Design):** Menggunakan software seperti **KiCad** atau **Altium**. Kamu belajar menggambar jalur tembaga dengan memperhatikan integritas sinyal agar data tidak korup saat mengalir cepat.
- **Integrasi Sistem:** Memahami standar koneksi seperti USB, PCIe, dan RAM slot agar hardware buatanmu bisa "berbicara" dengan perangkat lain.
