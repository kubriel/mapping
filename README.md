# mapping

<img src=screenshot1.png>

I made this in 2011, and im still using it for our video mapping shows and installations.
It is 9 point free transform tool to adjust geometry of texture, and possibility to save and load adjusted coordinates.
It use [curve3d] object of Gem.

I often use it with [gemframebuffer], Cyrille Henry's soft_edge.frag, (which you can find in gem-doc/examples/12.multi_screen_projection), [pix_coordinate] to crop texture to multiple pieces, and [pd-mpv], making it very effective pushing quite high resolutions even on old hardware.

Its a mess, but it works well. I will try to clean it.
Olivier Baudu already tried to, but i was not able to navigate through it, and i used only his implementation for loading and saving mapped coordinates.
You will need Puredata, Gem, zexy, cyclone/coll, and cyclone/prepend

run it like this:

pd -lib Gem -lib zexy -lib cyclone/prepend -lib cyclone/coll

based on work of Miller Puckette, and IOhannes m zmölnig
