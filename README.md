# HAICO
Retrieved from an already developped game similar at overcooked by daltonbr


![image](https://github.com/clounis/HAICO/assets/34571249/dcd47f8b-fbdf-4635-8d48-01198afafafa)


_**Disclaimer:** This is a fan-made game, inspired by one of my favorite franchises: Overcooked, an amazing couch-coop game.
All assets were created from scratch. This project doesn’t have any commercial goals or any legal affiliation with the original game or company.
This project is meant only for scientific research on human-artificial agent collaboration

## Game concept

In Undercooked, we have to process ingredients (chop & cook), mount them into plates, and finally serve the orders as they pop out as fast as you can, thus earning more points.

More complexity arises from twists on the levels, like physically separating parts of the kitchen or adding obstacles, different recipes, and processes.
Still, for this project, I set a clear goal to keep the scope small by building all the core mechanics to have a tight game loop using just one level.

## Core mechanics

* Selection of `Interactables` based on a mix of _proximity_ and _orientation_.
* **Pick/Drop** items base on the context.
* Raw ingredients from their crates.
* Chop items.
* Cooking Pan, with burning and cooking timers.
* Delivering (and evaluating of) plates.


## Interesting points

* **Asynchronous programming** in conjunction with Coroutines.
* `IPickable` interface and `Interactable` Abstract class
* Extensive use of [Pattern Matching](https://docs.microsoft.com/en-us/dotnet/csharp/pattern-matching) to handle the interaction between items.
* Use of the new (event-based) Unity Input System, allowing a seamless change between the keyboard and different brands of controllers.
* Several Particle Systems: smoke, steam, dust, stars.
* Some shaders in Shader Graph

## Tools

* **Unity** 2021.3.11f1 LTS
* Autodesk **Maya**, Adobe **Photoshop** , **Blender 3D** and **Illustrator**.

## Auxiliary tools


* UI animation using [LeanGUI](http://carloswilkes.com/Documentation/LeanGUI) and [LeanTransition](http://carloswilkes.com/Documentation/LeanTransition)
* [FBX Exporter](https://docs.unity3d.com/Packages/com.unity.formats.fbx@2.0/manual/index.html) - makes it easy to send geometry and animation to any application that supports FBX and back again with minimal effort.
