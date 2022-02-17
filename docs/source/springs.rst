
========
Springs
========

Springs merupakan vending machine yang didesain sebagai dispenser untuk wadah berbagai produk cair.

uC API Reference
================

setrefill()
-----------

.. code-block:: console

    >setrefill([option])


Parameters
^^^^^^^^^^

1. ``Int`` - Jumlah volume produk cair.

example
-------

.. code-block:: javascript

    ipcMain.on('init-refill-event',(event,data) => { 
        const parser = port.pipe(new Readline({ delimiter: '\r\n' }))
        function setrefill(data) {
            return new Promise((resolve, reject) => {
                setTimeout(() => {
                    resolve(port.write('setrefill('100')\r\n'))
                });
            });
        }
    ...
    })

resetrefill()
-------------

.. code-block:: console

    >resetrefill()

readstatus()
------------

.. code-block:: console

    >readstatus()


Returns
^^^^^^^

``Int``: Volume akhir produk yang diambil pelanggan.

Arduino Firmware:

For ``Arduino Firmware`` see the :ref:`Arduino source code <uc-springs>`.

