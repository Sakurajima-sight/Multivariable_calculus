
--- pic\Tangent planes.pdf_00.png ---

1. Tangent planes
    切平面

2. Just as the single variable derivative can be used to find tangent lines to a curve, partial derivatives can be used to find the tangent plane to a surface.
    就像单变量导数可以用来找到曲线的切线一样，偏导数可以用来找到曲面的切平面。

3. Background:Partial derivatives
    背景：偏导数

4. What we're building to: A tangent plane to a two-variable function $f(x, y)$ is, well, a plane that's tangent to its graph.
    我们要讲解的是：两变量函数$f(x, y)$的切平面，好吧，就是与其图形相切的平面。

5. The equation for the tangent plane of the graph of a two-variable function $f(x, y)$ at a particular point $(x_0, y_0)$ looks like this: 
    在特定点$(x_0, y_0)$处，两变量函数$f(x, y)$图形的切平面的方程看起来像这样：

6. The task at hand: Think of a scalar-valued function with a two-coordinate input, like this one: 
    当前的任务：想象一个有两个坐标输入的标量值函数，像这样的一个：

7. Intuitively, it's common to visualize a function like this with its three-dimensional graph.
    直观上，我们通常会用三维图形来可视化这样的函数。

--- pic\Tangent planes.pdf_01.png ---

1. Remember, you can describe this graph more technically by describing it as a certain set of points in three-dimensional space.
    记住，你可以更技术性地描述这个图，将其描述为三维空间中的某一组点。

2. Specifically, it is all the points that look like this: 
    具体来说，所有的点都像这样：

1. Here, $x$ and $y$  can range over all possible real numbers.
    在这里，$x$和$y$可以覆盖所有可能的实数。

2. A tangent plane to this graph is a plane which is tangent to the graph.
    对于这个图来说，切平面是与图形相切的平面。

3. Hmmm, that's not a good definition. 
    嗯，这个定义不好。用语言描述这个很难，所以我将展示一个包含各种不同切平面的视频。

1. This is hard to describe with words, so I'll just show a video with various different tangent planes.
用语言描述这个很难，所以我将展示一个包含各种不同切平面的视频。

--- pic\Tangent planes.pdf_02.png ---

1. Tangent planes of various points.
    各点的切平面。

2. Key question: How do you find an equation representing the plane tangent to the graph of the function at some specific point $(x_0, y_0, f(x_0, y_0))$ in three-dimensional space?
    关键问题：如何找到一个方程，表示在三维空间中函数图形在某个特定点$(x_0,y_0, f(x_0, y_0))$上的切平面？

3. Representing planes as graphs: Well, first of all, which functions $g(x,y)$ have graphs that look like planes?
    将平面表示为图形：首先，哪些函数$g(x,y)$的图形看起来像平面？

--- pic\Tangent planes.pdf_03.png ---

1. A plane passing through $(2, 2, 2)$
    一条穿过$(2, 2, 2)$的平面

2. The slope of a plane in any direction is constant over all input values, so both partial derivatives $g_x$, and $g_y$, would have to be constants.
    平面在任何方向的斜率都是常数，所以偏导数$g_x$和$g_y$都必须是常数。

3. The functions with constant partial derivatives look like this:
    具有常数偏导数的函数看起来像这样：

1.  Here, $a$, $b$, and $c$ are each some constant.
    这里，$a$、$b$和$c$每一个都是某个常数。

2. These are called linear functions.
    这些被称为线性函数。

3. Well, technically speaking they are affine functions since linear functions must pass through the origin, but it's common to call them linear functions anyway.
    严格地说，它们是仿射函数，因为线性函数必须经过原点，但我们通常还是称它们为线性函数。

4. Question: How can you guarantee that the graph of a linear function passes through a particular point $(x_0, y_0, z_0)$ in space?
    问题：你如何能保证一个线性函数的图形会穿过空间中的一个特定点$(x_0, y_0, z_0)$？

5. One clean way to do this is to write our linear function as  
    做到这一点的一个清晰的方法是将我们的线性函数写为 

6. In effect, we have fixed the constant $c$  in the expression $ax + by + c$ to be $c = z_0 - ax_0 - by_0$.
    实际上，我们已经确定了表达式$ax + by + c$中的常数c，使其等于$c = z_0 - ax_0 - by_0$。

7. Concept check: With $g$ defined this way, compute $g(x_0, y_0)$.
    概念检查：以这种方式定义$g$，计算$g(x_0, y_0)$。


--- pic\Tangent planes.pdf_04.png ---

1. Writing $g(x,y)$ like this makes it clear that $g(x_0, y_0) = z_0$.
   这样写$g(x,y)$可以清楚地看出$g(x_0, y_0) = z_0$。

2. This guarantees that the graph of g must pass through $(x_0, y_0, z_0)$.
   这保证了g的图形必须通过$(x_0, y_0, z_0)$。

3. The other constants a and b are free to be whatever we want.
   其他常数a和b可以是我们想要的任何值。

4. Different choices for a and b result in different planes passing through the point $(x_0, y_0, z_0)$.
   对a和b的不同选择会导致不同的平面通过点$(x_0, y_0, z_0)$。

1. The video below shows how those planes change as we tweak a and b:
下面的视频展示了当我们调整a和b时，这些平面是如何变化的：

1. Equation for a tangent plane
切平面的方程

5. Back to the task at hand. We want a function $T(x, y)$ that represents a plane tangent to the graph of some function $f(x, y)$ at a point $(x_0, y_0, f(x_0, y_0))$.
   回到我们的任务。我们希望一个函数$T(x, y)$，它代表着在点$(x_0, y_0, f(x_0, y_0))$处与某个函数$f(x, y)$的图像相切的平面。

6. As you tweak the values of a and b, this equation will give various planes passing through the graph of f at the desired point, but only one of them will be a tangent plane.
   当你调整a和b的值时，这个等式会给出经过f的图像在所需点的各种平面，但只有其中一个会是切平面。

--- pic\Tangent planes.pdf_05.png ---

7. Of all the planes passing through $(x_0, y_0, f(x_0, y_0))$, the one tangent to the graph of f will have the same partial derivatives as f.
   在所有通过$(x_0, y_0, f(x_0, y_0))$的平面中，与f的图像相切的那一个平面将具有与f相同的偏导数。

1. Try it! Take the partial derivatives of the equation for T(x, y) above.
试试看！对上面的T(x, y)方程求偏导数。

8. Therefore setting $a = f_x(x_0, y_0)$ and $b = f_y(x_0, y_0)$ will guarantee that the partial derivatives of our linear function T match the partial derivatives of f.
   因此，设定$a = f_x(x_0, y_0)$和$b = f_y(x_0, y_0)$将保证我们的线性函数T的偏导数与f的偏导数匹配。

1. Well, at least they will match for the input $(x_0, y_0)$, but that's the only point we care about.
好吧，至少它们会对输入$(x_0, y_0)$匹配，但那是我们唯一关心的点。

1. Putting this together, we get a usable formula for the tangent plane.
把这些放在一起，我们得到了一个可用的切平面公式。

2. Example: Finding a tangent plane
示例：找一个切平面

--- pic\Tangent planes.pdf_06.png ---

9. Given the function $f(x, y) = \sin(x) \cos(y)$, find the equation for a plane tangent to the graph of f above the point $\left(\frac{\pi}{2}, \frac{\pi}{2}\right)$.
   给定函数$f(x, y) = \sin(x) \cos(y)$，找出在点$\left(\frac{\pi}{2}, \frac{\pi}{2}\right)$上方与f的图像相切的平面的方程。

10. The tangent plane will have the form $T(x, y) = f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0) + f(x_0, y_0)$.
    切平面将有形式$T(x, y) = f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0) + f(x_0, y_0)$。

1. Step 1: Find both partial derivatives of f.
步骤1：找到f的两个偏导数。

2. Step 2: Evaluate the function f as well as both these partial derivatives at the point $\left(\frac{\pi}{6}, \frac{\pi}{4}\right)$:
步骤2：在点$\left(\frac{\pi}{6}, \frac{\pi}{4}\right)$处评估函数f以及这两个偏导数：

--- pic\Tangent planes.pdf_07.png ---

1. Putting these three numbers into the general equation for a tangent plane, you can get the final answer.
    将这三个数字代入切平面的一般等式，你可以得到最后的答案。

12. A tangent plane to a two-variable function $f(x, y)$ is, well, a plane that's tangent to its graph.
    一个二元函数$f(x, y)$的切平面，就是切于其图像的平面。

1. The equation for the tangent plane of the graph of a two-variable function $f(x, y)$ at $(x_0, y_0)$ a particular point looks like this:$T(x, y) = f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0) + f(x_0, y_0)$. 
一个二元函数$f(x, y)$在特定点$(x_0, y_0)$处的切平面方程看起来像这样：$T(x, y) = f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0) + f(x_0, y_0)$.