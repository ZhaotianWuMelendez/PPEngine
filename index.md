# PPEngine

### [Link to Repository](https://github.com/FernandoDavis/PPEngine)




# Introduction
***

The Platformer Programming Engine is a programming language based on Platform 2D (P2D) to simplify 2D video game creation, utilizing Scala. With Scala, we can enable features such as Concurrency (hyperthreading) which provide better efficiency and performance, allowing for more sophisticated 2D projects.
	
The goal of PPEngine and P2D is to make it accessible and fun to start on the journey of game design and programming without the need of extensive software development knowledge. Designing some easy to implement functions and using less variables, we can then shorten the amount of code needed to perform useful tasks such as creating game objects, managing behaviour and interactions between them, and to create controllers which manage inputs. These will be used in the same nature as object oriented programming, letting the user define the different game elements. These are core elements of 2D games that the user can then expand upon and mix as they like to develop their own programs and games.
 
# Guide
***

After declaring level, you may declare various objects within it. This straightforward process lets you focus on the ever-expandable positioning and qualities of game elements. 

Currently implemented objects:
		
Level(Name(String))
		
Player(xPosition(integer), yPosition(integer), skinTag (string), Behaviour(TypeDeclaration))
	The player object is controllable with WASD and Space for movement, animations and sounds with the included SpriteSheet, Sound classes are possible.
		
Object(xPosition(integer), yPosition(integer), textureTag(String), Behaviour(TypeDeclaration))
	Usable to create platforms, backgrounds, moving particles, and more. The Behaviour parameter allows for great flexibility with object customizability.
		
Enemy(xPosition (Integer), yPosition(integer), enemyTag(string))
	The various enemy classes have combinations of behaviours, posses sounds and animations, and are easily declared with enemyTags such as “enemy2”.

First declare a Level with a name. Then, place your objects. "end" marks the end of the list of objects in a given Level.

# Example Code
***
```scala
Level(MudWorld):
Object(100, 200, 500, 200, img1, Behaviour(none))
Object(95, 10, 50, 300, img1, Behaviour(none))
Object(605, 10, 50, 300, img1, Behaviour(none))
Object(200, 50, 50, 50, img1, Behaviour(jump+moveBackAndForth+followPlayer))
Player(400, 100, 40, 40, img1, Behaviour(none))
end
Level(Rubicks):
Object(220, 300,ufo, Behaviour(5,5,8,DEFAULT, False))
Object(160, 300,ufo, Behaviour(5,5,8,DEFAULT, False))
Object(60, 300,ufo, Behaviour(5,5,8,DEFAULT, False))
Enemy(100,500,enemy1)
Enemy(120,500,enemy2)
Player(70 , 100,ufo, Behaviour(5,5,8,DEFAULT, False))
end

```

---![Branching](https://i.imgur.com/VJ6MkEF.png)
---![Branching](https://i.imgur.com/Q17l01K.png)


# Video Demonstration
***

<iframe width="560" height="315" src="https://www.youtube.com/embed/3ToX_4zstz8" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

# How to Run
***
	Import from the PPEngine repository into an IDE (IntelliJ).
	Build Project (CTRL+F9)
	Write PPEngine code into the text file “PPEngineCode.txt”
	Run “Main1”.





