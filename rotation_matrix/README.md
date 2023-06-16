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