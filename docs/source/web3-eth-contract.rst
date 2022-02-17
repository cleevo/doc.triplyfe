.. _eth-contract:

=================
web3.eth.Contract
=================

The ``web3.eth.Contract`` object makes it easy to interact with smart contracts on the ethereum blockchain.
When you create a new contract object you give it the json interface of the respective smart contract
and web3 will auto convert all calls into low level ABI calls over RPC for you.

This allows you to interact with smart contracts as if they were JavaScript objects.

To use it standalone:

.. code-block:: javascript

    var Contract = require('web3-eth-contract');

    // set provider for all later instances to use
    Contract.setProvider('ws://localhost:8546');

    var contract = new Contract(jsonInterface, address);

    contract.methods.somFunc().send({from: ....})
    .on('receipt', function(){
        ...
    });


------------------------------------------------------------------------------


new contract
============

.. index:: JSON interface

.. code-block:: javascript

    new web3.eth.Contract(jsonInterface[, address][, options])

----------
Parameters
----------

1. ``jsonInterface`` - ``Object``: The json interface for the contract to instantiate
2. ``address`` - ``String`` (optional): The address of the smart contract to call.
3. ``options`` - ``Object`` (optional): The options of the contract. Some are used as fallbacks for calls and transactions:
    * ``from`` - ``String``: The address transactions should be made from.
    * ``gasPrice`` - ``String``: The gas price in wei to use for transactions.
    * ``gas`` - ``Number``: The maximum gas provided for a transaction (gas limit).
    * ``data`` - ``String``: The byte code of the contract. Used when the contract gets deployed.

-------
Returns
-------

``Object``: The contract instance with all its methods and events.


-------
Example
-------

.. code-block:: javascript

    var myContract = new web3.eth.Contract([...], '0xde0B295669a9FD93d5F28D9Ec85E40f4cb697BAe', {
        from: '0x1234567890123456789012345678901234567891', // default from address
        gasPrice: '20000000000' // default gas price in wei, 20 gwei in this case
    });

---------------------