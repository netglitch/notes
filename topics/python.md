# Python

## PyGame
___

### Basic PyGame Window

A simple window with a game and event loop

```
import sys
import pygame

def run_game():
	"""The game function"""

	#Initialize imported pygame modules
	pygame.init()

	#initialize a window and returns a surface
	screen = pygame.display.set_mode((640,480))

	#Setting a background color
	screen.fill((255,0,0))

	#main game loop
	while True:
		#Check for events
		for event in pygame.event.get():
			if event.type == pygame.QUIT:
				sys.exit()

		#update the full display surface to the screen
		pygame.display.flip()

run_game()
```