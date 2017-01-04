---
title: "Recap: January 3, 2017 Meetup"
date: 2017-01-03 020:24 UTC
---

Thanks, all who rocked out at our first meetup of 2017! Member David Jones recorded tonight’s talk: look for it soon on our Youtube channel, [youtube.com/indyelixirorg](https://www.youtube.com/indyelixirorg).

Thanks as always to [our awesome sponsors](https://www.meetup.com/indyelixir/sponsors/) who made tonight possible. And congrats to Dave and Meining, winners of Manning’s *Elixir In Action* and *The Little Elixir and OTP Guidebook*, respectively.

## The Talk

**Steve Grossi** walked through some experiments with making music in Elixir: [github.com/stevegrossi/sweet_beats](https://github.com/stevegrossi/sweet_beats). We covered:

- Communicating with [the SoX audio library](http://sox.sourceforge.net/) from Elixir
- Using supervised processes to play audio simultaneously
- Relying on Elixir 1.4’s upcoming [`Registry`](http://elixir-lang.org/docs/master/elixir/Registry.html) module as a metronome to send messages to groups of processes
- Building a self-correcting timing mechanism when process messages arrive later than expected

Look for a recording of the talk to be posted here once it’s ready.

Then we ended the evening with an hour of musical hacking and discussion. Some highlights:

- Ben Falk pointed out that appending items to the end of a linked list is relatively slow on the BEAM, and suggested using a queue instead, for which he’d [written a library](https://hex.pm/packages/e_queue). Check out [the pull request](https://github.com/stevegrossi/sweet_beats/pull/1)!
- I learned the difference between performing `GenServer` setup in `start_link` vs. `init`. `start_link` happens in the originating process, while `init` happens in the `GenServer` process. So perform any memory-intensive setup in `start_link` to keep the `GenServer`’s own memory footprint small.
- Lucas Falk suggested using guard clauses to ensure we actually get lists when we’re expecting them. Always a good practice!

Please note that we’re switching to a bi-monthly schedule, so our next event will be on [March 7, 2017](https://www.meetup.com/indyelixir/events/235620866/)! We’re looking for speakers—please [let me know](mailto:hello@indyelixir.org) if you’re interested!
