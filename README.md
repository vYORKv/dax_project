# Data Visualizer Project
Made with Godot version v4.4.stable.official [4c311cbee]

This is a simple prototype of a data visualization application made for a friend. Currently, all it does is randomly spawn a circle of a starting color, then moves that circle down a line of nodes to combine their colors and output these combinations to a final color combination at the end of the chain. There is a reason for this odd movement and combination of colors traveling randomly down a chain of nodes, but that reasoning is beyond the scope of this repository.

## Personal Style Guide
- All self-defined functions use PascalCasing.
- All built-in engine functions are _snake_casing and .snake_casing().
- Node variables use PascalCasing (helps to remember we are referencing nodes
when we see these variables in the script and to separate them from 
int/float/bool variables of similar name).
- Constants (including pre-loaded scenes and assets) are SCREAMING_SNAKE_CASING.
- All other variables are snake_casing.

## Newcomer GDScript notes
- When instantiating a child scene follow this line of loading it into parent scene:
  
	var child_scene: Object = CHILD_SCENE.instantiate()

	add_child(child_scene)

	child_scene.position = PositionNode.global_position

	** Follow with any code setting values to child_scene **
