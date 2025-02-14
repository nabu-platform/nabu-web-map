# TODO

## Clarify render failures

It is unclear what happens if the registered endpoint is not available/too slow/...
Do we get an error? There is no catch.
Does it just silently fail and retry every hour?

We should try to render it a couple of times and stop + event when we can't

## Disk cleanup

Chrome uses quite a bit of diskspace to render offline. We need to clean it up.
The files reside by default in: /tmp/snap-private-tmp/snap.chromium/tmp

# General

One sitemap list can only contain up to 50.000 entries and can not exceed 50mb unzipped.
We want to support both generated entries and manual entries