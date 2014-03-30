PolyThrottle
================

This can throttle API usages globally, or for a particular request identitifer (whether that be session id, ipaddress)
Could even use client fingerprinting.

Can differentiate on different things to throttle for.

Use leaky bucket strategy, but look into other strategies as well.

Should be a daemonised service, exposing a REST/RPC interface.

Temporary data should be stored in memory. This is throttling, not for setting API limits.

If it needs to use a external memory storage, it should link up to a remote cache service. Let's not use libraries. But external services.
