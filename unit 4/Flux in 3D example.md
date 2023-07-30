
--- pic\Flux in 3D example.pdf_00.png ---

1. Flux in 3D example
   三维通量示例

2. After learning about what flux in three dimensions is, here you have the chance to practice with an example.
   在学习了三维中的通量是什么之后，你有机会用一个例子来实践。

3. Background
   背景

4. Flux in three dimensions
   三维中的通量

5. Unit normal vector
   单位法向量

6. Surface integral
   表面积分

7. The steps
   步骤

8. In the last article, I talked about how the flux of a flowing fluid through a surface is a measure of how much fluid passes through that surface per unit of time.
   在上一篇文章中，我谈到了流体通过表面的通量是衡量单位时间内通过该表面的流体量的一个度量。

9. If that fluid flow is represented with a vector field $F(x, y, z)$, and if $S$ represents the surface itself, the flux is computed with the following surface integral: 
   如果该流体流动由向量场$F(x, y, z)$表示，并且如果$S$代表表面本身，则通量是用以下表面积分计算的：

10. The vector-valued function $n(x, y, z)$ gives the unit normal vector to $S$.
    向量值函数$n(x, y, z)$给出了$S$的单位法向量。

11. For closed surfaces, you typically choose an outward facing unit normal vector.
    对于闭合表面，你通常选择一个朝外的单位法向量。

12. In practice, there is quite a lot that goes into solving this integral.
    在实践中，解这个积分涉及的内容非常多。

13. Step 1: Rewrite the integral in terms of a parameterization of $S$, as you would for any surface integral.
    第1步：将积分重写为关于$S$的参数化，就像你对任何表面积分所做的那样。

1. Step 2: Insert the expression for the unit normal vector $n(x, y, z)$.
   第2步：插入单位法向量$n(x, y, z)$的表达式。

2. It's best to do this before you actually compute the unit normal vector since part of it cancels out with a term from the surface integral.
   最好在实际计算单位法向量之前做这个，因为其中的一部分会和表面积分中的一个项相消。

15. Step 3: Simplify the terms inside the integral.
    第3步：简化积分内的项。

16. Step 4: Compute the double integral.
    第4步：计算双重积分。

1. The problem
   问题所在

--- pic\Flux in 3D example.pdf_01.png ---

1. Consider the paraboloid graph defined by the following equation: 
   考虑由以下等式定义的抛物面图形：

1. Let $S$ be the portion of this paraboloid which sits above the $xy$-plane.
让$S$是这个抛物面坐在$xy$平面上方的部分。

1. Whoa, that ended up looking way more like a nuclear warhead than I intended.
   哇，这看起来比我打算的更像核战头。

2. Ah well, at least it makes clear what surface we're talking about.
   啊，无论如何，至少它明确了我们在谈论什么表面。

1. For flux integrals, we must specify the orientation of this surface.
   对于通量积分，我们必须指定这个表面的方向。

2. Let's orient it with outward-facing normal vectors, in the sense that the vectors $i$, $j$ and $k$ are all outward facing from the region under the paraboloid.
   让我们以外向法向量对其进行定向，这意味着向量$i$、$j$和$k$都从抛物面下的区域向外面。

4. Now imagine there is a fluid flowing around in three-dimensional space.
   现在想象有一个流体在三维空间中流动。

5. Let's say it flows along the vector field defined by the function $F(x, y, z)$.
   让我们说它沿着由函数$F(x, y, z)$定义的向量场流动。

5. Key question: What is the flux of this flowing fluid through the surface $S$?
   关键问题：这个流动的流体通过表面$S$的通量是多少？

--- pic\Flux in 3D example.pdf_02.png ---

1. Step 1: Rewrite the flux integral using a parameterization.
   第一步：使用参数化重写通量积分。

2. Right now, the surface $S$ has been defined as a graph, subject to a constraint on $z$.
   现在，表面$S$已经被定义为一个图形，受到$z$的约束。

3. But for computing surface integrals, we need to describe this surface parametrically.
   但是对于计算表面积分，我们需要参数化描述这个表面。

4. Luckily, this conversion is not too hard. 
   幸运的是，这种转换并不难。

1. You basically let one parameter play the role of $x$, while the other parameter plays the role of $y$: 
你基本上让一个参数扮演$x$的角色，而另一个参数扮演$y$的角色：

5. After writing this function, you still need to specify what region of the $ts$-plane corresponds with our surface $S$.
   编写了这个函数后，你仍然需要指定$ts$-平面的哪个区域与我们的表面$S$相对应。

6. This requires translating the constraint $z \geq  0$ into a constraint on $t$ and $s$.
   这需要将约束$z \geq  0$转化为对$t$和$s$的约束。

1. Concept check: What is the constraint on $t$ and $s$ which will ensure that the $z$-component of $v(t, s)$ is greater than or equal to 0?
   概念检查：对于$t$和$s$，有什么约束可以确保$v(t, s)$的$z$分量大于或等于0？

2. Write your answer as an inequality.
   将你的答案写成一个不等式。

--- pic\Flux in 3D example.pdf_03.png ---

1. We take the $z$-component of the definition and set it to be $\geq  0$.
   我们取定义的$z$-分量，并设定它为$\geq  0$。

2. To better understand what this region looks like, it helps to rearrange it a bit.
   为了更好地理解这个区域的形状，有助于稍微重新排列一下。

3. Written like this, it is easier to see that the region we care about is a disk of radius 2 centered at the origin of the $ts$-plane.
   这样写出来，更容易看出我们关心的区域是半径为2、以$ts$-平面原点为中心的圆盘。

4. Since this region is a disk with radius 2, let's name It $D_2$.
   由于这个区域是一个半径为2的圆盘，我们就把它命名为$D_2$。

5. Later down the road, we'll expand this fully as a set of bounds for $t$ and $s$, but while we work on all the innards of the integral it helps to just have a symbolic representation.
   稍后，我们将这个完全展开为$t$和$s$的一组界限，但是当我们在处理所有的积分内部时，有一个符号表示是有帮助的。

6. Writing our flux surface integral as a double integral in the parameter space, here's what we get:
   将我们的流量表面积分写为参数空间中的双重积分，我们得到的是：

--- pic\Flux in 3D example.pdf_04.png ---

1. Double integral in flat parameter space.
   在平面参数空间中的双重积分。

2. If this transition to a double integral in the parameter space seems unfamiliar, consider reviewing the article on surface integrals, or the one on surface area.
   如果在参数空间中转换为双重积分的过程对你来说不熟悉，可以考虑复习一下关于表面积分或表面积的文章。

3. Step 2: Insert the expression for a unit normal vector.
   第二步：插入单位法向量的表达式。

4. In a previous article, I talked about how you can find a function which gives the unit normal vector to a surface based on its parameterization $v(t, s)$.
   在之前的一篇文章中，我讨论了如何找到一个函数，该函数基于其参数化$v(t, s)$给出表面的单位法向量。

5. Basically, you normalize the cross product of the partial derivatives of $v(t, s)$ (boy is that a mouthful to say): 
   基本上，你需要将$v(t, s)$的偏导数的叉积进行归一化（哇，这可真不容易说清楚）：

6. Now, for those of you who just love computing the magnitude of cross products of partial derivative vectors, hold off for a moment.
   现在，对于那些喜欢计算偏导数向量叉积大小的人，暂时停一下。

7. When we insert this into the flux integral, that magnitude term cancels out.
   当我们将其插入通量积分时，那个大小项会被取消掉。

--- pic\Flux in 3D example.pdf_05.png ---

1. This is a bit detailed, but it's a very satisfying intuition once you wrap your mind around it.
   这有点详细，但一旦你理解透彻，就会有非常满足的直觉感。

2. Remember the intuition behind a flux integral: We divide the surface $S$ into many tiny pieces, and look at how much fluid flows through each one of them per unit time: 
   记住流通积分背后的直觉：我们将表面$S$划分为许多小片，看每个小片每单位时间内流过的流体量：

1. Flow through a single piece of area
流过单片面积的流量

1. Typically, we think of one of these tiny pieces of area as being a parallelogram, spanned by the two infinitesimal vectors $\frac{\partial v}{\partial t}dt$ and $\frac{\partial v}{\partial s}ds$.
   通常，我们认为这些小面积之一是一个平行四边形，由两个无穷小矢量$\frac{\partial v}{\partial t}dt$和$\frac{\partial v}{\partial s}ds$所跨越。

1. In the parameter space
   在参数空间中

2. On the surface $S$
   在表面 $S$ 上

--- pic\Flux in 3D example.pdf_06.png ---

1. Because this piece is so small, we can assume that all the fluid particles passing through it move with basically the same velocity vector, $F(v(t, s))$ for some point $(t, s)$ which lands you inside the piece.
   因为这个部分很小，我们可以假设所有通过它的流体粒子基本上都具有相同的速度向量$F(v(t, s))$，对于一些落在这个部分内的点$(t, s)$。

2. This means the volume formed by fluid passing through this piece forms a parallelepiped (my favorite word!), which is the three-dimensional analog of a parallelogram.
   这意味着通过这个部分流动的流体形成的体积形成了一个平行六面体（我最喜欢的词！），这是平行四边形的三维类比。

1. Let's assume the parallelepiped represents the fluid passing through the parallelogram over one unit of time.
   我们假设这个平行六面体代表了在一个时间单位内通过平行四边形的流体。

2. Then to find its volume, you want to multiply the area of the parallelogram by the component of the vector $F (v(t, s))$ which is perpendicular to that parallelogram.
   然后，要找到其体积，你要将平行四边形的面积乘以向量$F(v(t, s))$的那个与该平行四边形垂直的分量。

3. But think about what this cross product represents: 
   但是想想这个叉积表示什么：

4. It gives a vector perpendicular to the parallelogram, whose magnitude is the area of that parallelogram.
   它给出了一个垂直于平行四边形的向量，其大小就是那个平行四边形的面积。

5. So what is the meaning of this dot product: 
   那么，这个点积的意义是什么：

6. It will give the component of $F(v(t, s))$ that is perpendicular to the parallelogram, multiplied by the area of that parallelogram.
   它将给出$F(v(t, s))$的那个与平行四边形垂直的分量，并乘以那个平行四边形的面积。

7.  But this is exactly the volume we want!
    但这恰好就是我们想要的体积！

8.  When you pull out the $dt$ and $ds$ terms, whose product is $dA$, you get the integral that we found above after canceling out the norm of the cross product.
    当你取出$dt$和$ds$这两项，它们的乘积是$dA$，你就得到了我们在取消了叉积的范数之后上面找到的积分。

9.  Step 3: Expand the integrand.
    第3步：扩展被积函数。

10. Let's start by working out the cross product term: 
    让我们开始处理叉积项：

11. For reference, this was how I defined $v(t, s)$:
    供参考，这就是我如何定义$v(t, s)$的：

--- pic\Flux in 3D example.pdf_07.png ---

1. Now compute each partial derivative, then find their cross product. 
   现在计算每个偏导数，然后找到它们的叉积。

--- pic\Flux in 3D example.pdf_08.png ---

1. To take the cross product, use the usual determinant trick, where the $2^{nd}$ and $3^{rd}$ rows are the answers to the previous two questions: 
   要取叉积，使用通常的行列式技巧，其中第2行和第3行是前两个问题的答案：

2. For the $i$ component, cross out the top row and left column, then take the determinant.
   对于$i$组分，划掉上方的行和左边的列，然后取行列式。

3. For the $j$ component, cross out the top row and middle column, then take the negative determinant.
   对于$j$组分，划掉上方的行和中间的列，然后取负行列式。

4. Finally, for the $k$ component, cross out the top row and last column, then take the determinant:
   最后，对于$k$组分，划掉上方的行和最后的列，然后取行列式：

5. Concept check: Does the expression for $\frac{\partial v}{\partial t}\times\frac{\partial v}{\partial s}$ that you just found give an outward-facing or inward-facing normal vector?
   概念检查：你刚找到的 $\frac{\partial v}{\partial t}\times\frac{\partial v}{\partial s}$ 的表达式给出的是朝外的还是朝内的法向量？

6. Choose 1 answer:
   选择1个答案：

--- pic\Flux in 3D example.pdf_09.png ---

3. The best way to find out is to just plug in a specific input.
   找出答案的最好方法就是插入一个特定的输入值。

4. The easiest input is probably $(t, s) = (0,0)$, which corresponds to the very top of our paraboloid surface.
   最容易的输入值可能就是$(t, s) = (0,0)$，它对应我们抛物线表面的顶部。

1. This is a vector pointing straight up, which is outside the region enclosed by the paraboloid.
   这是一个指向上方的向量，它在由抛物线围成的区域外面。

2. Therefore, it is an outward-facing vector.
   因此，它是一个外向的向量。

3. If it was not, we would need to flip the sign of our surface integral.
   如果不是这样，我们需要改变表面积分的符号。

4. Next, write out the term $F(v(t, s))$ in terms of just $t$ and $s$.
   接下来，只用$t$和$s$来写出$F(v(t, s))$这个项。

5. For reference, this is how $F$ and $v$ are defined: 
   作为参考，这是$F$和$v$的定义方式：

--- pic\Flux in 3D example.pdf_10.png ---

1. Let's explicitly write the vector-valued function $v(t, s)$ as three separate scalar-valued functions: 
   让我们明确地将矢量值函数$v(t, s)$写成三个单独的标量值函数：

2. Plugging those into the definition of $F$, we get the following:
   将这些插入到$F$的定义中，我们得到以下内容：

3. Great! Now we have all the pieces for the innards of our integral.
   太好了！现在我们有了积分内部所需的所有部分。

4. By taking the dot product of the previous two answers, write the inside of this integral purely in terms of the parameters $t$ and $s$.
   通过取前两个答案的点积，纯粹地以参数$t$和$s$表示这个积分的内部。

5. It will help the integral computation in the next section if you simplify your answer as much as possible.
   如果你尽可能简化你的答案，将有助于下一部分的积分计算。


--- pic\Flux in 3D example.pdf_11.png ---

1. Factor out $4 - t^2 - s^2$
   提取出$4 - t^2 - s^2$因子

2. Factor out $s$
   提取出$s$因子

3. Step 4: Compute the integral.
   第4步：计算积分。

1. Up until this point, we have been writing a little $D_2$ under the double integral to indicate that the region of the $t s$-plane we will be integrating over is the disk with radius 2.
   到目前为止，我们在双重积分下面写了一个小的 $D_2$，以表示我们将在 $t s$ 平面上进行积分的区域是半径为2的圆盘。

4. Now, as we turn to computing the integral itself, we need to spell this out into concrete bounds on the parameters $t$ and $s$.
   现在，当我们转向计算积分本身时，我们需要将其详细到参数$t$和$s$的具体边界。

5.  To do this, draw yourself a picture of $D_2$, and imagine cutting it into vertical stripes.
   为了做到这一点，自己画一张$D_2$的图片，并想象将其切成垂直的条纹。


--- pic\Flux in 3D example.pdf_12.png ---

1. The value $t$ ranges from -2 to 2.
   $t$的值从-2到2。

2. The range for $s$ depends on the value of $t$, which you can find using the Pythagorean theorem.
   $s$的范围取决于$t$的值，你可以使用毕达哥拉斯定理找到这个值。

2. From the diagram, you can see that $s$ ranges from $-\sqrt{(4 - t^2)}$ to $+\sqrt{(4 - t^2)}$.
   从图中，你可以看到$s$的范围从$-\sqrt{(4 - t^2)}$到$+\sqrt{(4 - t^2)}$。

3. Applying these bounds to our double integral, here's what we get: 
   将这些边界应用到我们的双重积分，我们得到的是：

4. From here, there are a few ways you might finish the problem.
   从这里开始，你可能有几种方式来完成这个问题。

5. Painfully: Compute this double integral in full by hand (ugh!).
   痛苦地：用手完全计算这个双重积分（呃！）。

6. Pragmatically: Plug this into a calculator, or a computer algebra tool like Wolfram Alpha.
   实际地：将这个输入到计算器，或者像Wolfram Alpha这样的计算机代数工具。

7. Cleverly: You can recognize that the integrand is an odd function with respect to $s$.
   聪明地：你可以认出被积函数相对于$s$是一个奇函数。

8. Distribute the $s$, and notice that all terms either have an $s$ or an $s^3$.
   分配$s$，并注意所有的项要么有$s$，要么有$s^3$。

9. This means the inner integral on the portion from $-\sqrt{(4 - t^2)}$ to 0 will cancel out with the portion from 0 to $\sqrt{(4 - t^2)}$.
   这意味着从$-\sqrt{(4 - t^2)}$到0的部分的内部积分将与从0到$\sqrt{(4 - t^2)}$的部分相抵消。

10. Therefore, the integral as a whole is 0.
    因此，积分总和为0。

8. Summary: A flux integral starts its life looking something like this.
   总结：通量积分开始时看起来像这样。

--- pic\Flux in 3D example.pdf_13.png ---

1. Solving this involves the following four steps: 
   解决这个问题包括以下四个步骤：

2. Step 1: Parameterize the surface, and translate this surface integral to a double integral over the parameter space.
   第一步：参数化表面，并将此表面积分转换为参数空间上的双重积分。

3. Step 2: Apply the formula for a unit normal vector.
   第二步：应用单位法向量的公式。

4. Step 3: Simplify the integrand, which involves two vector-valued partial derivatives, a cross product, and a dot product.
   第三步：简化被积函数，这涉及到两个向量值的偏导数，一个叉积，和一个点积。

5. Step 4: Compute the double integral (in practice a computer can handle it from here).
   第四步：计算双重积分（实际上，从这里开始，计算机可以处理）。