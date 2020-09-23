[![wild-west](./title.png)](https://github.com/moretrim/wild-west)

> Victoria 2 Gone Wild West. 

<footer>Concept by electric_I.</footer>

Build status:
[![travis-master][travis-master-image]](https://travis-ci.com/moretrim/wild-west/branches)

[travis-master-image]: https://travis-ci.com/moretrim/wild-west.svg?branch=master

Description
-----------

Start a game of [HPM] or [HFM] where every uncivilised country present or future undergoes
Westernisation on 1 January 1836. You also have the option to unlock Great Wars and World Wars at
the same time.

(See below for more information about mod compatibility.)

This mod does not change the number of cowboys or outlaws. Sorry.

[HPM]: https://github.com/arkhometha/Historical-Project-Mod
[HFM]: https://github.com/SighPie/HFM

Installation
------------

Since this is a submod, you need either of the following two base mods installed already:

- [Historical Project Mod][HPM/releases]
- [Historical Flavour Mod][HFM]

[HPM/releases]: https://github.com/arkhometha/Historical-Project-Mod/releases

Follow their respective instructions to install them if you haven’t already.

Grab the [0.1.0 release].

[0.1.0 release]: https://github.com/moretrim/wild-west/releases/tag/v0.1.0

Install this as you would any other mod. When installed properly, the `wild_west.mod` file and the
`wild-west` directory should live side-by-side with the respective `.mod` file and directory of the
underlying mod (be it HPM or HFM).

In the Victoria 2 launcher you should see an entry for the submod:

![launcher](./launcher.jpg)

Make sure you are loading **both** <cite>Wild West</cite> and the underlying mod (in the picture
that is HFM), as indicated by the check marks.

This submod has been designed so that load order should not matter.

Usage
-----

Once a game has been started you can verify that <cite>Wild West</cite> has been loaded correctly by
looking at the decision screen. It should include the following decision somewhere:

![decision](./decision.jpg)

Note that you can be playing any country of your choice, civilised or not, for this to be available.

This decision can only be activated during the first month of the game. It is further suggested that
if the decision is to be activated at all, it should be done on 1 January 1836 as the very first
thing before doing anything else. (You may miss on some features if you don’t.) Once activated,
you’ll immediately receive an event to Westernise *all* uncivilised countries whether they are
already on the map or not.

![event](./event.jpg)

The event gives you three options:

- Westernise all uncivilised countries and remove their lack of writing system modifiers (if any)
- same as above, but also unlock Great Wars and World Wars
- do nothing (in case you activated the decision by accident)

National Value
--------------

In HPM & HFM a Westernising country has the opportunity to shake off the shackles of tradition by
picking a new national value. <cite>Wild West</cite> extends the same choice to all newly
Westernised countries. The requirements are similar except that countries at war are allowed to pick
a new national value, unlike as in those mods. This is to account for the wars at the start of the
game.

There is another meaningful difference: in HPM/HFM the AI countries always pick ‘Order’ as the new
national value. Since this may be due to an oversight, <cite>Wild West</cite> instead reinterprets
the original design to assign the following random odds:

National Value  | Chance to pick
:---------------|-----------------:
Order           | 47%
Autocracy       | 33%
Productivity    | 10%
Equality†       | 5%
Liberty†        | 5%

†: in the original design these picks may not have been intended to be available to the AI

Compatibility
-------------

Besides HPM or HFM <cite>Wild West</cite> should be compatible with any mod (and submod) as long as
the following holds:

- event IDs `1596225xxx` are available
- the start date is in January 1836
- events `90900`, `90903`, and `90910` are in charge of Westernisation and look similar enough to
  those of HPM/HFM
- the national values of HPM/HFM are included in the mod’s national values
- `lacks_writing_system` is an event modifier

Some of those requirements preclude from using the submod with no other mod on.

<cite>Wild West</cite> is compatible with the [Ported HPM Dismantlement] submod.

[Ported HPM Dismantlement]: https://github.com/moretrim/ported-hpm-dismantlement

Image Licence
-------------

The <cite>Wild West</cite> title picture is based on a design by [Drid].

The image as well as its variants that can be found in the mod proper are licenced under a [Creative
Commons Attribution-ShareAlike 4.0 International License][CC BY-SA 4.0]. They are derivative works
of [<cite>Winchester Model 1873</cite>] by [Hmaag] available under the same terms.

[Drid]: https://www.twitch.tv/dridlicious
[<cite>Winchester Model 1873</cite>]: https://commons.wikimedia.org/wiki/File:Winchester_Model_1873.jpg
[Hmaag]: https://commons.wikimedia.org/wiki/User:Hmaag
[CC BY-SA 4.0]: https://creativecommons.org/licenses/by-sa/4.0

Release History
---------------

### 0.1.0

[The original release.][v0.1.0]

[v0.1.0]: https://github.com/moretrim/wild-west/tree/v0.1.0
