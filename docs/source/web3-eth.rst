.. _eth:

========
web3.eth
========

The ``web3-eth`` package allows you to interact with an Ethereum blockchain and Ethereum smart contracts.


.. code-block:: javascript

    var Eth = require('web3-eth');

    // "Eth.providers.givenProvider" will be set if in an Ethereum supported browser.
    var eth = new Eth(Eth.givenProvider || 'ws://some.local-or-remote.node:8546');


    // or using the web3 umbrella package

    var Web3 = require('web3');
    var web3 = new Web3(Web3.givenProvider || 'ws://some.local-or-remote.node:8546');

    // -> web3.eth


Note on checksum addresses
==========================

All Ethereum addresses returned by functions of this package are returned as checksum addresses.
This means some letters are uppercase and some are lowercase.
Based on that it will calculate a checksum for the address and prove its correctness.
Incorrect checksum addresses will throw an error when passed into functions.
If you want to circumvent the checksum check you can make an address all lower- or uppercase.


-------
Example
-------

.. code-block:: javascript

    web3.eth.getAccounts(console.log);
    > ["0x11f4d0A3c12e86B4b5F39B213F7E19D048276DAe" ,"0x85F43D8a49eeB85d32Cf465507DD71d507100C1d"]


------------------------------------------------------------------------------

subscribe
=====================

For ``web3.eth.subscribe`` see the :ref:`Subscribe reference documentation <eth-subscribe>`.


------------------------------------------------------------------------------


Contract
=====================

For ``web3.eth.Contract`` see the :ref:`Contract reference documentation <eth-contract>`.

------------------------------------------------------------------------------