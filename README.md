# leaky-vs-token-bucket

## Notes

* Full credit goes to Michael Drogalis (of https://shadowtraffic.io/) for sparking the idea in me to try creating this app
* "Eff. Rate" is calculated over the lifetime of the simulation, so that's why it may look slow to update/catch up
* "Backpressure Cooldown (sec)" is meant to simulate networking delays, where the producer doesn't immediately get a signal from the downstream system that it is backed up; it's just a simple hack; I just wanted to get a middle ground between "unrealistic instant communication" and "waterfalls of balls overflowing due to animation delays/checks/etc."