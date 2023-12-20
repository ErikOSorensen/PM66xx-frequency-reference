# PM66xx-frequency-reference

The plan is to build a good 10MHz reference for a PM6674 frequency counter (and those that are related).
This will be a gift to a lucky owner of such a counter.

Inspiration (and physical measurements) are taken from [The sync channel](https://syncchannel.blogspot.com/2016/04/flukephilips-pm66xx-frequency-counter.html),
but I am not so sure about using the internal voltage reference of the oscillator module. I would rather use an external low tempco 
reference such as the [ADR434BRZ](https://www.analog.com/en/products/adr434.html), which means I also need to add
a voltage regulator for this chip.

Looking at the output of my spare CTS 970 oscillator, I think it would also be nice to provide 
a filter on the output, and I've added a 10.5 MHz low pass filter on the bottom of the board.