 --- pic\Curl warmup, fluid rotation in two dimensions.pdf_00.png ---

1. Curl warmup, fluid rotation in two dimensions
   卷曲预热，二维流体旋转

2. Curl measures the rotation in a fluid flowing along a vector field.
   卷曲度量了沿矢量场流动的流体的旋转。

3. Formally, curl only applies to three dimensions, but here we cover the concept in two dimensions to warmup.
   形式上，卷曲只适用于三维，但在这里我们将这个概念应用到二维来进行预热。

1. Background Partial derivatives Vector fields 
    背景 部分导数 向量场

2. Note: Throughout this article I will use the following convention: 
    注意：在这篇文章中，我将使用以下规定：

4. $i$ represents the unit vector in the x-direction. $j$ represents the unit vector in the y-direction.
   $i$代表x方向上的单位向量。$j$代表y方向上的单位向量。

3. What we're building to 
    我们将要构建的是

5. Curl measures the "rotation" in a vector field.
   卷曲度量了矢量场中的"旋转"。

4. In two dimensions, if a vector field is given by a function $\mathbf{v}(x, y)$ = $v_1(x, y) \mathbf{i} + v_2(x, y) \mathbf{j}$ , this rotation is given by the formula 
    在二维中，如果向量场由函数 $\mathbf{v}(x, y)$ = $v_1(x, y) \mathbf{i} + v_2(x, y) \mathbf{j}$

5. Rotation in fluid flow 
    流体流动中的旋转
6. Have $y_0$urself a nice swirly vector field :
    有一个好看的旋涡型向量场：

--- pic\Curl warmup, fluid rotation in two dimensions.pdf_01.png ---

1. This particular vector field is defined with the following function:
   这个特定的向量场是用以下函数定义的：

2. Now I want $y_0$u to imagine that this vector field describes a fluid flow, perhaps in a chaotic part of a river.
   现在我希望你想象一下，这个向量场描述的是流体流动，可能在河流的混乱部分。

3. The following video shows a simulation of what this might look like.
   下面的视频显示了这可能是什么样子的模拟。

4. A sample of fluid particles, shown as blue dots, will flow along the vector field.
   流体粒子样本，显示为蓝点，将沿着向量场流动。

5. This means that at any given moment, each dot moves along the arrow it is closest to.
   这意味着在任何给定的时刻，每个点都沿着它最近的箭头移动。
7. Focus in particular on what happens in the four circled regions. 
    特别关注四个圆圈区域中发生的情况。

--- pic\Curl warmup, fluid rotation in two dimensions.pdf_02.png ---

1. Amidst all the chaos, $y_0$u might notice that the fluid is rotating within the circled regions.
   在所有的混乱中，你可能会注意到流体在圆圈区域内旋转。

2. In the left and right circles, the rotation is counterclockwise, and in the top and bottom circles, the rotation Is clockwise.
   在左右两个圆中，旋转是逆时针的，在上下两个圆中，旋转是顺时针的。

8. Key Question $\mathbf{v}(x, y)$: If we are given a function that defines a vector $(x, y)$field, along with some specific point in space, , how much does a 0 0 fluid flowing along the vector field rotate at the point $(x, y)$? 
    关键问题 $\mathbf{v}(x, y)$: 如果我们得到一个定义向量$(x, y)$场的函数，以及空间中的某个特定点，那么在点$(x, y)$处，沿着向量场流动的流体旋转多少？

3. The vector calculus operation curl answer this question by turning this idea of fluid rotation into a formula.
   矢量微积分操作卷曲通过将流体旋转的这个概念转化为公式来回答这个问题。

9. It is an operator which takes in a function defining a vector field and spits out a function that describes the fluid rotation given by that vector field at each point. 
    它是一个操作符，它接受一个定义向量场的函数，并输出一个描述该向量场在每一点给出的流体旋转的函数。

4. Technically, the curl operation only applies to three dimensions.
   技术上来说，卷曲操作只适用于三个维度。

5. $y_0$u can see what that means and how it is computed in the next article, but in this article, we warm up by describing fluid rotation in two dimensions with a formula.
   你可以在下一篇文章中看到这意味着什么以及它是如何计算的，但在这篇文章中，我们通过一个公式描述二维流体的旋转来进行预热。
10. Capturing two-dimensional rotation with a formula 
    用公式捕捉二维旋转
11. One of the simplest examples of a vector field which describes a rotating fluid is 
     描述旋转流体的向量场的最简单示例之一是
12. Here's what it looks like. 
     它看起来是这样的。


--- pic\Curl warmup, fluid rotation in two dimensions.pdf_03.png ---

1. Animated, all the fluid particles just go in circles. 
   动画中，所有的流体粒子都只是在圆圈中运动。

2. In some sense, this is the most perfect example of counterclockwise rotation.
   在某种意义上，这是最完美的逆时针旋转的例子。

3. $y_0$u can understand the general formula for rotation in a two-dimensional vector field just by understanding why the function $\mathbf{v}(x,y) = -y\mathbf{i} + x\mathbf{j}$ gives counterclockwise rotation.
   你只需理解为什么函数$\mathbf{v}(x,y) = -y\mathbf{i} + x\mathbf{j}$会产生逆时针旋转，就可以理解二维向量场中旋转的一般公式。

--- pic\Curl warmup, fluid rotation in two dimensions.pdf_04.png ---
1. The $i$-component
    $i$分量
1. First, let's understand why the $-yi$ component suggests counterclockwise rotation. 
    首先，我们来理解为什么$-yi$分量暗示逆时针旋转。
2. Imagine a small twig sitting in our fluid, oriented parallel to the y-axis. 
    想象一下在我们的流体中有一小枝，它与y轴平行。
3. More specifically, let's say one end is at the origin (0,0), and the other is at the point (0, 2).
    更具体地说，我们假设一端在原点（0,0），另一端在点（0,2）处。
4. What does the $-yi$ component of the vector field imply for the fluid velocity at points on this twig?
    向量场的$-yi$分量对于这根小枝上的点的流体速度意味着什么？
5. This means the velocity at the top of the twig is $-2i$, a leftward vector, while the velocity at the bottom of the twig is 0.
    这意味着树枝顶部的速度是$-2i$，一个向左的矢量，而树枝底部的速度是0。
6. For the twig, this means the important factor for counterclockwise rotation is that vectors point more to the left as we move up the vector field.
    对于小枝来说，逆时针旋转的重要因素是，当我们向上移动矢量场时，矢量越来越向左指。
7. Said with a few more symbols, the important point here is that the i-component of a vector attached to a point $(x_0,y_0)$ decreases as $y_0$ increases.
    用更多的符号说，这里的重要点是，附着在点$(x_0,y_0)$上的矢量的i分量随着$y_0$的增加而减少。

2. Said with even more symbols, 
    用更多的符号来说，

8. Let's generalize this idea a bit. Question: Consider a more general vector field.
    让我们稍微概括一下这个想法。问题：考虑一个更一般的向量场。

--- pic\Curl warmup, fluid rotation in two dimensions.pdf_05.png ---
1. The components $v_1$ and $v_2$ are any scalar-valued functions.
    分量$v_1$和$v_2$是任何标量值函数。
2. If you place a small twig at some point $(x_0, y_0)$, oriented parallel to the y-axis, how can $y_0$u tell if the twig will rotate just by looking at $v_1$, $v_2$ and $(x_0, y_0)$?
    如果你在某点$(x_0, y_0)$放置一个小树枝，与y轴平行，你如何仅凭观察$v_1$、$v_2$和$(x_0, y_0)$就能判断树枝是否会旋转？
3. Look at the rate of change of $v_1$ as y varies near the point of interest, $(x_0, y_0)$: Suggests counterclockwise rotation if negative.
    观察y在兴趣点$(x_0, y_0)$附近变化时$v_1$的变化率：如果为负，则暗示逆时针旋转。
4. If this is negative, It indicates that vectors point more to the left as $y_0$ increases, so rotation would be counterclockwise.
    如果这是负数，它表示当$y_0$增加时，矢量更多地指向左侧，所以旋转将是逆时针的。
5. If it is positive, vectors point more to the right as $y_0$ increases, indicating a clockwise rotation.
    如果它是正数，当$y_0$增加时，向量更多地指向右侧，表明是顺时针旋转。

6. Next, let's see why the $xj$ component of the original vector field suggests counterclockwise rotation as well. 
    接下来，让我们看看原始向量场的$xj$分量为什么也暗示逆时针旋转。
7. This time, imagine a twig which is parallel to the x-axis. Specifically, put one end of the twig at the origin (0,0), and put the other at the point (2, 0).
    这次，想象一条与x轴平行的树枝。具体地说，把小枝的一端放在原点（0,0），另一端放在点（2, 0）处。
3. The vector attached to the origin is 0, but the vector attached to the other end at (2,0) is 2$j$, an upward vector.
    附着在原点的向量是0，但附着在(2,0)的另一端的向量是2$j$，一个向上的向量。

1. Therefore, the fluid pushes the right end of the stick upwards, and the left end experiences no force, so there will be a counterclockwise rotation. 
   因此，流体推动棒的右端向上，左端没有受力，所以会有一个逆时针的旋转。

--- pic\Curl warmup, fluid rotation in two dimensions.pdf_04.png ---

1. For this second twig, the vertical component of vectors increases as we move right, suggesting counterclockwise rotation.
    对于这第二根小枝，当我们向右移动时，向量的垂直分量增加，这暗示了逆时针旋转。
2. That is to say, the y component of a vector attached to a point $(x_0, y_0)$ increases as $x_0$ increases.
    也就是说，附在点$(x_0, y_0)$上的向量的y分量随着$x_0$的增加而增加。

4. In the case of a more general vector field function, 
    对于更一般的向量场函数，

1. We can measure this effect near a point ( $x_0$ , $y_0$ ) by looking at the change in $v_2$ as x changes.
   我们可以通过观察x变化时$v_2$的变化来测量在点($x_0$ , $y_0$)附近的这种效应。

1. Suggests counterclockwise rotation if positive 
    如果为正，则暗示逆时针旋转

3. Combining both components, the rotation of a fluid flowing along a vector field v near a point ($x_0$, $y_0$) can be measured using the following quantity.
    组合这两个分量，流动在向量场v附近的点（$x_0$, $y_0$）的流体的旋转可以用以下数量来测量。

5. When you evaluate this, a positive number will indicate a general tendency to rotate counterclockwise around ( $x_0$ , $y_0$ ) , a negative quantity indicates the opposite, clockwise rotation. If it equals 0 , there is no rotation in the fluid around ( $x_0$ , $y_0$ ). If you are curious about the specifics, this formula gives precisely twice the angular velocity of the fluid near ( $x_0$ , $y_0$ ). 
    当你评估这个时，一个正数将表示在（$x_0$，$y_0$）附近逆时针旋转的一般趋势，一个负数表示相反的，即顺时针旋转。如果等于0，那么在（$x_0$，$y_0$）附近的流体没有旋转。如果你对细节感到好奇，这个公式精确地给出了流体在（$x_0$，$y_0$）附近的角速度的两倍。

6. Some authors will call this the " two-dimensional curl " of v . This isn't standard, but let's write this formula as if " 2d-curl " was an operator.
    一些作者会称这为v的"二维旋度"。这不是标准的，但让我们写这个公式，就好像"2d-curl"是一个运算符。

7. Example: Analyzing rotation in a 2d vector field using curl 
    例子：使用旋度分析2d向量场中的旋转

--- pic\Curl warmup, fluid rotation in two dimensions.pdf_07.png ---
1. Problem: Consider the vector field defined by the function. Determine whether a fluid flowing according to this vector field has clockwise or counterclockwise rotation at the point p= $(0, \frac{\pi}{2})$.
    问题：考虑由函数定义的向量场。确定根据这个向量场流动的流体在点p=$(0, \frac{\pi}{2})$处是顺时针旋转还是逆时针旋转。
2. Step 1: Compute the 2d-curl of this function.
    步骤1：计算这个函数的2d-curl。

--- pic\Curl warmup, fluid rotation in two dimensions.pdf_08.png ---
1. We apply the 2d-curl formula we just found to this function. 
    我们将刚刚找到的2d-curl公式应用到这个函数上。
2. This will give us a new, scalar-valued function that indicates the rotation near each point. 
    这将给我们一个新的，标量值的函数，表示每个点附近的旋转。
3. Then, we'll plug in the point $(0, \frac{\pi}{2})$ to see whether the rotation there is positive (counterclockwise), zero, or negative (clockwise).
    然后，我们将插入点$(0, \frac{\pi}{2})$以看该处的旋转是正（逆时针），零，还是负（顺时针）。
4. Step 2: Plug in the point $(0, \frac{\pi}{2})$.
    步骤2：插入点$(0, \frac{\pi}{2})$。
5. Step 3: Interpret. How does the fluid tend to rotate near this point?
    步骤3：解释。流体在这个点附近如何倾向于旋转？
6. Because this is a positive value, the fluid will tend to flow counterclockwise at the point p.
    因为这是一个正值，所以流体在点p处将倾向于逆时针流动。

--- pic\Curl warmup, fluid rotation in two dimensions.pdf_09.png ---

1. Let's watch a sample of particles in this fluid flow: 
    让我们来观察这个流体流动中的一些粒子：

1. The point towards the top where all the particles congregate corresponds with p= $(0, \frac{\pi}{2})$: Particles rotate counterclockwise in this region, which should be consistent with $y_0$ur 2d-curl calculations.
    所有粒子聚集的最顶部的点对应于p= $(0, \frac{\pi}{2})$：粒子在这个区域内逆时针旋转，这应与你的2d-curl计算结果一致。
2. Summary: Curl measures the "rotation" in a vector field. In two dimensions, if a vector field is given by a function $\mathbf{v}(x,y)$=$v_1(x, y) \mathbf{i} + v_2(x, y) \mathbf{j}$, this rotation is given by the formula. 
    摘要：旋度测量向量场中的"旋转"。在二维中，如果向量场由函数$\mathbf{v}(x,y)$=$v_1(x, y) \mathbf{i} + v_2(x, y) \mathbf{j}$给出，那么这个旋转由公式给出。
3. On to the third dimension! The true curl operation, covered in the next article, extends this idea and this formula to three dimensions.
    进入第三维度！真正的Curl操作，在下一篇文章中介绍，将这个想法和这个公式扩展到三个维度。