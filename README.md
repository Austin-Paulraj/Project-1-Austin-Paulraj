# Project 1: Pinhole camera, rasterized display

Austin Paulraj — Submission for Project 1
Implemented is a Scene of a small patch of grass with pyramids acting as brushes and a blocky tree in the center (Kept very simple and straightforward)

Link to video presentation - https://youtu.be/-n9841k6pXo

The code implemented draws heavily from the given examples in the assignments/example rasterizer articles provided, but adapted to  host the multi-scene setup of the page.

As requested, the following were implemented:
Level 0 - A copy of the first assignment showing lines forming a basic block
Level 1 - The scene of the tree drawn in a 1600 x 1000 Canvas using built-in line-drawing functions
          Added a threshold on how far forward the camera is able to come into the scene, to stop any weird interactions or flipping of the scene.
Level 2 - A customized line-drawing function setup using Bresenham's line algorithm.
          This was applied to a "pseudo-320x200" canvas made by turning a block of pixels in the larger canvas into 1 single color
Level 3 - Applied triangular rasterization to color in the faces of the line meshes. 
          Also applied a rudimentary "z buffer" to track pixel occlusion and stop background pixels from jumping in front
          Continuing to use the custom line algorithm and a smaller canvas size
