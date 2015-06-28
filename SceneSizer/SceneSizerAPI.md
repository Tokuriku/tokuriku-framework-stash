# SceneSizer Framework API Document
#### Part of the Tokuriku-Framework-Stash GitHub Repository
https://github.com/Tokuriku/tokuriku-framework-stash

All the methods in this Framework are dependent on the "**SceneSizer**" Class and are **Type Methods**. This Framework is for **Xcode 6.3** and **Swift 1.2** or lower.

### Installation
To use this Framework:

1. Download the full Repository at https://github.com/Tokuriku/tokuriku-framework-stash
2. Take the Framework itself (the Lego block) in the **SceneSizer** folder and insert it into your project.
3. Make sure the Framework is not only linked but **Embedded** also in the project's General tab.
4. Call the framework with `import SceneSizer` before using it in a Class.

### Usage
The main method you'll want to use is the public method:

    calculateSceneSize(#initialSize: CGSize, desiredWidth: CGFloat, desiredHeight: CGFloat) -> CGSize

It requires the size of your **Screen** and the desired sizes of your **Scene**. It outputs a scene size that will always fit your scene padding either width or heigth.

ex:

    scene.size = SceneSizer.calculateSceneSize(initialSize: skView.bounds.size, desiredWidth: 768, desiredHeight: 1024)

Then if you use a anchorPoint that is **CGPointZero** (*ignore if you use an anchorPoint of "0.5, 0.5"*), you'll need to know the point where to shift your anchor if the size of the scene was changed:

    calculateCGPointZero(#sceneSize: CGSize, desiredSceneWidth: CGFloat, desiredSceneHeight: CGFloat) -> CGPoint

ex:

    scene.anchorPoint = SceneSizer.calculateCGPointZero(#sceneSize: scene.size, desiredSceneWidth: 768, desiredSceneHeight: 1024)

### Changelog
Current Version (1.1)
- Made the framework support Xcode 6.3 compiler

Version 1.0
- Full functionality
