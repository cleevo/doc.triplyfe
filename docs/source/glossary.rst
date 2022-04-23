
========
Glossary
========


Aktivitas
    Definition for Aktivitas
Journey
    Sedikit berbeda dengan ketiga kata lainnya, journey yang tergolong sebagai kata benda atau noun ini memiliki makna 
    “sebuah perjalanan panjang yang jauh dan memakan waktu lama.” Biasanya, kata journey juga bisa digunakan untuk mengatakan “perjalanan hidup” dalam bahasa Inggris.
Travel
    Kata “travel” dalam bahasa Inggris biasanya bisa diartikan sebagai “bepergian”. Itu sebabnya, saat kamu jalan-jalan ke berbagai tempat 
    dalam jarak yang cukup jauh, kamu bisa disebut sedang travelling. Kata ini sebenarnya tidak berbeda jauh maknanya dengan kata “trip”. 
    Akan tetapi, jika “trip” adalah kata benda atau noun, kata “travel” termasuk sebagai kata kerja atau verb. Dalam bahasa Inggris, 
    kamu bisa menggunakan kata “travel” untuk menunjukkan aksi atau kegiatan yang dilakukan dan berkaitan dengan bepergian. Jika kegiatan tersebut 
    sedang berlangsung saat kamu mengatakannya, kamu bisa menggunakan kata “travelling” sebagai present participle dari kata “travel”.
Traveler
    Traveler adalah orang-orang yang melakukan perjalanan (travelling). Perjalanan ini bisa dilakukan dengan jarak pendek atau pun jarak jauh.
Tour
    Sama halnya dengan kata trip, kata tour juga termasuk sebagai kata benda atau noun. Kata yang satu ini memiliki makna “perjalanan yang dilakukan 
    ke beberapa tempat, bisa daerah, kota, hingga negara”. Hal ini bisa digunakan untuk mendeskripsikan sebuah perjalanan yang menyenangkan dan 
    dilakukan secara berkelanjutan ke beberapa tempat. Meski demikian, kata ini sebenarnya juga bisa difungsikan sebagai verb layaknya “travel”. 
    Biasanya, jika digunakan sebagai kata kerja, tour bermakna aktivitas bepergian yang dilakukan ke beberapa tempat secara berkelanjutan.
Tour Organizer
    sebuah biro dan agen perjalanan wisata yang menyediakan akomodasi dan fasilitas kegiatan berwisata yang sekaligus menyediakan kebutuhan perlengkapan 
    program acara dan kebutuhan lainnya yang menyertai kegiatan berwisata tersebut.
Trip
    Secara harfiah, kata “trip” artinya adalah sebuah perjalanan, biasanya bolak-balik ke suatu tempat. Meski bisa digunakan untuk perjalanan jauh, 
    kata “trip” akan lebih sesuai digunakan untuk perjalanan singkat yang sengaja dilakukan untuk kesenangan atau menyenangkan diri sendiri. 
    Dalam bahasa Inggris, kamu bisa menggunakan kata “trip” yang berupa kata benda atau noun untuk menceritakan perjalanan kerja (business trip), 
    liburan singkat (short trip), atau liburan sekolah (school trip).
Triplyfe
    Merupakan platform marketplace yang mempertemukan para pelaku industri pariwisata dengan para penggunanya (wisatawan/traveler).
Tripster
    Di triplyfe.id kami menyebut semua pengguna yang `bergabung dengan triplyfe<https://triplyfe.id/>`__ baik sebagai traveler maupun pelaku industri pariwisata yang 
    memberikan dan atau merasakan pengalaman-pengalaman unik bersama kami sebagai Tripster.

..
  -------------
  Specification
  -------------

  Functions:

  - ``type``: ``"function"``, ``"constructor"`` (can be omitted, defaulting to ``"function"``; ``"fallback"`` also possible but not relevant in web3.js);
  - ``name``: the name of the function (only present for function types);
  - ``constant``: ``true`` if function is specified to not modify the blockchain state;
  - ``payable``: ``true`` if function accepts ether, defaults to ``false``;
  - ``stateMutability``: a string with one of the following values: ``pure`` (specified to not read blockchain state), ``view`` (same as ``constant`` above), ``nonpayable`` and ``payable`` (same as ``payable`` above);
  - ``inputs``: an array of objects, each of which contains:

  - ``name``: the name of the parameter;
  - ``type``: the canonical type of the parameter.
  - ``outputs``: an array of objects same as ``inputs``, can be omitted if no outputs exist.

