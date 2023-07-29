
--- pic\Double integrals over non-rectangular regions.pdf_00.png ---

1. Double integrals over non-rectangular regions
   非矩形区域上的双重积分

2. What makes double integrals tricky is finding the bounds in non-rectangular regions.
   使双重积分变得棘手的是在非矩形区域中找到边界。

3. Here we go through what that means and practice a few examples.
   在这里，我们将通过这个意思，并练习几个例子。

4. Background:
   背景

1. Double integrals
双重积分

5. What we're building to
   非矩形区域的例子

6. Example of a non-rectangular region
   我们正在构建的是

7. If you wish to perform an integral over a region of the $xy$-plane that is not rectangular, you have to express each of the bounds of the inner integral as a function of the outer variable.
   如果你希望在不是矩形的 $xy$  平面区域上执行积分，你必须将内部积分的每个边界表达为外部变量的函数。

8. Evaluates to some function of $y$
   计算得到的是 $y$ 的某个函数

9. or alternatively, Evaluates to some function of $x$
   或者，计算得到的是 $x$ 的某个函数


--- pic\Double integrals over non-rectangular regions.pdf_01.png ---

1. The trouble with non-rectangular regions
   非矩形区域的问题

1. Consider the function $f(x, y) = xy^2$.
   考虑函数 $f(x, y) = xy^2$。

2. Its graph looks like this:
   它的图像如下：

1. We will find the volume under a portion of this graph.
   我们将找到此图的一部分下的体积。

2. Unlike the last article, this volume will not lie above a rectangular region on the $xy$-plane.
   与上一篇文章不同，这个体积不会位于 $xy$-平面上的一个矩形区域之上。

4. Instead, we will look for a volume whose base is a triangle.
   相反，我们将寻找一个底面是三角形的体积。

5. The triangle pictured below, to be specific.
   具体来说，是下面描绘的三角形。


--- pic\Double integrals over non-rectangular regions.pdf_02.png ---

1. This is a right isosceles triangle, one of whose legs connects the points $(0, 0)$ and $(2,0)$ on the $x$-axis.
   这是一个直角等腰三角形，其中一条腿连接 $x$ 轴上的点 $(0, 0)$ 和 $(2,0)$。

2. The other leg connects the points $(2,0)$ and $(2,2)$.
   另一条腿连接点 $(2,0)$ 和 $(2,2)$。

3. The volume above this triangle and below the graph of $f(x, y) = xy^2$ looks like this: Volume under 
   这个三角形上方且 $f(x, y) = xy^2$ 图形下方的体积看起来像这样

1. $xy^2$ bounded by triangle.
三角形限定下的 $xy^2$ 下的体积。

4. This is similar to the problem I showed in the last article, which introduced the double integral.
   这个问题与我在上一篇文章中介绍的双重积分问题类似。

5. And indeed, the way to solve it is similar.
   确实，解决它的方法也类似。

6. Find a formula for slices of area using an integral.
   使用积分找到面积切片的公式。

7. Use a second integral to add those infinitely many slices of area into a volume.
   使用第二个积分将那些无穷多的面积切片累加成一个体积。

8. What gets tricky now is the bounds.
   现在变得棘手的是积分的界限。

9. For example, consider the slices of this volume which represent constant $x$ values.
   例如，考虑代表恒定 $x$ 值的这个体积的切片。

10. The following animation shows what these slices look like, as the constant $x$-value varies back and forth between 0 and 2.
    下面的动画显示了这些切片的样子，当恒定的 $x$ 值在 0 和 2 之间来回变化时。

--- pic\Double integrals over non-rectangular regions.pdf_03.png ---

1. The height of one of these slices changes based the height of the graph of $f(x,y) = xy^2$ above its base.
   这些切片中的一个的高度会根据其基底上 $f(x,y) = xy^2$ 图的高度而变化。

2. But the length of the base of the slice also changes.
   但是，切片的基底长度也会变化。

1. For example, when $x = 0.5$, the value of $y$ at the base can range from $0$ to $0.5$, as in the vertical red stripe pictured below.
   例如，当 $x = 0.5$ 时，底部的 $y$ 值可以从 $0$ 变化到 $0.5$，如下图中的红色垂直条纹所示。

2. Alternatively, when $x = 1.5$, the value of $y$ ranges from $0$ to $1.5$:
   或者，当 $x = 1.5$ 时，$y$ 的值范围从 $0$ 到 $1.5$：

3. This means when we set up an integral to find the area of one of these constant-$x$-value slices, the upper bound is written in terms of $x$.
   这意味着当我们设置一个积分来找到这些常数 $x$ 值切片之一的面积时，上界是以 $x$ 的形式写的。

--- pic\Double integrals over non-rectangular regions.pdf_04.png ---

1. As far as our computations are concerned, it's perfectly fine to have one of the bounds written in terms of $x$.
   就我们的计算而言，将其中一个界限写成 $x$ 的形式是完全没有问题的。

2. After all, we'll end up with an expression in terms of $x$ anyway.
   毕竟，我们最终还是会得到一个以 $x$ 为变量的表达式。

3. Go ahead and work out the integral for yourself: 
   你自己去计算这个积分：

4. Remember, in the eyes of the integral, $x$ is a constant, since it is an integral with respect to $y$ (as indicated by the "$dy$").
   记住，在积分看来，$x$ 是一个常数，因为它是关于 $y$ 的积分（如 "$dy$" 所示）。

5. From here, there is nothing new.
   从这里开始，没有新的内容。

6. Multiply this value by $dx$ to give it a little depth, and hence make it an infinitesimal volume.
   将这个值乘以 $dx$，使其具有一点深度，从而使其成为一个无穷小的体积。

7. Then when we integrate it with respect to $x$, the bounds are constants, $x = 0$ and $x = 2$, since this is where the base of our triangle sits on the $x$-axis.
   然后当我们对其进行关于 $x$ 的积分时，界限是常数，$x = 0$ 和 $x = 2$，因为这是我们的三角形的底边在 $x$ 轴上的位置。

8. The total volume is therefore $\frac{32}{15}$.
   因此，总体积为 $\frac{32}{15}$。

9. Integrating over a disk
   在一个圆盘上进行积分

10. Now let's try something a little harder: finding the volume under a graph bounded by the unit disk.
    现在让我们试试稍微难一点的事情：找出由单位圆盘限制的图形下的体积。

1. The unit disk on the $xy$-plane is all points $(x, y)$ such that $x^2 + y^2 \leq 1$
   在$xy$平面上的单位圆盘是所有满足$x^2 + y^2 \leq 1$的点$(x, y)$

--- pic\Double integrals over non-rectangular regions.pdf_05.png ---

1. For example, the volume underneath the graph $f(x,y) =3+y-x^2$ bound by the unit disk looks like this: 
   例如，单位圆盘约束下图形 $f(x,y) =3+y-x^2$ 下的体积看起来像这样：

1. Volume between $3+y-x^2$ and unit disk.
$3+y-x^2$ 和单位圆盘之间的体积。

2. Once again, consider slices of this volume which correspond to constant $x$-values: Slices of area under $3+y-x^2$ over unit disk.
   再次，考虑对应于常数 $x$ 值的这个体积的切片：单位圆盘上 $3+y-x^2$ 下的面积切片。

3. Think about what the base of each of these slices looks like on the $xy$-plane.
   想一想，每个切片在 $xy$ 平面上的基底看起来是什么样子。

4. Each slice corresponds with some vertical stripe in the unit disk.
   每个切片都对应单位圆盘中的某个垂直条纹。

--- pic\Double integrals over non-rectangular regions.pdf_06.png ---

1. Using the Pythagorean theorem, we can find the $y$-values which determine the top and bottom of this stripe as a function of the $x$-value that the stripe represents.
   使用勾股定理，我们可以找到确定这条带状部分顶部和底部的 $y$ 值，这些 $y$ 值是带状部分所代表的 $x$ 值的函数。

2. We can now find the area of one of these constant-$x$-value slices by integrating $f(x, y)$ with respect to $y$.
   我们现在可以通过对 $f(x, y)$ 按照 $y$ 进行积分，来找到这些恒定 $x$ 值切片的其中一个的面积。

3. Again, where this is different from the case of rectangular regions is that the bounds are each a function of $x$.
   再次强调，这与矩形区域的情况不同的地方在于，界限都是 $x$ 的函数。

4. Concept check: Which of the following integrals represents the area of a constant-$x$-value slice of the volume we are looking for?
   概念检查：以下哪个积分代表我们正在寻找的体积的恒定 $x$ 值切片的面积？

--- pic\Double integrals over non-rectangular regions.pdf_07.png ---

1. The first choice is correct: 
   第一个选择是正确的：

2. In this integral, $x$ should be thought of as a constant.
   在这个积分中，$x$ 应被视为一个常数。

3. The height of the slice at each point (as a function of $y$) is $f(x, y) = 3 + y - x^2$.
   每个点处的切片高度（作为 $y$ 的函数）是 $f(x, y) = 3 + y - x^2$。

4. The bounds for the $y$-value at the base of the slice are what we just found geometrically: $y = -\sqrt{1-x^2}$ and $y = \sqrt{1-x^2}$.
   切片基底处 $y$ 值的界限是我们刚刚在几何上找到的：$y = -\sqrt{1-x^2}$ 和 $y = \sqrt{1-x^2}$。

5. Work through it: This is a heavier computation than previous examples, but if you feel up to it, compute this integral to get a formula for the area of a constant-$x$-value slice, as a function of $x$.
   动手算一算：这比之前的例子计算量大，但如果你觉得可以的话，计算这个积分来得到一个公式，这个公式表示的是作为 $x$ 函数的恒定$x$值切片的面积。

3. Area of a constant-$x$-value slice:
   固定 $x$ 值切片的面积：

--- pic\Double integrals over non-rectangular regions.pdf_08.png ---

1. The $x$-values in the unit disk range from $x = -1$ to $x = 1$, so to find the volume we are looking for, integrate the expression you just found with respect to $x$ between the value $-1$ and $1$.
   单位圆盘中的 $x$ 值范围从 $x = -1$ 到 $x = 1$，所以要找到我们正在寻找的体积，就要将你刚刚找到的表达式对 $x$ 在 $-1$ 和 $1$ 之间进行积分。

2. As before, you can imagine this as adding up many, many paper-thin volumes.
   就像之前那样，你可以想象这就像是叠加许多许多纸薄的体积。

4. This turns out to be a tricky integral, but for pragmatism's sake we can solve it using any ol' computer algebra system or numerical integration tool, such as Wolfram Alpha.
   这实际上是一个棘手的积分，但为了实用，我们可以使用任何计算机代数系统或数值积分工具来解决，例如 Wolfram Alpha。

4. Total volume
   总体积

5. Slice the other way: Shark fin region.
   另一种切法：鲨鱼鳍区域。

6. Sometimes it's easier to consider constant-$y$-value slices, which involves cutting your region in $xy$-plane along horizontal stripes.
   有时候，考虑恒定 $y$ 值的切片更简单，这涉及在 $xy$ 平面上沿水平条纹切割你的区域。

--- pic\Double integrals over non-rectangular regions.pdf_09.png ---

1. This region kind of looks like a shark's dorsal fin.
   这个区域有点像鲨鱼的背鳍。

2. The upper right corner of the region is where the curve $x = y^2$ meets the line $x = y + 2$.
   区域的右上角是曲线 $x = y^2$ 与直线 $x = y + 2$ 相交的地方。

3. That point is $(4, 2)$.
   那个点是 $(4, 2)$。

4. Let's find the volume of a solid that has this region as its footprint, and whose height is determined by a relatively simple multivariable function: $f(x,y) = x+ 2y$.
   让我们找到一个实体的体积，该实体以这个区域为基础，其高度由一个相对简单的多变量函数 $f(x,y) = x+ 2y$ 确定。

5. Here's what the volume looks like: 
   下面是体积的样子：

1. Volume over shark fin region.
鲨鱼背鳍区域上的体积。

6. This time, imagine cutting constant-$y$-value slices of this volume.
   这次，想象一下切割这个体积的恒定 $y$ 值的切片。

4. This will give the area above a horizontal strip of our shark fin region, such as the one pictured below in red.
   这将给出我们鲨鱼鳍区域上方的一个水平条带的面积，如下图红色部分所示。

--- pic\Double integrals over non-rectangular regions.pdf_10.png ---

1. Concept check: If one of these horizontal stripes corresponds to a value $y$, what are the bounds on the $x$-value of the stripe?
   概念检查：如果这些水平条纹中的一条对应于一个值 $y$，那么这条纹的 $x$ 值的界限是多少？

1. That is, what are the $x$-coordinates of the left and right ends of this line as a function of $y$?
   也就是说，这条线的左端和右端的 $x$ 坐标作为 $y$ 的函数是什么？

2. Lower bound: $x = y^2$.
   下界：$x = y^2$.

3. Upper bound: $x = y + 2$.
   上界：$x = y + 2$.

3. These come directly from the definition of the region given above.
   这些直接来自上面给出的区域的定义。

4. Concept check: Which of the following integrals represents the slice of area above one of these stripes, and under the graph of $f(x, y) = x+ 2y$, as a function of $y$?
   概念检查：下面哪个积分代表了这些条纹中的一条上方的面积切片，并且在 $f(x, y) = x+ 2y$ 的图形下，作为 $y$ 的函数？

--- pic\Double integrals over non-rectangular regions.pdf_11.png ---

1. The first choice is correct.
   第一个选择是正确的。

2. The integration moves horizontally, as indicated by the "$dx$".
   如 "$dx$" 所示，积分在水平方向上进行。

3. It is also bounded by the values found in the last question, indicating that it stays within the shark fin region.
   它还受到上一个问题中找到的值的限制，表明它保持在鲨鱼鳍区域内。

4. Concept check: Solve this integral to find the area of the constant $y$-value slices of our volume.
   概念检查：求解这个积分，找出我们体积中恒定 $y$ 值切片的面积。

5. Area of constant-$y$-value slice: 
   恒定 $y$ 值切片的面积：      

6. Factor out $\frac{1}{2}$
   提取出 $\frac{1}{2}$

7. Concept check: When we integrate this function of $y$ to get the total volume, what bounds should we use?
   概念检查：当我们对 $y$ 的函数进行积分以得到总体积时，我们应该使用什么界限？

--- pic\Double integrals over non-rectangular regions.pdf_12.png ---

1. Looking at the picture of our shark fin region, $y$ varies from 0 to 2.
   看一下我们的鲨鱼鳍区域的图片，$y$ 的变化范围是从0到2。

2. Therefore, the second choice is correct.
   因此，第二个选择是正确的。

3. The integral giving our desired volume looks like this: 
   积分表达式代表我们想要的体积，看起来像这样：

4. Bring it on home: Solve this integral to find the volume of the region defined at the start of this section. (Feel free to use a calculator).
   最后一步：求解这个积分，找到本节开始定义的区域的体积。（可以使用计算器）。

--- pic\Double integrals over non-rectangular regions.pdf_13.png ---

1. When you need to perform a double integral over a non-rectangular region, follow these steps.
   当你需要对非矩形区域执行双重积分时，按照以下步骤进行。

2. Start by cutting your region along slices that correspond with holding one of the variables constant.
   首先，沿着与保持一个变量恒定相对应的切片来切割你的区域。

3. For example, holding $x$ at some constant value will give a vertical stripe of your region.
   例如，保持 $x$ 在某个恒定值将给出你区域的一个垂直条纹。

4. Find how to express the bounds of these stripes as a function of the other variable.
   找出如何将这些条纹的界限表示为另一个变量的函数。

5. For example, the top and bottom of a vertical stripe would be expressed as some function of $x$.
   例如，垂直条纹的顶部和底部将表示为 $x$ 的某个函数。

6. When you set up your double integral, the inner integral will correspond to integrating along one of these stripes, and each of its bounds will be a function of the outer variable.
   当你设置双重积分时，内部积分将对应于沿这些条纹之一进行积分，其每个界限都将是外部变量的函数。

4. If the inner integral corresponds to constant-$x$-values, the double integral as a whole might look like this:
   如果内部积分对应于常数 $x$ 值，那么整个双重积分可能看起来像这样：

4. Evaluates to some function of $x$
   计算得到的是 $x$ 的某个函数

--- pic\Double integrals over non-rectangular regions.pdf_14.png ---


1. Alternatively, if you started with horizontal constant-$y$-value slices, the double integral might look like this:
   或者，如果你从水平的常数 $y$ 值切片开始，双重积分可能看起来像这样：

2. Evaluates to some function of $y$
   计算得到的是 $y$ 的某个函数
