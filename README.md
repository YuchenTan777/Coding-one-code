# Coding-one-code

## WHAT IS LOWPOLY 🧡💛💚💙💜🖤🤍🤎

The so-called Low Poly is actually **composed of triangular mesh**, graphics are alternately connected to each other into broken lines, and then form a new geometric figure. The sharp edges and abstract shapes of the polygons are very reminiscent of computer games from the 90s, in a retro style. When Low poly contains more triangles or polymorphs, it gives a more realistic and futuristic feeling.

To achieve the visual effect of Low Poly, we first need to divide the multiple color elements in the form of triangles, and the color of each small triangle comes from the corresponding position of the original color element. Then the triangles are spaced and colored, that is, filled with pure color, and the three-dimensional effect is formed by the contrast of color shades and shadows.

![image](https://github.com/YuchenTan777/Codingone-Projectcode/blob/main/picture/pic%201.png)

## How to achieve it by code

### Delaunay triangulation
Theoretically, Low Poly is actually a polygon **triangulation method**. The triangulation method I use here is **Delaunay Triangulation**.
In fact, Delaunay triangulation is not an algorithm, but a definition of a **"good" triangular mesh**. Its excellent properties are the null circle property and the maximizing minimum angle property, which avoid the generation of **narrow triangles** and make Delaunay triangulation widely used.
![image](https://github.com/YuchenTan777/Codingone-Projectcode/blob/main/picture/del_tri.gif)
![image](https://github.com/YuchenTan777/Codingone-Projectcode/blob/main/picture/720px-Delaunay_Triangulation_(100_Points).svg.png)

Before Delaunay triangulation, Sobel edge detection algorithm is used to obtain the edges of the image, and then randomly generate points on the edges. 
Edge detection is a very important image feature extraction method in the field of computer vision, and is likewise a relatively well used feature extraction method. We use edge detection is to find the set of pixel points in the image where the pixel brightness changes dramatically, and usually these sets are often shown as contours.
