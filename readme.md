# Canvas Engine
http://canvasengine.net

## Description

Framework to create video games in HTML5 Canvas

## Get Started

Follow the steps below to start:

1. Download the code `canvasengine-X.Y.Z.all.min.js` on Github or this website
2. Add this code in your page : 
        
		<!DOCTYPE html>
		<script src="canvasengine-X.Y.Z.all.min.js"></script>
		<canvas id="canvas_id" width="640" height="480"></canvas>
		
       
3. Initialize the canvas in your JS file :

        var canvas = CE.defines("canvas_id").ready(function() {	
         
        });

Method `ready` is called when the canvas is ready (DOM loaded)

## Features

* Scene Structure
* Overlay scenes
* Multiplayer model
* Preloading
* Animations
* Timeline
* Collision (beetween entities and grid)
* Keyboard and Gamepad
* Windows
* Sound
* Text and Game effects
* Scrolling
* Level Design
* Save & Load
* Spritesheet Management
* Mouse Control & Multi Touch
* Elements Manipulation

## Editors
* Tiled Map Editor (http://www.mapeditor.org)
* Gleed 2d (http://gleed2d.codeplex.com)

## Roadmap (in order)

* Transition
* UI
* Box2d
* Synchronized multi canvas (local multiplayer)

## Test performance

### v1.0.6

* [Native class and CanvasEngine Class 1](http://jsperf.com/native-class-and-canvasengine-class)
* [Native class and CanvasEngine Class 2](http://jsperf.com/native-class-and-canvasengine-class-test2)

## Contributors

* [robwalch](https://github.com/robwalch) - [commit](https://github.com/robwalch/CanvasEngine/commit/e55909952c26ba1ec3e3d5bd6f733ddfffc4b647)

## Changelog

### v1.2.3

* Fix materials loading as `{id: Number, path: String}` ([Doc](http://canvasengine.net/doc/?p=core.materials.load))
* Fix `mouseover` and `mouseout`  ([Doc](http://canvasengine.net/doc/?p=core.element.events.on))
* Add `mouveEvent` property in Canvas class ([Doc](http://canvasengine.net/doc/?p=core.canvas.mouseEvent))
* Force `ready` method of canvas if the DOM is already loaded ([Doc](http://canvasengine.net/doc/?p=core.engine.ready))

### v1.2.2

* Fix scene reloaded
* Fix sounds for iOS

### v1.2.1

* Add getBasePath method in Materials class
* Add getFilename method in Materials class
* Add mousedown et mouseup events
* Add zIndex method in Scene class
* Fix mulit-touch gestures on touchpads
* Improve loading sounds

### v1.2.0

* Add Text feature
* Add Effect feature
* Add Cursor feature in Window class
* Add off method in Element class
* Add scroll method in Window class
* Add invertColor method in Materials class
* Add forceEvent property in Element class
* Add hasCmd method in Context class
* Add propagationOpacity property in Element Class
* Add mouseScroll method in Scrolling class
* Add random method in CanvasEngine Core
* Add freeze property in Scrolling class
* Add mobileUserAgent method in CanvasEngine core
* Fix event "canvas:render" when element is hidden
* Fix clip method in Context class
* Fix name attribute in Element class
* Fix value 0 in Timeline class
* Fix press method in Input class
* Fix load method in Materials class
* Fix animation construct in Animation class
* Fix load sound in cache
* Fix scrolling
* Fix measureText method in Canvas class
* Fix draw map in Tiled class
* Fix testCell method in Hit class
* Fix intersectsWith method in Polygon class
* Fix animation loop in Animation class
* Improve children method in Element class
* Improve position method in Window class
* Improve append method in Element class
* Improve clone method in Element class
* Improve reset method in Input class
* Improve load and dump methods in Marshal class
* Improve new method in CanvasEngine class
* Improve classes in Hit class
* Improve isPressed method in Input class
* Merge Hammer.js in CanvasEngine for multi touch feature

### v1.1.1

* Add testCell method in Grid class
* Add removeCmd method in Element class
* Add origin points in parameters in set method in SpriteSheet class
* Changing getEntityCells method in Grid Class
* Fix imageToCanvas method in Materials class
* Fix frequence in Animation class
* Fix set method in SpriteSheet class for windows
* getPropertyByCell method in Hit class returns undefined if column or row doesn't exist


### v1.1.0

* Add specific image param in animation
* Add position param in animation
* Add getStage method in Scene class
* Add getEnabled method in Scene class
* Add collision feature
* Add Window feature
* Add overlay scenes
* Add moveArray method in CanvasEngine Object
* Add offset method in Element Class
* Add position method in Element Class
* Add pack method in Element Class
* Add unpack method in Element Class
* Add detach method in Element Class
* Add children method in Element Class
* Add removeAttr method in Element Class
* Add prepend method in Element Class
* Add zIndex method in Element Class
* Add zIndexBefore method in Element Class
* Fix reload scene
* Fix click on multi scene
* Fix click on element witch opacity < 1
* Improving draw performance 
* Improving documentation (markdown)

### v1.0.8

* Add multi-tilemap in Tiled Class (robwalch)
* Add origin points in Spritesheet Class (robwalch)
* Fix keyUp method in Input Class (https://github.com/RSamaium/CanvasEngine/issues/4)
* Fix NPM problem (https://github.com/RSamaium/CanvasEngine/issues/7)
* Fix identifiers keys in Input class
* Fix addKey method in Input class
* Fix set method in Spritesheet class

### v1.0.7

* Move clear method (Context class -> Canvas class)
* Change exit method in Scene Class
* Add multi scenes feature.
* Add togglePause method in Scene Class
* Add pause method in Scene Class
* Add isEnabled method in Scene Class
* Add exitAll method in Scene Class
* Add eventExist method in Element Class
* Add alias for new method : New
* Improves the performance of clicks
* Fix [Info of tile size](https://github.com/RSamaium/CanvasEngine/issues/2)
* Fix "this_" in Marshal class
* Improving documentation

### v1.0.6

* Change addLoopListener method
* Ignore loading music if the type is not supported
* Add getExtension method in Materials class
* Add remove method in Marshal class
* Add special events defined by a namespace (methods: refresh)
* Add moveTo, lineTo, quadraticCurveTo, bezierCurveTo in Context
* Add addMethod method in Context Class
* Addition to loading the canvas for CocoonJS)
* Fix save and load (IE9+)
* Fix reference of image loaded (for CocoonJS)
* Fix click on element
* Fix Gamepad (Google Chrome)
* Fix extend Context Class
* Fix positions of a element's children resized
* Fix origin point of element's children
* Improving documentation

### v1.0.5

* Fix restart of animations (Animation Class)
* Fix children elements opacity
* Fix reading some element properties
* Fix positions of a element resized
* Add rgbToHex method in CanvasEngine object
* Add pattern method in Spritesheet class
* Add cropImage method in Materials class
* Add transparentColor method in Materials class
* Add imageToCanvas method in Materials class
* Add getScene method in Element class
* Add createPattern method in Canvas class
* Add createLinearGradient method in Canvas class
* Add createRadialGradient method in Canvas class
* Add addColorStop method in Canvas class
* Add measureText method in Canvas class
* Improving performance click
* Improving the get method in Materials class
* Improving documentation

### v1.0.4

* Fix animated images
* Improving documentation

### v1.0.3
Not indicated
### v1.0.2
Not indicated
### v1.0.1
Not indicated
### v1.0.0

* Initial Release

## Examples and Demos

http://rsamaium.github.com/CanvasEngine

## License

MIT. Free for commercial use.
