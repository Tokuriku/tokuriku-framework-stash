SceneSizer Framework API Document

All the methods in this framework are dependent on the "SceneSizer" Class and are Type Methods.

The main function you'll want to use is the public method:
calculateSceneSize(#initialSize: CGSize, desiredWidth: CGFloat, desiredHeight: CGFloat) -> CGSize
It requires the size of your SCREEN and the desired sizes of your SCENE.
It outputs a scene size that will always fit your scene padding either width or heigth.
ex: scene.size = SceneSizer.calculateSceneSize(initialSize: skView.bounds.size, desiredWidth: 768, desiredHeight: 1024)

Then if you use a anchorPoint that is CGPointZero (ignore if you use an anchorPoint of "0.5, 0.5"),
you'll need to know the point where to shift your anchor if the size of the scene was changed:
scene.anchorPoint = SceneSizer.calculateCGPointZero(#sceneSize: scene.size, desiredSceneWidth: 768, desiredSceneHeight: 1024)