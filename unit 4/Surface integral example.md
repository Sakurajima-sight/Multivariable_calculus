
--- pic\Surface integral example.pdf_00.png ---

1. Surface integral example.
   曲面积分示例。

2. Practice computing a surface integral over a sphere. 
   练习在球面上计算曲面积分。

3. Background
   背景

1. Surface integrals
   表面积分

4. The task at hand: Surface integral on a sphere. 
   当前的任务：球面上的曲面积分。

5. In the last article, I talked about what surface integrals do and how you can interpret them.
   在上一篇文章中，我讨论了曲面积分的作用以及你如何可以解释它们。

6. Here, you can walk through the full details of an example. 
   在这里，你可以浏览一个例子的全部详细信息。

7. If you prefer videos you can also watch Sal go through a different example.
   如果你喜欢视频，你也可以看Sal走过一个不同的例子。

8. Consider the sphere of radius 2, centered at the origin. 
   考虑半径为2、以原点为中心的球体。

9. Your task will be to integrate the following function over the surface of this sphere:
   你的任务将是在这个球的表面上积分以下函数：

--- pic\Surface integral example.pdf_01.png ---

1. Step 1: Take advantage of the sphere's symmetry.
   步骤1：利用球的对称性。

2. The sphere with radius 2 is, by definition, all points in three-dimensional space satisfying the following property: 
   定义上，半径为2的球是三维空间中满足以下性质的所有点：

1. This expression is very similar to the function: 
   这个表达式与函数非常相似：

2. In fact, we can use this to our advantage.
   事实上，我们可以利用这个优势。

1. Concept check: When you evaluate $f(x, y, z) = (x - 1)^2+ y^2 + z^2$ on points that happen to be on the sphere with radius 2 , what simpler expression do you get?
   概念检查：当你在半径为2的球体上的点上计算 $f(x, y, z) = (x - 1)^2+ y^2 + z^2$ 时，你会得到什么更简单的表达式？

5. On the sphere, this is 4.
   在球上，这是4。

1. Keep in mind, $f(x, y, z)$ does not equal this simpler expression everywhere, but only on the points where $x^2 + y^2 + z^2 = 4$.
   请记住，$f(x, y, z)$并不在所有地方都等于这个更简单的表达式，只有在$x^2 + y^2 + z^2 = 4$的点上。

2. Since we will only integrate over points on this sphere, though, we can justifiably replace the function $f$ in the integral with this value.
   然而，由于我们只会对球体上的点进行积分，因此我们可以在积分中将函数$f$合理地替换为这个值。

--- pic\Surface integral example.pdf_02.png ---

1. Of course, this is not something you can do for every surface integral, but It's a good lesson to take advantage of symmetry when you can to make these integrals easier.
   当然，这并不是你可以对每个表面积分做的事情，但这是一个好教训，当你可以的时候，利用对称性可以使这些积分更容易。

2. Step 2: Parameterize the sphere.
   步骤2：参数化球面。

3. To relate this surface integral to a double integral on a flat plane, we need to first find a function which parameterizes the sphere.
   为了将这个表面积分与一个平面上的双重积分联系起来，我们首先需要找到一个参数化球面的函数。

4. Concept check: Which of the following functions parameterizes the sphere with radius 2? 
   概念检查：下列哪个函数参数化了半径为2的球体？

1. The first choice Is correct:
   第一项选择是正确的：

2. And you apply this to the region of the $ts$-plane where $0 \leq  t \leq  2\pi$ and $0\leq s\leq \pi$.
   你将其应用到$ts$平面上$0 \leq  t \leq  2\pi$和$0\leq s\leq \pi$的区域。

6. There are no two ways about it, parameterizing surfaces is hard. 
   毫无疑问，参数化表面是困难的。

7. The trick to a problem like this, where you need to recognize what surface a given function will parameterize, is to think about what happens when you freeze one variable and let the other one vary.
   对于这样的问题，你需要识别给定函数将参数化哪个表面，解决的技巧是思考当你冻结一个变量，让另一个变量变化时会发生什么。

--- pic\Surface integral example.pdf_03.png ---

1. For example, in the expression for $v(t, s)$ above, imagine freezing $s$ and let $t$ vary:
   例如，在上面对$v(t, s)$的表达中，想象冻结$s$并让$t$变化：

2. Since $x$ is proportional to $\cos(t)$, and $y$ is proportional to $\sin(t)$, letting $t$ range from $0$ to $2\pi$ will draw a circle around the $z$-axis:
   由于$x$与$\cos(t)$成正比，$y$与$\sin(t)$成正比，让$t$从$0$到$2\pi$变化将在$z$轴周围画出一个圆：

3. Let $t$ vary.
   让$t$变化。

1. Alternatively, imagine fixing $t$ and letting $s$ vary.
   或者，想象固定$t$，让$s$变化。

2. This one also draws a circle (can you see why?)
   这也会画出一个圆（你能看出为什么吗？）

3. Let $s$ vary.
   让$s$变化。

--- pic\Surface integral example.pdf_04.png ---

1. Now imagine letting $s$ range from 0 to $\pi$, meaning only half of the red circle shown in that last animation is drawn.
   现在想象让$s$的范围从0到$\pi$，这意味着在最后的动画中显示的红色圆圈只画了一半。

2. Rather than thinking of $t$ as a fixed amount, picture the entire circle that $t$ draws for each specific value of $s$.
   与其把$t$想象成一个固定的数量，不如想象出$t$为$s$的每一个特定值所画出的整个圆。

3. These circles will sweep over the sphere from top to bottom: Drawing a sphere.
   这些圆将从上到下扫过球体：绘制一个球体。

4. This is why we let $t$ range from 0 to $2\pi$, but we only let $s$ range from 0 to $\pi$.
   这就是为什么我们让$t$的范围从0到$2\pi$，但是我们只让$s$的范围从0到$\pi$。

5. Great! Now we have a formula for the parameterization $v(t, s)$ of the sphere, along with a corresponding region on the $ts$-plane.
   太好了！现在我们有了一个球面的参数化$v(t, s)$的公式，以及在$ts$-平面上对应的区域。

6. We can start expanding out surface integral like this: 
   我们可以开始这样展开表面积分：

1. $x$ -value of parameterization
   参数化的 $x$ 值

7. We need work this out.
   我们需要解决这个问题。

8. Step 3: Compute both partial derivatives
   步骤3：计算两个偏导数

9. The main beast to wrangle with in any surface integral is this little guy:
   在任何曲面积分中，主要难题是这个小家伙：

--- pic\Surface integral example.pdf_05.png ---

1. Concept check: To start, compute both partial derivatives of our parametric function: $v$.
   概念检查：首先，计算我们的参数函数 $v$ 的两个偏导数。

2. Step 4: Compute the cross product
   步骤 4：计算叉乘

3. Compute the cross product of the two partial derivative vectors that you just found.
   计算你刚找到的两个偏导数向量的叉乘。

--- pic\Surface integral example.pdf_06.png ---

1. Now apply the usual determinant trick for cross products:
   现在我们使用常用的交叉乘积行列式技巧：

2. We take this one component at a time.
   我们一次处理一个组件。

2. $i$ component:Cross out the top row and left column, then take the determinant: 
   $i$分量：划掉顶行和左列，然后取行列式：

3. $j$ component:Cross out the top row and middle column, then take the negative determinant: 
   $j$分量：划掉顶行和中列，然后取负行列式：

4. $k$ component: Lastly, and most nastily, cross out the top row and last column, then take the determinant: 
   $k$分量：最后，并且最复杂的是，划掉顶行和最后一列，然后取行列式：

5.  factor out $- 4 \sin(s) \cos(s)$
    提取出$- 4 \sin(s) \cos(s)$

6.  Step 5: Find the magnitude of the cross product.
    第5步：找出交叉乘积的大小。

--- pic\Surface integral example.pdf_07.png ---

1. Find the magnitude of the cross product that you just found. 
   找到你刚刚得到的叉积的大小。

2. Factor out $4^2$ 
  提出$4^2$的公因数 

1. Factor out $\sin^4(s)$
    提出$\sin^4(s)$的公因数

1. Factor out $\sin^2(s)$
    提出$\sin^2(s)$的公因数

1. Notice, technically the answer should have an absolute value sign in it.
   请注意，严格来说，答案中应该包含绝对值符号。

2. However, because our parameterization only applies to the region where $0 < s < \pi$, the value of $\sin(s)$ will always be positive anyway, so we are free to leave that out.
   但是，因为我们的参数化只适用于$0 < s < \pi$的区域，所以$\sin(s)$的值总是正的，所以我们可以省略它。

1. Step 6: Compute the integral 
   步骤6：计算积分

--- pic\Surface integral example.pdf_08.png ---

1. Taking everything we've done so far, here's what the surface integral has turned into: 
   将我们到目前为止所做的所有事情整合起来，这就是表面积分变成的样子：

2. As a the final step, compute this double integral. 
   作为最后一步，计算这个双重积分。
   
3. First, let's break this integral into two simpler ones:
   首先，让我们把这个积分分成两个更简单的积分：
   
   
4. Now let's go through each, one at a time:
   现在让我们一个一个地通过：
   
--- pic\Surface integral example.pdf_09.png ---

1. Well, that makes things easier! 
   好的，这让事情变得更容易！

2. What about the other integral:
   那么其他的积分呢：

1. Constant with respect to $t$.
   关于 $t$ 是常数。

3. Therefore, our final integral simplifies as
   因此，我们的最终积分可以简化为

