# Homogeneous Matrix

Homogeneous transformation matrices represent configurations, including positions and orientations. They are square matrices, usually $4 \times 4$ in 3D, combining translation and rotation. Multiplying them by augmented vectors transforms points or vectors. These matrices accurately represent spatial relationships and have applications in computer graphics, computer vision, and robotics.





The body frame is fixed and attaches to the moving body, while the space frame is a fixed reference frame in space. The body's configuration is expressed as the pair $(R, p)$ , where $R \in SO(3)$ is a $3 \times 3$ rotation matrix representing the orientation of the body frame relative to the space frame. Additionally, $p \in R^3 $ is a 3-vector representing the position of the body frame's origin relative to the space frame.