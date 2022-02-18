
========
Glossary
========



Tripster
=====================

Di triplyfe.id kami menyebut traveler yang `bergabung <https://triplyfe.id/signup/>`__ dan merasakan pengalaman-pengalaman unik bersama kami sebagai TRIPSTER.

Using this json interface web3.js is able to create JavaScript object representing the smart contract and its methods and events using the :ref:`web3.eth.Contract object <eth-contract>`.

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

