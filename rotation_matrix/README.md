# Rotation Matrix
旋轉矩陣為一種兩個座標系的相對位置的敘述方法，例如要描述body-frame(簡稱w-frame)對於world frame(簡稱w-frame)的旋轉矩陣為

$$
R^w_b = 
\begin{bmatrix}
x^w_b & y^w_b & z^w_b  
\end{bmatrix}
$$

$R^w_b$為b-frame相對於w-frame的旋轉矩陣， $x^w_b$ 、 $y^w_b$ 、 $z^w_b$ 則是代表
$x_b$ 、 $y_b$ 、 $z_b$ 在w-frame中的表示方法

![Alt text](image/rotation_matrix_1.png)

假設原本b-frame和w-frame重合，b-frame繞著z軸旋轉90度，此時兩者的相對位置為

![Alt text](image/rotation_matrix_2.png)

那麼敘述兩者之間的旋轉矩陣為

$$
R^w_b = 
\begin{bmatrix}
x^w_b & y^w_b & z^w_b  
\end{bmatrix} = \begin{bmatrix}
0 & -1 & 0 \\
1 &  0 & 0 \\
0 &  0 & 1
\end{bmatrix}
$$

如果由z軸朝下看x-y平面的話，繞著z軸的轉動可以寫成

![Alt text](image/rotation_matrix_3.png)

$$
R^w_b(\theta = 90) = 
\begin{bmatrix}
x^w_b & y^w_b & z^w_b  
\end{bmatrix} = \begin{bmatrix}
\cos\theta & -\sin\theta & 0 \\
\sin\theta &  \cos\theta & 0 \\
0 &  0 & 1
\end{bmatrix}
$$