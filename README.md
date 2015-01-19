# tokuriku-framework-stash
Here is all the small yet very useful Frameworks I built for my iOS Apps.

## SceneSizer
As the name implies, **SceneSizer** helps you resize a scene. It is a Framework for iOS Spritekit and will help with the black letterboxing that happens when you want to preserve the aspect ration of your scene (usually happens with .AspectFit). It will pad either the top and bottom or the left and right so that your original scene size is kept but the scene fills the screen. Obviously, since the padding adds points to your scene, you might like to set your anchorPoint to the original (0, 0) of the scene. There is a metod in this Framework to make this quite easy.

## HardwareScanner
A pure Swift solution to detect the Hardware Type of the device running the application.
