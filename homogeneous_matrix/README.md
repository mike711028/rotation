# Homogeneous Matrix

## Introduction

Homogeneous transformation matrices represent configurations, including positions and orientations. They are square matrices, usually $4 \times 4$ in 3D, combining translation and rotation. Multiplying them by augmented vectors transforms points or vectors. These matrices accurately represent spatial relationships and have applications in computer graphics, computer vision, and robotics.



/picture about boby frame and fixed frame/

The body frame is fixed and attaches to the moving body, while the space frame is a fixed reference frame in space. The body's configuration is expressed as the pair $(R, p)$ , where $R \in SO(3)$ is a $3 \times 3$ rotation matrix representing the orientation of the body frame relative to the space frame. Additionally, $p \in R^3 $ is a 3-vector representing the position of the body frame's origin relative to the space frame.

The configuration of a moving body is represented by the homogeneous transformation matrix T, which belongs to the Special Euclidean group SE(3). This group includes all 4x4 real matrices and represents the set of possible configurations known as rigid body motions. Alternatively, T can be expressed as the pair (R,p), where R is a 3x3 rotation matrix and p is a 3-vector. Utilizing 4x4 matrices simplifies algebraic calculations when working with these matrices to represent the configuration of a moving body.

## Properties of Homogeneous Transformation Matrices 

* Identity matrix: The identity matrix, denoted as I, represents a trivial form of a transformation matrix. It indicates that the orientation and origin of the body frame {b} are the same as the reference frame.

```math
\begin{bmatrix}
0 \\ 1 \\ 0 \\ 1
\end{bmatrix} 
=
\begin{bmatrix}
a & b & c & d \\
e & f & g & h \\
i & j & k & l \\
m & n & o & p
\end{bmatrix}
```


$$
\begin{bmatrix}
0 \\ 1 \\ 0 \\ 1
\end{bmatrix} 
=
\begin{bmatrix}
a & b & c & d \\
e & f & g & h \\
i & j & k & l \\
m & n & o & p
\end{bmatrix}
$$