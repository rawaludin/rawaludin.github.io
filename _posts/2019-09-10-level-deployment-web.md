---
layout: post
title: Level-Level Deployment Web
---

Level 1: Pakai shared hosting. Upload code via ftp, import sql via phpmyadmin. Test manual.

Level 2: Pakai VPS. Connect repository ke travis, deploy pas commit di develop/master branch. Test otomatis.

Level 3: Pakai cloud. Sama kayak level 2, cuman pakai instance dari AWS, Google Cloud, etc. Biar auto scale, load balance, etc.

Level 4: Containerized app. Misal pakai docker. Build image dari travis, deploy image ke cloud pas success.

Level 5: Container Orchestration. Sama kayak level 4, cuman deploy nya di orchestra misalnya pakai kubernetes. Maklum, servernya banyak. Microservices bro.
