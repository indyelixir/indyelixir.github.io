---
title: "Recap: March 6, 2018 Meetup"
---

Thanks to all the folks who joined us on Tuesday! If you couldn’t make it, look for recordings soon on our Youtube channel, [youtube.com/indyelixirorg](https://www.youtube.com/indyelixirorg).

Thanks as always to [our sponsors](https://www.meetup.com/indyelixir/sponsors/) who made tonight possible. And congrats to Andrew, Doug, and Joe, winners of Manning Publications’ *Elixir In Action*, *The Little Elixir and OTP Guidebook*, and the upcoming *Phoenix In Action*.

We kicked things off with an open-mic night that ended up spanning the whole meeting!

<figure>
  <div class="FlexVideo">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/wY0kwp9X65o" frameborder="0" allowfullscreen></iframe>
  </div>
</figure>

**Eric Oestrich** shared a clever approach to keeping commonly-used strings (like form labels) in a separate text file that’s compiled into functions by hooking into Phoenix’s code-reloading with `@external_resource`. Check out [the blog post for more detail](https://blog.oestrich.org/2018/03/elixir-external-resources/).

**Steve Grossi** talked about a positive experience deploying Eric’s [ex_venture](https://github.com/oestrich/ex_venture) on [Gigalixir](https://gigalixir.com/), a relatively new Elixir hosting platform-as-a-service more tailored to Elixir and OTP apps than something like Heroku.

**Ben Falk** gave a fascinating deep-dive into reverse-engineering the binary protocol used by the Dark Age of Camelot MMORPG in an effort to build his own server for the game. Elixir makes parsing binary data easy, but doing so at this scale required some interesting patterns.

Our next event will be on Tuesday, [May 1, 2018](https://www.meetup.com/indyelixir/events/248627642/) We’re always looking for speakers—please [let me know](mailto:hello@indyelixir.org) if you’re interested!
