---
title: "Nusantara School"
type: "docs"
weight: 1
bookToC: false
---

**Nusantara School** adalah platform edukasi terbuka yang didedikasikan bagi siapa saja yang ingin memahami dunia komputer secara mendalam, menyeluruh, dan fundamental.

### Alur Pembelajaran yang Terstruktur

Dokumentasi ini disusun secara akurat untuk memandu Anda melalui perjalanan teknis yang runtut, mulai dari gerbang logika hingga terciptanya sebuah kepingan silikon. Berikut adalah tahapan yang akan Anda lalui:

**Fase Fondasi dan Desain Arsitektur CPU**

Perjalanan dimulai dengan memahami bagaimana sebuah instruksi diproses oleh gerbang logika dasar. Pada tahap awal ini, fokus utama adalah merancang unit fungsional seperti ALU, Register, dan Control Unit berbasis arsitektur RISC-V (RV32I) menggunakan simulasi visual Logisim Evolution. Setelah logika dasarnya matang, Anda akan belajar menerjemahkan desain visual tersebut ke dalam standar industri menggunakan *Hardware Description Language* (HDL), yaitu Verilog atau SystemVerilog. Penggunaan alat verifikasi seperti Verilator dan Icarus Verilog menjadi sangat krusial di sini untuk memastikan desain CPU bebas dari kesalahan logika sebelum melangkah ke perangkat keras.

**Implementasi pada Perangkat Keras Nyata (FPGA)**

Setelah desain digital tervalidasi, langkah selanjutnya adalah menanamkan kode HDL tersebut ke dalam chip FPGA untuk menguji kinerjanya secara fisik. Kami berkomitmen penuh menggunakan *toolchain* yang sepenuhnya *open-source*, seperti Yosys untuk sintesis logika dan nextpnr untuk proses *Place and Route*. Dengan menggunakan papan pengembangan seperti Lattice iCE40 atau ECP5, Anda dapat menyaksikan bagaimana desain logika yang tadinya hanya berupa kode di layar komputer kini benar-benar berdenyut dan menjalankan perintah di dalam perangkat keras nyata.

**Desain Fisik Silikon dan EDA (Electronic Design Automation)**

Sebagai puncak dari seluruh proses pembelajaran, Anda akan mendalami dunia desain fisik silikon untuk menghasilkan *microchip* yang siap diproduksi di pabrik. Menggunakan alur kerja OpenLane atau LibreLane yang terintegrasi dengan PDK (*Process Design Kit*) industri seperti SkyWater 130nm, Anda akan mempelajari proses transformasi RTL-to-GDSII. Melalui tahap *Static Timing Analysis* (STA) hingga *Design Rule Check* (DRC), seluruh proses ini bermuara pada pembuatan berkas GDSII—sebuah cetak biru tata letak cip final yang siap dikirim ke *foundry* untuk dicetak menjadi kepingan silikon nyata.

**kontributor**

Kami selalu membuka pintu seluas-luasnya bagi para kontributor untuk ikut membangun dan menyempurnakan dokumentasi pembelajaran ini. Jika Anda menemukan kesalahan, kekurangan, atau memiliki saran perbaikan, silakan laporkan melalui fitur *Issue* di repositori GitHub kami agar platform ini dapat terus berkembang menjadi lebih baik.
