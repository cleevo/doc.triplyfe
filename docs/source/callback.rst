
========
Callback
========

.. _xendit:
    https://xendit.co

Amara.id menggunakan jasa pihak ketiga, `<xendit_>`_, sebagai penyedia payment gateway. Untuk setiap transaksi pembayaran yang terjadi, xendit akan mengirimkan responnya berupa data dalam bentuk json ke http get.

.. code-block:: javascript

    {
        "event": "qr.payment",
        "id": "qrpy_8182837te-87st-49ing-8696-1239bd4d759c",
        "amount": 1500,
        "created": "2020-01-08T18:18:18.857Z",
        "qr_code": {
            "id": "qr_8182837te-87st-49ing-8696-1239bd4d759c",
            "external_id": "testing_id_123",
            "qr_string": "0002010102##########CO.XENDIT.WWW011893600#######14220002152#####414220010303TTT####015CO.XENDIT.WWW02180000000000000000000TTT52045######ID5911XenditQRIS6007Jakarta6105121606##########3k1mOnF73h11111111#3k1mOnF73h6v53033605401163040BDB",
            "type": "DYNAMIC"
        },
        "status": "COMPLETED"
    }

--------------
