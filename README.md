# InlineBallutes

Slow down your rocket in an upper atmosphere. Ballute = parachute + baloon = an alternative to a heatshield.

# FAQ

#  Is it even real? 


Yes, you can read about this technology here [pdf] and here [pdf].

#    How to use it? 


Get into upper thin atmosphere (i.e. Duna, Kerbin or Laythe). Deploy it. Initially deceleration is mariginal (depending on your vessel speed and mass) but it picks up quickly when you lower your altitude. You can repack it like a normal parachute if you plan multiple orbital decelerations

#    Can I use it instead of parachute? 


Rather not. Ballute drag is 3-4 times lower than parachute. And then it's much heavier due to used material and shape(Zylon instead of Nylon). However since it's inline version you can use it complementary to parachute. Ballute is also great for semi-powered landing when you just need to use engines just above over the surface for the final slowdown.

#    It is better than heatshield? 


Depending on scenario it can be better than heatshield. Shields usually have small diameter thus requiring ship to be slim and tall. With ballute you slow down in higher atmosphere when there's not much heat, thus you can have more broad vessel design. Also ballute slows you down quite effectively in thin atmosphere (i.e. above surface of Duna) whereas heatshield doesn't have enough area to do this.
However sometimes it's easier to use heatshield.

#    How it works with stock aero? Can I use it with FAR? 


#Stock aerodynamics:
Aerocapture and aerobraking works as it should in my opinion. So all in all ballute can be used for both things.
Duna scenario - it slows down a craft to about 80-90 m/s near the ground so it works better than heatshield and complementary to standard parachutes. It is able to slow down craft from speeds 2+ km/s using less dense atmo.
Kerbin scenario - it is possible to reentry 1st stage or other stuff using inline ballute. Should work nicely when constructing reusable stages (SpaceY as well). Still requires powered landing however not much fuel is required.
Jool aerobraking - doesn't work or work very poorly at best (very narrow altitude band when heating doesn't kill ballute). I don't think it is possible for it to work since if I tweak values to be sustainable for Jool stuff the parachute would become too op for other scenarios.

You can modify sensitivity of parachutes by modifying skinMaxTemp.

#FAR aerodynamics:

FAR simulates perfectly upper parts of an atmospheres unlike stock aerodynamics where heat kicks in even in the uppermost part of it. Thus FAR can simulate real aerobraking scenarios when ships incoming with high interplanetary speeds can decelerate effectively in upper parts of atmosphere (where there's almost no heating involved).

Unfortunately FAR replaces stock ModuleParachute with RealChuteFAR module which has several values set as static (so they cannot be changed), for example parachute max temperature 220C, drag, etc.If you want to configure those values install RealChute mod and replace ModuleParachute with RealChute one (most variables there are held in a material definition).

How it works now:
- it's great for aerobraking - getting into eliptical orbits decelerating from high interplanetary speeds in upper atmosphere where there's practically no heat involved,
- it's no good for aerocapture - 220 max temp and other constants set by RealChuteFAR makes it so that parachute breaks instantly when crossing certain atmosphere threshold (except Duna).

Kerbin aerobraking scenario: great aerobraking potential till about 38km threshold when temperature suddenly rips ballute apart. Still can bleed about 800 m/s before a ballute is destroyed.
Duna scenario: great aerobraking potential. Plus due to a thin atmosphere it's possible to aerocapture and slow down to about 100 m/s near the surface.
Jool aerobraking: great potential however orbit needs to be set precisely since only an uppermost atmosphere layer doesn't heat up stuff. 
