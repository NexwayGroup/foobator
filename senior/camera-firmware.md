# Camera firmware POC

Your task is to write a simple photo camera firmware POC.
It should support entire process from reading sensors values, setting exposure time,
aperture size, focal length, shutter release, and passing raw image to another subsystem
for storing on external memory card. It should support various modes
of operation: fully manual parameter settings, fixed exposure time,
fixed aperture size, fully automatic settings.

Use stubs or mocks where needed. The physics of photography doesn't actually matter.
The interaction between its componens is what really matters.

Guidelines:
- follow SOLID principles
- identify and use design patterns where appropriate
- use git to track changes and maintain traceable commit history
- comment relevant pieces of code only

Create a short documentation illustrating taking a photo with fully manual and fully automatic settings mode.
Bonus points for providing UML class diagram.
