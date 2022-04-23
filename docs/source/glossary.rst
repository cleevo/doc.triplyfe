
========
Glossary
========


Aktivitas
    Definition for Aktivitas
Travel
    Kata “travel” dalam bahasa Inggris biasanya bisa diartikan sebagai “bepergian”. Itu sebabnya, saat kamu jalan-jalan ke berbagai tempat dalam jarak yang cukup jauh, kamu bisa disebut sedang travelling. Kata ini sebenarnya tidak berbeda jauh maknanya dengan kata “trip”. Akan tetapi, jika “trip” adalah kata benda atau noun, kata “travel” termasuk sebagai kata kerja atau verb. Dalam bahasa Inggris, kamu bisa menggunakan kata “travel” untuk menunjukkan aksi atau kegiatan yang dilakukan dan berkaitan dengan bepergian. Jika kegiatan tersebut sedang berlangsung saat kamu mengatakannya, kamu bisa menggunakan kata “travelling” sebagai present participle dari kata “travel”.
Traveler
    Traveler adalah orang-orang yang melakukan perjalanan (travelling). Perjalanan ini bisa dilakukan dengan jarak pendek atau pun jarak jauh.
Travel Organizer
    Definition for travel organizer
Trip
    Secara harfiah, kata “trip” artinya adalah sebuah perjalanan, biasanya bolak-balik ke suatu tempat. Meski bisa digunakan untuk perjalanan jauh, 
    kata “trip” akan lebih sesuai digunakan untuk perjalanan singkat yang sengaja dilakukan untuk kesenangan atau menyenangkan diri sendiri. 
    Dalam bahasa Inggris, kamu bisa menggunakan kata “trip” yang berupa kata benda atau noun untuk menceritakan perjalanan kerja (business trip), 
    liburan singkat (short trip), atau liburan sekolah (school trip).
Triplyfe
    Definition for term
Tripster
    Di triplyfe.id kami menyebut traveler yang `bergabung <https://triplyfe.id/signup/>`__ dan merasakan pengalaman-pengalaman unik bersama kami sebagai Tripster.

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

