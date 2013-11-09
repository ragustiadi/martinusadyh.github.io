---
comments: true
date: 2013-03-16 13:57:54+00:00
layout: post
slug: howto-change-default-editor-font-in-mysql-workbench
title: Howto Change Default Editor Font in MySQL Workbench
wordpress_id: 2439
categories:
- DataBase
tags:
- Font
- MySQL
- Workbench
---

Pernah merasa bahwa font yang digunakan oleh aplikasi [MySQL Workbench](http://dev.mysql.com/downloads/workbench/) kurang nikmat dipandang mata ? Pernah merasa ingin mengganti font yang digunakan oleh **MySQL Workbench** melalui menu **Edit > Preferences** tapi masih saja tidak berubah  ? Jika iya, berarti kita mempunyai masalah yang sama :D Setelah kemarin iseng-iseng bertanya ke paman [Google](http://google.com), akhirnya saya menemukan juga bagaimana mengganti font untuk SQL Editor di **MySQL Workbench** :) Jika kita menggunakan linux, maka carilah file dengan nama `/home/namauser/.mysql/workbench` (catatan: **namauser** diganti dengan nama user anda) dan jika di Windows maka carilah file `C:\Users\User\AppData\Roaming\MySQL\Workbench\wb_options.xml` Jika sudah, sekarang carilah entri seperti dibawah ini :

    
    
    <value type="string" key="workbench.general.Editor:Font">Bitstream Vera Sans Mono 11</value>
    



Gantilah entrian font dengan font yang anda inginkan, jika sudah tutup dan jalankan lagi **MySQL Workbench** maka kita akan mendapatkan hasil kurang lebih seperti gambar dibawah ini :)
[caption id="attachment_2443" align="alignnone" width="429"][![Tampilan Editor dengan Font Monaco](http://martinusadyh.web.id/wp-content/uploads/2013/03/Tampilan-Editor-dengan-Font-Monaco.png)](http://martinusadyh.web.id/gallery/?album=4&gallery=3&pid=392) Tampilan Editor dengan Font Monaco[/caption]

Nah dengan begini, jadi makin betah bukan berlama-lama menggunakan **MySQL Workbench** :)

**Referensi:**




  1. [Change Font MySQL Workbench](http://starikovs.com/2011/02/20/change-font-mysql-workbench-editor/)



