---
layout: post
title: Level-Level Manajemen Environment Server Web
---

Level 1: Cuma satu, production. Biasanya single developer. Environment production berfungsi sekaligus buat QA. Testing manual atau via travis. Kalau ada yang error, benerin, langsung push ke server. Beres.

Level 2: Dua environment, development sama production. Yang ini mau environment production bener2 udah jalan. QA di environment development. Biasanya auto deploy, misal ada commit baru di branch develop, deploy server deveploment. Commit baru di master, deploy server production.

Level 3: Tiga environment; development, QA sama production. Yang ini tim nya banyak. Frontend dan backend beda repository. Makanya butuh dev dan qa terpisah. Buat integrasi antar tim di environment dev dulu. Kalau dah bener, baru dia deploy ke QA. Kalau di QA dah ok, baru deploy ke production. Sama, auto deploy. Khusus buat qa dan production, pakai tagged release buat detect nya. Branch develop ada tag baru, deploy qa. Branch master ada tag baru, deploy production.

Level 4: Empat environment; development, QA, staging sama production. Mirip level 3, yang ini butuh production bener2 error free. Staging dibuat mirip banget sama production. Misal database production di copy ke staging. Setelah lulus di QA, di staging di cek lagi. Mungkin bisa load test gitu, kan mirip sama production. Ke production dan staging manual release sama Release Manager.

Tergantung kompleksitas, jumlah environment ini tidak selalu sama dengan jumlah server. Bisa kurang atau lebih.
