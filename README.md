<<<<<<< HEAD
Starling Extension: Particle System
===================================

The Starling Particle System classes provide an easy way to display particle systems from within the [Starling Framework][1]. That way, adding special effects like explosions, smoke, snow, fire, etc. is very easy to do.

The extension consists of three classes:

1. `Particle`: stores the state of a particle, like its position and color
2. `ParticleSystem`: the base class for particle systems. Implements a very simple particle movement. To create a custom particle system, extend this class and override the methods `createParticle`, `initParticle`, and `advanceParticle`.
3. `PDParticleSystem`: a particle system subclass that can display particle systems created with the  [Particle Designer][2] from 71squared.

Installation
------------

Which version to download depends on the Starling version you are using:

* If you work with a release version of Starling, download the Particle System with the equivalent tag (Starling 1.1 -> Particle System 1.1).
* If you work with the latest development version of Starling, download the head revision of the Particle System. 

After downloading, you will find the three classes described above in the `src`-directory. You can either copy them directly to your Starling-powered application, or you add the source path to your FlexBuilder project.

Demo-Project
------------

The `demo`-directory contains a sample project. To compile it, add a reference to the Starling library and add the source directory that contains the particle system classes.

The project contains 4 sample configurations. Switch between configurations in `Demo.as` by 
hitting the space bar.
=======
Starling Extension: Animated Particle System
===================================

This Starling Extension allows you to create PD (Particle Designer) particle systems using animations from Sprite Sheets by passing a Starling TextureAtlas instance to the particle system constructor.

This extension depends on the Starling Framework: https://github.com/PrimaryFeather/Starling-Framework and the Starling-Extension-Particle-System: https://github.com/PrimaryFeather/Starling-Extension-Particle-System
>>>>>>> 44f4a052f3f566fd05b9d9dfb66877592104d807

Sample Code
-----------

<<<<<<< HEAD
The class `ParticleSystem` extends `DisplayObject` and behaves accordingly. You can add it as a child to the stage or any other container. As usual, you have to add it to a juggler (or call its `advanceTime` method once per frame) to animate it.

    // create particle system
    mParticleSystem = new PDParticleSystem(psConfig, psTexture);
    mParticleSystem.emitterX = 320;
    mParticleSystem.emitterY = 240;
    
    // add it to the stage and the juggler
    addChild(mParticleSystem);
    Starling.juggler.add(mParticleSystem);

    // start emitting particles
    mParticleSystem.start();

    // stop emitting particles
    mParticleSystem.stop();
=======
The example directory contains a quick demonstration for creating a particle system of 500 animated birds. All artwork in the example belongs to Gamua/PrimaryFeather. A compiled version of the example can be seen here: http://onebyonedesign.com/flash/starling/anipart/
>>>>>>> 44f4a052f3f566fd05b9d9dfb66877592104d807

More information
----------------

<<<<<<< HEAD
You can find more information in the [Starling Wiki](http://wiki.starling-framework.org/extensions/particlesystem).

[1]: http://www.starling-framework.org
[2]: http://particledesigner.71squared.com
=======
Particle configurations can be created with the 71 Squared Particle Designer or the online Particle Editor. Sprite sheets can be created with Texture Packer or within the Flash IDE (or other sprite sheet generators). For the moment, sprite sheets should be created with equally sized rectangles (no clipping) - this is a known issue and is being worked. For more info, see:

- http://www.starling-framework.org
- http://particledesigner.71squared.com
- http://onebyonedesign.com/flash/particleeditor/
- https://github.com/PrimaryFeather/Starling-Extension-Particle-System
- http://www.codeandweb.com/texturepacker
- http://www.adobe.com/devnet/flash/articles/using-sprite-sheet-generator.html
>>>>>>> 44f4a052f3f566fd05b9d9dfb66877592104d807
