
========
Docker
========

Network
=======

Mengkonfigurasi network agar setiap container dapat berkomunikasi:

.. code-block:: powershell

    D:\Teguh\docker> docker network ls

Membuat network dengan nama ``palapa-net``:

.. code-block:: powershell

    D:\Teguh\docker> docker network create palapa-net

Melakukan inspeksi container-container apa saja yang menjadi anggota network ``palapa-net``:

.. code-block:: powershell

    D:\Teguh\docker> docker network inspect palapa-net

Untuk menghubungkan container yang sedang berjalan ke user-defined bridge yang sudah ada, gunakan perintah ``docker network connect``. Perintah berikut menghubungkan container ``eclipse-mosquitto`` dan ``mongodb`` ke jaringan ``palapa-net``

.. code-block:: powershell

    D:\Teguh\docker> docker network connect palapa-net eclipse-mosquitto

    D:\Teguh\docker> docker network connect palapa-net mongodb
