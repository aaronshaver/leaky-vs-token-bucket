# leaky-vs-token-bucket

Interactive simulation of Leaky Bucket vs Token Bucket rate limiting algorithms

## Where to play with the simulation?

https://aaronshaver.github.io/leaky-vs-token-bucket/

## Notes

* Credit goes to Michael Drogalis (of https://shadowtraffic.io/) for sparking the idea in me to try creating this app
* Click the BURST button to do a one-time burst of taking tokens (this shows how the token bucket algorithm can better increase the effective consumption rate compared to the leaky bucket's fixed-drip)
* "Eff. Rate" (effective consumption rate) is calculated over the lifetime of the simulation -- it can take time to catch up to a new rate
* "Backpressure Cooldown" simulates network delay. The producer doesn't immediately get the signal from the downstream system (to back off for X seconds)
