
====
Web3
====

This is the main (or 'umbrella') class of the web3.js library.

.. code-block:: javascript

    var Web3 = require('web3');

    > Web3.utils
    > Web3.version
    > Web3.givenProvider
    > Web3.providers
    > Web3.modules

------------------------------------------------------------------------------

Web3.modules
=====================

.. code-block:: javascript

    Web3.modules

Will return an object with the classes of all major sub modules, to be able to instantiate them manually.

-------
Returns
-------

``Object``: A list of module constructors:
    - ``Eth`` - ``Constructor``: The Eth module for interacting with the Ethereum network.
    - ``Net`` - ``Constructor``: The Net module for interacting with network properties.
    - ``Personal`` - ``Constructor``: The Personal module for interacting with the Ethereum accounts.
    - ``Shh`` - ``Constructor``: The Shh module for interacting with the whisper protocol.
    - ``Bzz`` - ``Constructor``: The Bzz module for interacting with the swarm network.

-------
Example
-------

.. code-block:: javascript

    Web3.modules
    > {
        Eth: Eth(provider),
        Net: Net(provider),
        Personal: Personal(provider),
        Shh: Shh(provider),
        Bzz: Bzz(provider),
    }


------------------------------------------------------------------------------