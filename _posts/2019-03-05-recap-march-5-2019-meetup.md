---
title: "Recap: March 5, 2019 Meetup"
---

Thank you to [our sponsors](https://www.meetup.com/indyelixir/sponsors/) for making tonight’s meetup possible. And congrats to Jared, Eric, and Dave, winners of Manning Publications’ *Elixir In Action*, *The Little Elixir and OTP Guidebook*, and *Phoenix In Action*. Remember you can always use our group’s discount code—`ug367`—on [manning.com](https://www.manning.com/) for 36% off their books on Elixir and other topics.

Tonight’s event was an Elixir Open Mic Night. Eric started things off, having just returned from Lonestar Elixir Conf (see [his talk here](https://www.youtube.com/watch?v=ETUD9SaRCjY&list=PLGqeEOaC5KsRisF-GUlgJh35EowwzMYoS&index=2)). Eric recently introduced some big changes to his [Grapevine](https://grapevine.haus/) game network, most notably a web client where you can play games from across the network without leaving your browser! Eric and his company SmartLogic have also been producing content, including [a fantastic Elixir podcast](https://podcast.smartlogic.io) (featuring some familiar Indy Elixir faces) and an Elixir coding [live stream](https://www.twitch.tv/smartlogictv) ([recordings here](https://www.youtube.com/channel/UCWAV0_JasFSJMLGryeUedCQ)).

Jared shared a new library he found, [wormhole](https://github.com/renderedtext/wormhole), that runs a function, traps any errors, and returns a status—handy when you don't want to risk a process dying and losing its state while processing unknown data.

Finally, we wrapped up with an Exercism.io exercise appropriately titled “Meetup” about calculating meetup dates given a schedule like "second Monday" or "Wednesteenth" (the only Wednesday ending in "-teenth"). See [our solution here](https://exercism.io/my/solutions/f69577fa89cd4c2096870fc467cf03a8). It was fun to workshop, even if it [could have been simpler](https://exercism.io/tracks/elixir/exercises/meetup/solutions/e25bec45c5454381971022676f11d0ee) if we'd used the recently-added `Calendar` module. This bit was my favorite:

```elixir
defp ok!({:ok, value}), do: value
```

We wanted to call it 🆗, but were surprised (given Elixir's excellent Unicode support) that emoji in function names won't compile. 🤷‍♂️

Our next event will be on Tuesday, [May 7, 2019](https://www.meetup.com/indyelixir/events/259558481/) We’re always looking for speakers—please [reach out](mailto:hello@indyelixir.org) if you’re interested!
