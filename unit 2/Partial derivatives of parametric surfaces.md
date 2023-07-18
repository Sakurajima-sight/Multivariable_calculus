

--- pic\Partial derivatives of parametric surfaces.pdf_00.png ---

1. Partial derivatives of parametric surfaces

   偏微分的参数曲面

2. If you have a function representing a surface in three dimensions, you can take its partial derivative.

   如果你有一个表示三维表面的函数，你可以对其进行偏导数。

3. Here we see what that looks like, and how to interpret it.

   这里我们看到它的样子以及如何解释它。

4. What we're building to.

   我们正在构建的内容。

5. As setup, we have some vector-valued function with a two-dimensional input and a three-dimensional output.

   作为设置，我们有一些具有二维输入和三维输出的向量值函数。

6. Its partial derivatives are computed by taking the partial derivative of each component.

   它的偏导数是通过对每个组件取偏导数来计算的。

7. You can interpret these partial derivatives as giving vectors tangent to the parametric surface defined by v.

   你可以将这些偏导数解释为给出与由v定义的参数曲面切线的向量。

--- pic\Partial derivatives of parametric surfaces.pdf_01.png ---

1. Suppose I were to give you a function with a two-dimensional input, and a three-dimensional output, like this one.

   假设我要给你一个有二维输入和三维输出的函数，像这样一个。

2. Since the input is multi-dimensional, you cannot take the ordinary derivative of this function, but you can take a partial derivative.

   由于输入是多维的，你不能对这个函数进行常规的求导，但你可以进行偏导。

3. The focus of this article is on getting an intuitive feel for what those partial derivatives mean.

   本文的重点是直观地了解这些偏导数的含义。

4. The function itself actually has a very nice geometric meaning.

   这个函数本身实际上有一个非常好的几何含义。

5. Since it has a two-coordinate input and a three-coordinate output, we can visualize it as a parametric surface.

   由于它有一个二维的输入和一个三维的输出，我们可以将它视为一个参数曲面。
6. Specifically, consider all inputs (t, s) such that 0 ≤ t ≤ 2π and 0 ≤ s ≤ 2π. This can be seen as a square in the "ts-plane". I'll draw this with a checkerboard pattern since it makes things easier to follow later on.

   具体来说，考虑所有输入(t, s)，满足0 ≤ t ≤ 2π 和 0 ≤ s ≤ 2π。这可以被视为"ts-平面"上的一个正方形。我将使用棋盘格图案来绘制它，因为这样在后面更容易理解。

7. For any given point (t, s), the value v(t, s) is some point in three-dimensional space.

   对于任意给定的点(t, s)，值v(t, s)是三维空间中的某一点。

8. Concept check: Evaluate v(π, π). In other words, where does the function v take the input (t, s) = (π, π)?

   概念检查：计算v(π, π)的值。换句话说，函数v在哪里取得输入(t, s) = (π, π)?


--- pic\Partial derivatives of parametric surfaces.pdf_02.png ---

1. If you imagine doing this computation for all inputs (t, s) in the square, getting some point in three-dimensional space each time, all of the resulting outputs will form a two-dimensional surface in three-dimensional space.

   如果你想象对正方形中的所有输入(t, s)进行这种计算，每次都能得到三维空间中的某个点，那么所有的输出结果将形成三维空间中的二维表面。

2. The result is a doughnut shape! Math folk call this a torus.

   结果是一个甜甜圈形状！数学家称之为圆环体。

--- pic\Partial derivatives of parametric surfaces.pdf_03.png ---

1. To compute a partial derivative of this function, you take the partial derivative of each individual component.

   要计算这个函数的偏导数，你需要对每个独立的组成部分求偏导数。

2. So...what does this new vector-valued function actually mean?

   那么...这个新的向量值函数实际上意味着什么？

3. Well, computing this partial derivative requires treating the variable s as if it was constant. What does this mean geometrically?

   嗯，计算这个偏导数需要把变量s当作常数处理。几何学上这意味着什么？

4. In the ts-plane, a constant value of s corresponds with a horizontal line. 
   
   在ts平面上，s的恒定值对应一条水平线。 

5. Here's one such line representing s = π/2, drawn in red:

   这是一条代表s = π/2的线，用红色画出：

6. After this square gets warped and morphed into the torus, this red line gets turned into some circle which goes the long way around the torus:

   在这个正方形扭曲并变形为环面之后，这条红线会变成一个环绕环面的长圆圈：

--- pic\Partial derivatives of parametric surfaces.pdf_04.png ---

1. The partial derivative $\frac{\partial \mathbf{v}}{\partial t}$ tells us how the output changes slightly when we nudge the input in the t-direction.

   偏导数告诉我们，当我们在t方向上稍微改变输入时，输出如何略微改变。

2. The partial derivative $\frac{\partial \mathbf{v}}{\partial t}$ tells us how the output changes slightly when we nudge the input in the t-direction.

   偏导数 $\frac{\partial \mathbf{v}}{\partial t}$ 告诉我们，当我们在t方向上轻轻推动输入时，输出会如何稍微变化。

3. In this case, the vector representing that nudge (drawn in yellow below) gets transformed into a vector tangent to the red circle which represents a constant value of s on the surface:

   在这种情况下，代表这种微调的向量（下面用黄色画出）被转化成了一个切于红圆的向量，该红圆代表了表面上s的常数值：

--- pic\Partial derivatives of parametric surfaces.pdf_05.png ---

1. Specifically, the input point used for the pictures above is $(t_0, s_0) = (\frac{\pi}{4}, \frac{\pi}{2})$.

   具体来说，上面图片使用的输入点是$(t_0, s_0) = (\frac{\pi}{4}, \frac{\pi}{2})$。

2. This means the point on the torus is 

   这意味着环面上的点是

3. And the tangent vector is 

   而切向量是  

--- pic\Partial derivatives of parametric surfaces.pdf_06.png ---

1. Concept check: Why does it make sense that the z-component of this tangent vector is 0?

   概念检查：为什么这个切线向量的z分量是0是有意义的？

2. The z-coordinate of all the points on the red circle representing s = π/2 is always 0.

   表示s = π/2的红圈上所有点的z坐标总是0。

3. The z-coordinate of all the points on the red circle representing s = π/2 does not change.

   表示s = π/2的红圈上所有点的z坐标不改变。

4. Differentiate with respect to s. The partial derivative with respect to s is similar.

   关于s进行微分。对s的偏导数是类似的。

5. You compute it by taking the partial derivative of each component in the definition of v 

   你可以通过计算v定义中每个组成部分的偏导数来计算它。   


6. This time, we can imagine holding t constant to get some vertical line in the parameter space.

   这次，我们可以想象将t保持恒定以获得参数空间中的一条垂直线。

--- pic\Partial derivatives of parametric surfaces.pdf_07.png ---

1. The yellow arrow represents some velocity vector as a particle travels up along this line.

   黄色箭头表示粒子沿着这条线向上移动时的一些速度向量。

2. Which is to say, as you vary s while holding t constant.

   也就是说，当你在保持t恒定的同时改变s。

3.After the square turns into the torus via the function v, the red line and the yellow velocity vector might look something like this:

   通过函数v，正方形变为环面后，红线和黄色速度向量可能看起来像这样： 

4. The partial derivative $\frac{\partial \mathbf{v}}{\partial t}$ can be interpreted as this resulting velocity vector on the torus.

   偏导数$\frac{\partial \mathbf{v}}{\partial t}$可以被解释为这个在圆环体上的结果速度向量。

5. As setup, we have some vector-valued function with a two-dimensional input and a three-dimensional output:

   在设置中，我们有一些向量值函数，具有二维输入和三维输出：

6. Its partial derivatives are computed by taking the partial derivative of each component:

   它的偏导数是通过计算每个组成部分的偏导数来得到的：

--- pic\Partial derivatives of parametric surfaces.pdf_08.png ---

1. You can interpret these partial derivatives as giving vectors tangent to the parametric surface defined by v.

   你可以将这些偏导数解释为给出与由v定义的参数曲面切线的向量。

2. For example, imagine nudging a point in the input space along the t direction, say from the coordinates (s,t) to the coordinates (s,t + h) for some small h.

   例如，想象沿着t方向在输入空间中轻轻推动一个点，比如从坐标(s,t)到坐标(s,t + h)的一些小h。

3. This results in some small nudge in the output along the surface, which is represented by the vector now $h \frac{\partial \mathbf{v}}{\partial t} (s, t)$.

   这将导致输出在表面上有一些小的推动，这被向量现在$h \frac{\partial \mathbf{v}}{\partial t} (s, t)$表示。