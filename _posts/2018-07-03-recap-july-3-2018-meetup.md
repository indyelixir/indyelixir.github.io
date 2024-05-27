---
title: "Recap: July 3, 2018 Meetup"
---

Thanks to everyone who joined us on Tuesday! If you couldn’t make it, look for recordings soon on our Youtube channel, [youtube.com/indyelixirorg](https://www.youtube.com/indyelixirorg).

A big thank-you to [our sponsors](https://www.meetup.com/indyelixir/sponsors/) who made tonight possible. And congrats to Jimmy, Chris, and Bethany, winners of Manning Publications’ *Elixir In Action*, *The Little Elixir and OTP Guidebook*, and the upcoming *Phoenix In Action*.

We kicked things off with **Jared Alford** sharing how his team at Sigstr uses Elixir to publish events to [Apache Kafka](http://kafka.apache.org/). A challenge they faced with the [kafka_ex](https://github.com/kafkaex/kafka_ex) library is that when Kafka would go down, so would kafka_ex and it would take their application down with it. His solution was a GenServer to monitor Kafka and handle downtime gracefully.

- [The repository on Bitbucket](https://bitbucket.org/sigstr/sigstr-elixir-kafka/)

<figure>
  <div class="FlexVideo">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/95vxTigSvNQ" frameborder="0" allowfullscreen></iframe>
  </div>
</figure>

Eric Oestrich mentioned a similar challenge he faced building <https://gossip.haus/> with websocket connection failures bringing down the entire supervision tree. He's [blogged recently](https://blog.oestrich.org/2018/07/otp-tether/) about his "tether" solution to that problem.

**Jimmy Miller** gave the second talk, diving into property-based testing in Elixir with [`StreamData`](https://github.com/whatyouhide/stream_data) and `ExUnitProperties`. The Elixir core team is considering [adding these to Elixir](https://elixir-lang.org/blog/2017/10/31/stream-data-property-based-testing-and-data-generation-for-elixir/), so it was great to see how they work. Jimmy closed his talk with a rousing argument for why property-based testing matters: it aligns with the very purpose of programming which is to allow developers to think and communicate at a higher level about how the intentions and behavior of the systems we build. Onward!

<figure>
  <div class="FlexVideo">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/VhW9D0mbW1o" frameborder="0" allowfullscreen></iframe>
  </div>
</figure>

Sound exciting? Our next event will be on Tuesday, [September 4, 2018](https://www.meetup.com/indyelixir/events/252591281/) We’re always looking for speakers—please [reach out](mailto:hellostevegrossi+indyelixir@gmail.org) if you’re interested!
