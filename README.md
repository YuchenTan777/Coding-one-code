# Coding-one-code

## WHAT IS LOWPOLY 🧡💛💚💙💜🖤🤍🤎

Low Poly, in fact, is made up of a **triangular grid of shapes** that alternate with each other to form folds and then form new geometric shapes. The sharp edges and abstract shapes of the polygons are very reminiscent of computer games from the 90s, in a retro style. When Low poly contains more triangles or polymorphs, it gives a more realistic and rather futuristic feel.

To achieve the visual effect of Low Poly, we first need to divide the multiple color elements in the form of triangles, and the color of each small triangle comes from the corresponding position of the original color element. Then the triangles are spaced and colored, that is, filled with pure color, and the three-dimensional effect is formed by the contrast of color shades and shadows.

The reason for wanting to make the images in this style came from a love for the game *Monument Valley*. I think this visual style is very beautiful and regular and has an algorithmic beauty. So I wonder if there is a code that can help me make the image into this geometric style. In fact, it was a bit difficult for me to create 3D images, so I started with 2

![image](https://github.com/YuchenTan777/Codingone-Projectcode/blob/main/picture/pic%201.png)

## How to achieve it by code

### Delaunay triangulation
Theoretically, Low Poly is actually a polygon **triangulation method**. The triangulation method I use here is **Delaunay Triangulation**.
In fact, Delaunay triangulation is not an algorithm, but a definition of a **"good" triangular mesh**. Its excellent properties are the null circle property and the maximizing minimum angle property, which avoid the generation of **narrow triangles** and make Delaunay triangulation widely used.
![image](https://github.com/YuchenTan777/Codingone-Projectcode/blob/main/picture/del_tri.gif)
![image](https://github.com/YuchenTan777/Codingone-Projectcode/blob/main/picture/720px-Delaunay_Triangulation_(100_Points).svg.png)

### Sobel edge detection
Before Delaunay triangulation, **Sobel edge detection algorithm** is used to obtain the edges of the image, and then randomly generate points on the edges. 
Edge detection is a very important image feature extraction method in the field of computer vision, and is likewise a relatively well used feature extraction method. We use edge detection is to find the set of pixel points in the image where the pixel **brightness changes** dramatically, and usually these sets are often shown as contours.

### Coloring
After the first two key steps, we take a simpler approach to coloring - using the color at the center of each triangle as the color of the triangle. The calculation of the center position is very simple, just average the positions of the three vertices and you're done

## Work Flow
![image](https://github.com/YuchenTan777/Codingone-Projectcode/blob/main/picture/flow.jpg)

## Feelings
The biggest thing I learned from this project is the importance of code and the ability it takes to write it. In fact, I have done this effect many times with PS and it took a long time, but this code helps me to get this effect quickly and adjust it to the most preferred level. I also found out that writing code requires a lot of mathematical knowledge and strong logical thinking, both of which I need to keep improving in the future.

## TRY IT!💗
https://mimicproject.com/code/929601bf-e8b6-0f10-d32c-41e96c9ebc21
