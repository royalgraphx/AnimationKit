# AnimationKit
Open Source Version of AnimationKit &amp; it's accompanying assets.

![AnimationKit Logo](https://github.com/royalgraphx/AnimationKit/blob/master/Logo.png?raw=true)

# Welcome to AnimationKit!
This is an Adobe After Effects project file that depends on Element3D for creating Animations for W1/H1 Devices! This is not the original way Apple uses to create the loops for iOS Splash screens, but this is an Open Sourced recreation, Element3D Supports .OBJ models and can easily be configured with this Project! Cameras and Looping have already been precomped and is ready to use instantly!

#### What is this currently for? What else could this become?
This all started from a proof-of-concept I created for a reddit request for a Juul animation that would replace the AirPods H1 Splash screen, quickly I hopped up to create a rough draft and began rendering multiple .MOV's with different codec's, resolutions, color depths, and other settings that would not match with the original, then I manually replaced the video file using Filza and it worked! This was although, a permanent "tweak", which worked even out of jailbreak mode, there was no actual preferences or panel to activate it easily, so it stayed as an .MOV that was manually installed, But then an amazing developer by the Twitter handle @BooDev , created a tweak to change AirPod's animations on the fly! So I began work on multiple colors for AirPod's and making as much starter content as I could, So for now, this is just for AirPods, and you can't use this to create cool iPhone animations that show up on other splash screens such as settings, this project file's resolution and settings are meant for AirPods animations, but in the future i hope to rig more cameras to create and automate other Anim's shown throughout iOS.

#### Future Plans!
I'd like to work towards supporting the change of other images in the splash screen for AirPods, as this currently can change the "Open Case" video, but reverts back to the regular AirPods when you take one out, or if its low battery, or other small issues that would change it to show the .PNG'S instead, which swapping those out isn't supported currently, but I've made a bunch of those replacements so implementation should be super easy i'd hope.

# How To | AnimationKit

This Requires Adobe After Effects CC2019+ & Element3D(https://www.videocopilot.net/products/element2/) by VideoCopilot

# Prepare your 3D Assets, Be sure to use .OBJ's
I'd recommend to get your assets from the following sources: </br>
https://www.models-resource.com/ </br>
https://www.spriters-resource.com/ </br>
https://www.textures-resource.com/ </br>
![Models Resource](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/1modelsresource.png?raw=true)
</br>
![Prepped Files](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/2preparemodels.png?raw=true)
</br>
If you find other files that are 3D formats but need to be converted to .OBJ I highly recommend this application: </br>
![CAD](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/3cad.png?raw=true)
https://cadexchanger.com/ </br>

# Launch After Effects & Learn Project Layout
![AnimKitV2](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/4openkit.png?raw=true)
## This is the Project Pane, It features all Comps in the Project file.
![Pane](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/5projpane.png?raw=true)
## This is the Main View, it changes depending on what Comp you are in. It is Also the Logo's design.
![Main View](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/6mainview.png?raw=true)
## This is the Preview Control Pane, Make sure you're set to 60 FPS.
![Preview Pane](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/7previewpane.png?raw=true)
## This is the Timeline, you can activate layers by clicking the Eye icon.
![Timeline Pane](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/8timelinepane.png?raw=true)
## Overview.
![Overview](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/9overview.png?raw=true)

# Viewing the Size Reference
This layer is the original ProxCard_loop, it can be turned on to view and compare your model's sizing to match to the original sizing.
![SizeRef](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/10sizeref.png?raw=true)
![SizeRef](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/11guidelines.png?raw=true)

# Importing the Left Animation
## Double Click the 'Left Animation' Pre-Comp to go inside and import your 3D Model
![TL](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/12leftanim.png?raw=true)
## In this Pre-Comp, We have two layers, A Camera that is Pre-Keyframed and an Element3D layer
![TL](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/13timeline.png?raw=true)
## The Main View will now feature a Top-Down View and a POV View
![New View](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/15visual.gif?raw=true)
## Select the 'Left Object' Layer and begin to import your model using Element3D, Don't forget to 'Normalize Size'!
![Visual](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/17leftanim.gif?raw=true)
## Return to the 'Render This' Pre-Comp, and resize the left animation to fit the guidelines of the AirPods
![Visual](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/18fixsize.gif?raw=true)
# Repeat for the Right Animation.
![Visual](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/19rightanim.gif?raw=true)
![Visual](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/20fixsize.gif?raw=true)

# Exporting & Rendering for iOS 13+
If you're creating a *Legacy* animation (iOS 12 <), you can render this with a white background and you're finished, you can skip to the deb preparation. If you're creating an animation for iOS 13+ which now supports the use of an Alpha layer for transparency, then you'll need to
# Add to Render Queue and Change the format to RGB + Alpha & Apple ProRes 4444
![Visual](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/21rgbalpha.gif?raw=true)
## Save it somewhere as an .MOV and let render.
![Visual](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/22render.png?raw=true)
# Now Convert by Right Clicking on the MOV and choosing 'Encode Selected Video Files', Set to HVEC 1080p Preserve Transparency
this finished .MOV is the final video file, if you know how to package your own debs then you are now finished!
![Visual](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/23convert.gif?raw=true)

# Packaging your Animation for AirPort iOS 13+
This is the deb file structure if you want to submit and publish for AirPort!
`Library/AirPortAnims/Custom/<Insert Name Here>/ProxCard_loop.mov`
![Visual](https://github.com/royalgraphx/AnimationKit/blob/master/Tutorial/24preparedeb.gif?raw=true)

