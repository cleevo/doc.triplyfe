
========
Glossary
========

---------
Aktivitas
---------

--------
Traveler
--------

Traveler adalah orang-orang yang melakukan perjalanan (travelling). Perjalanan ini bisa dilakukan dengan jarak pendek atau pun jarak jauh.

----
Trip
----

--------
Triplyfe
--------

--------
Tripster
--------

Di triplyfe.id kami menyebut traveler yang `bergabung <https://triplyfe.id/signup/>`__ dan merasakan pengalaman-pengalaman unik bersama kami sebagai Tripster.

``Tripster``: Di triplyfe.id kami menyebut traveler yang `bergabung <https://triplyfe.id/signup/>`__ dan merasakan pengalaman-pengalaman unik bersama kami sebagai Tripster;
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

