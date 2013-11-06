---
author: admin
comments: true
date: 2013-07-27 13:50:51+00:00
layout: post
slug: cara-mudah-mendebug-widget-di-dojo
title: Cara Mudah Mendebug Widget di Dojo
wordpress_id: 3098
categories:
- JavaScript
tags:
- Debugging Dojo Application
- Dojo
- Dojo Toolkit
- EnhancedGrid
- Grid
- JavaScript
- Widget
---

Pernah menggunakan [Dojo Toolkit](http://dojotoolkit.org/) sebagai UI _layer_? Pernah merasa kalau dokumentasi di Dojo itu sangat sedikit sekali ? Bingung tentang _function_ apa saja yang terdapat di komponen tersebut ? Jika iya berarti sama dengan saya ketika dulu baru pertama kali baru mulai menggunakan Dojo sebagai pilihan untuk sisi UI. Sebenar-nya Dojo merupakan pilihan yang cukup **"mumpuni"** dibandingkan dengan [ExtJS](http://www.sencha.com/products/extjs) dari sisi kelengkapan widget-widget yang disediakan, tetapi sayang-nya kelengkapan widget ini tidak didukung dengan dokumentasi yang sepadan jika dibandingkan dengan [ExtJS](http://www.sencha.com/products/extjs) yang dokumentasi-nya cukup lengkap dari tutorial sampai ke sisi API _(Application Programming Interface)_-nya.

Meskipun [Dojo Toolkit](http://dojotoolkit.org/) juga mempunyai sebuah halaman [API Documentation](http://dojotoolkit.org/api/), tapi rasanya masih kurang lengkap menurut saya. Nah untuk mendebug sebuah widget Dojo untuk menampilkan seluruh function yang terdapat didalam-nya, maka kita memerlukan sebuah browser dan [Firebug](http://getfirebug.com/) sebagai alat bantu kita (jika menggunakan Chrome, tidak perlu firebug lagi karena kita bisa membuka **Developer Tools** dengan menekan kombinasi tombol **CTRL+SHIFT+J**)

Sebagai contoh misalkan kita mempunyai sebuah widget grid dengan id `tblSettingSegment` seperti gambar dibawah ini :
[caption id="attachment_3102" align="alignnone" width="300"][![Contoh Grid](http://martinusadyh.web.id/wp-content/uploads/2013/07/Contoh-Grid-300x54.png)](http://martinusadyh.web.id/gallery/?album=4&gallery=3&pid=669) Contoh Grid[/caption]
<!-- more -->
jika grid tersebut sudah tampil di browser, maka bukalah firebug atau tekan kombinasi tombol **CTRL+SHIFT+J** kemudian di console ketikkan perintah `dijit.byId('tblSettingSegment')` kemudian tekan **ENTER** hingga Firebug tampilan-nya menjadi seperti dibawah ini :
[caption id="attachment_3103" align="alignnone" width="300"][![Debug Grid Widget](http://martinusadyh.web.id/wp-content/uploads/2013/07/Debug-Grid-Widget-300x41.png)](http://martinusadyh.web.id/gallery/?album=4&gallery=3&pid=671) Debug Grid Widget[/caption]

Setelah hasilnya seperti diatas, maka kita bisa melihat seluruh fungsi yang terdapat di dojo grid tersebut dengan mengklik hasil output tersebut hingga tampilan-nya seperti gambar dibawah ini :
[caption id="attachment_3104" align="alignnone" width="300"][![Daftar Function](http://martinusadyh.web.id/wp-content/uploads/2013/07/Daftar-Function-300x146.png)](http://martinusadyh.web.id/gallery/?album=4&gallery=3&pid=670) Daftar Function[/caption]

Nah disini kita bisa melihat seluruh function yang digunakan oleh Dojo grid baik yang terdapat di halaman API Documentation maupun tidak :) Mudah bukan ?
