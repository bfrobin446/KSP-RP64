# RP-64: A realistic vision of the Kerbol system

RP-64 is my attempt to curate a Kerbal Space Program experience that includes
realistic mechanics and limitations, but retains more of the stock aesthetic
and more compatibility with other mods than a total conversion like RP-1.

## What's included

### Sigma Dimensions at 6.4x scale

A larger solar system allows more realistically-proportioned rockets and more
realistic ascent profiles. Most launch vehicles won't have to coast and then
restart their engines just to make low Kerbin orbit.

### Engines by Real Fuels

### Life support by USI

You don't realize quite how far away Minmus is until you're trying to build a
ship that can keep a crew comfortable for two or three hundred hours. The Mun
becomes the logical choice for your first crewed landing.

### Lightweight satellites-first tech tree

It should always be possible to send an uncrewed mission to a place before you
can send a kerbal there.

I've looked at the two main probes-first tech tree conversions with recent
updates, Probes Before Crew and Unkerballed Start, and they both make changes
that I don't agree with. So I've chosen Bluedog Design Bureau as my reference
for how capabilities should progress through the tech tree, and I move a few
stock parts to live in the same tier as BDB parts with similar capabilities.

### ElectricCharge rebalance

RealAntennas and most life support mods follow the convention that one unit
of ElectricCharge represents one kilojoule of energy. Batteries and
generators will have their capacities increased to match.

## How to install

1. Manually download and install [Sigma Dimensions](https://github.com/Sigma88/Sigma-Dimensions/releases).
   The last release of Sigma Dimensions that's indexed on CKAN is several
   years out of date.

1. Set CKAN to allow mods compatible with KSP 1.10 and 1.11. The mods that we
   need 1.10 compatibility for are RealAntennas and SolverEngines.

1. I intend to make RP64 installable with CKAN once I have a version that's
   complete enough to declare as an official release. Until then:
   
   1. Use CKAN to install the other dependencies listed in RP64.netkan. Add
      recommended and suggested packages to taste.
            
   1. Copy or link the `GameData/RP64` folder from the repository into your KSP
      GameData.

1. If you have the Breaking Ground expansion installed, change
   `SERENITY_ROCS_VISUAL_SPEED` to 12 in KSP's `settings.cfg`.
   For game performance reasons, the researchable surface features in Breaking
   Ground are hidden if the active vessel's surface speed is above this
   threshold. But when Sigma Dimensions is installed, the speed that's compared
   to the threshold appears to be scaled down by the square of the solar system
   scale factor. At 6.4x, a threshold of 12 causes surface features to appear
   at roughly the same speed that we get with the default threshold of 500 at
   stock scale.

1. If you've been playing stock KSP on High terrain detail and you see poor
   frame rates near the Mun after installing the rescale, RP64 adds a
   "Medium-High" detail setting that may work better for you.

## Things to watch for future work

### Kerbalism

I like the way Kerbalism handles science, with experiments that have to stay
active for hours or days to produce a full return. But it has awkward
interactions with contracts that want the player to complete and return an
experiment, and if I let Kerbalism run life support I break compatibility
with other mods I want to support.

If a future version of Kerbalism has enough improvements to the process system
to replace the native modules for USI/Near Future nuclear reactors, I'll
consider converting other things that I'm supporting to use Kerbalism.
