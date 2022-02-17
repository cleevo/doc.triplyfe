.. _eth-subscribe:

==================
web3.eth.subscribe
==================

The ``web3.eth.subscribe`` function lets you subscribe to specific events in the blockchain.


subscribe
=========

.. code-block:: javascript

    web3.eth.subscribe(type [, options] [, callback]);

----------
Parameters
----------

1. ``String`` - The subscription you want to subscribe to.
2. ``Mixed`` - (optional) Optional additional parameters, depending on the subscription type.
3. ``Function`` - (optional) Optional callback, returns an error object as first parameter and the result as second. Will be called for each incoming subscription, and the subscription itself as the 3rd parameter.

.. _eth-subscription-return:

-------
Returns
-------

``EventEmitter`` - A Subscription instance

    - ``subscription.id``: The subscription id, used to identify and unsubscribing the subscription.
    - ``subscription.subscribe([callback])``: Can be used to re-subscribe with the same parameters.
    - ``subscription.unsubscribe([callback])``: Unsubscribes the subscription and returns `TRUE` in the callback if successful.
    - ``subscription.arguments``: The subscription arguments, used when re-subscribing.
    - ``on("data")`` returns ``Object``: Fires on each incoming log with the log object as argument.
    - ``on("changed")`` returns ``Object``: Fires on each log which was removed from the blockchain. The log will have the additional property ``"removed: true"``.
    - ``on("error")`` returns ``Object``: Fires when an error in the subscription occurs.
    - ``on("connected")`` returns ``String``: Fires once after the subscription successfully connected. Returns the subscription id.

--------------------
Notification returns
--------------------

- ``Mixed`` - depends on the subscription, see the different subscriptions for more.

-------
Example
-------

.. code-block:: javascript

    var subscription = web3.eth.subscribe('logs', {
        address: '0x123456..',
        topics: ['0x12345...']
    }, function(error, result){
        if (!error)
            console.log(result);
    });

    // unsubscribes the subscription
    subscription.unsubscribe(function(error, success){
        if(success)
            console.log('Successfully unsubscribed!');
    });

    ---------