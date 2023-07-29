


--- pic\Surface area integrals.pdf_00.png ---

1. Surface area integrals
   曲面积分

2. How do you find the surface area of a parametric surface?
   如何找到参数曲面的面积？

3. This will lead to the more general idea of a surface integral.
   这将引导我们理解曲面积分更一般的概念。

4. Background 
   背景 

1. Partial derivatives of parametric surfaces
参数曲面的偏导数


5. In particular, make sure you have a strong intuition for the partial derivatives of a function parameterizing a surface, and what they represent.
   特别是，要确保你对参数化曲面的函数的偏导数以及它们代表的含义有深刻的直觉。

6. Double integrals 
   双重积分 

1. Cross product (video)
叉积（视频）

1. What we are building to
   我们正在构建的是什么

1. Setup: $S$ is some surface in three-dimensional space.
设置：$S$是三维空间中的某个曲面。

2. $V(t, s)$ is a vector-valued function parameterizing $S$.
$V(t, s)$是参数化$S$的矢量值函数。

3. If you are unfamiliar with the idea of parameterization, see the article on parametric functions with two parameters.
   如果你对参数化的概念不熟悉，可以参阅关于两个参数的参数函数的文章。

4.  $T$ is the region of the $ts$-plane (also known as the parameter space) that corresponds with $S$.
    $T$是$ts$-平面（也称为参数空间）的区域，它对应于$S$。

5.  The surface area of $S$ can be computed with the following double integral: 
    $S$的表面积可以用以下的双重积分计算：

6.  These integrals can be very labor intensive to compute.
    这些积分可能需要大量的计算工作。

--- pic\Surface area integrals.pdf_01.png ---

1. Surface area
   表面积

2. From geometry, you might be familiar with the surface areas of a few specific shapes.
   从几何学中，你可能对一些特定形状的表面积很熟悉。

3. For example, the surface area of a sphere with radius $r$ is $4\pi r^2$.
   例如，半径为$r$的球体的表面积是$4\pi r^2$。

4. But what if someone gives you an arbitrary surface, defined using some parametric function that maps a region of two-dimensional parameter space into three-dimensional space?
   但是，如果有人给你一个任意的表面，这个表面是用一些参数函数定义的，这个函数将一个二维参数空间的区域映射到三维空间，那该怎么办？

5. How do you find its surface area?
   你如何找到它的表面积？

6. The answer is to use a certain integral, or rather a certain double integral, which you are about to learn.
   答案是使用一个特定的积分，或者更准确地说，一个特定的双重积分，这是你即将学习的。

7. This is analogous to how you can find the arc length of an arbitrary curve using a certain single integral, or the volume of a strangely shaped solid using the appropriate triple integral.
   这类似于你如何使用一个特定的单重积分找到任意曲线的弧长，或者使用适当的三重积分找到奇形怪状的实体的体积。

1. Example: Breaking down surface area
   示例：分解表面积

--- pic\Surface area integrals.pdf_02.png ---

1. Define a parametric surface with the following function:
   定义一个带有以下函数的参数曲面。

2. LeTs name this surface $S$.
   我们将此曲面命名为 $S$。

2. Of course, with parametric surfaces, it is not enough just to specify the function which parameterizes it.
   当然，对于参数曲面来说，仅指定参数化它的函数是不够的。

3. We also need to know the region of the parameter space that gets mapped onto the surface.
   我们还需要知道被映射到曲面上的参数空间的区域。

4. "Parameter space" is a fancy word for where the point $(t, s)$ lives, also known as the "domain".
   "参数空间"是一个高级词汇，用来描述点 $(t, s)$ 所在的位置，也称为"域"。

2. In this case, leTs say it is the rectangle defined by $-1 \leq t \leq 1$, $0 \leq s \leq 3$.
   在这种情况下，假设它是由 $-1 \leq t \leq 1$，$0 \leq s \leq 3$ 定义的矩形。

--- pic\Surface area integrals.pdf_03.png ---

1. LeTs call this rectangle $T$. 
   我们称这个矩形为$T$。

2. Here is what it looks like for $v$ to transform the rectangle $T$ in the parameter space into the surface $S$ in three-dimensional space.
   这就是在参数空间中，$v$将矩形$T$变换成三维空间中的曲面$S$的样子。

3. Our strategy for computing this surface area involves three broad steps:
   我们计算这个曲面积的策略包括三个大的步骤：

4. Step 1: Chop up the surface into little pieces.
   步骤1：将曲面切成小片。

5. Step 2: Compute the area of each piece.
   步骤2：计算每一块的面积。

6. Step 3: Add up these areas.
   步骤3：将这些面积加起来。

1. After studying line integrals, double integrals and triple integrals, you may recognize this idea of chopping something up and adding all its pieces as a more general pattern in how integration can be used to solve problems.
   在学习了线积分、双重积分和三重积分之后，你可能会认识到，这种将某物切割并加总所有部分的想法是一个更一般的模式，展示了如何使用积分来解决问题。


--- pic\Surface area integrals.pdf_04.png ---

1. As with those examples, our final computation will not actually involve chopping up the surface into a specific number of pieces and adding them up; we let an integral take care of that for us.
   就像那些例子一样，我们最终的计算实际上不会涉及将表面切成特定数量的片段并加起来；我们让积分替我们处理这个问题。

2. To be more precise, the integral we are shooting for will do something better than chopping up a surface and adding up the areas of each piece.
   更准确地说，我们所追求的积分会比切割表面和加起来每个片区的面积做得更好。

3. It considers what happens in the limit as you chop up the surface more and more finely into smaller and smaller pieces.
   它考虑了当你将表面切得越来越细，分成越来越小的片段时，极限会发生什么。

4. This is why it will give the exact surface area, not a mere approximation (as literal chopping would).
   这就是为什么它会给出精确的表面积，而不仅仅是一个近似值（就像字面上的切割那样）。

5. Step 1: Chopping up the surface
   第一步：切割表面

6. To start, think of chopping up the rectangle $T$ in the parameter space into many tiny little rectangles.
   首先，考虑在参数空间中将矩形$T$切成许多小矩形。

7. In the drawing, I'll only chop it into a few rectangles so that we can see and reference each one, but in principle you should think of very many, really small rectangles.
   在图中，我只会切成几个矩形，以便我们可以看到并参考每一个，但是原则上你应该想象有很多很小的矩形。

8. For one of these tiny rectangles, you can think its width as being $dt$, a tiny change to the parameter $t$.
   对于这些小矩形中的一个，你可以把它的宽度看作是$dt$，即参数$t$的微小改变。

9. Similarly, think of its height as being $ds$, a tiny change to the parameter $s$.
   同样，将其高度视为$ds$，即参数$s$的微小改变。


--- pic\Surface area integrals.pdf_05.png ---

1. Now consider how the function $v(t, s)$ maps one of these tiny rectangles onto the surface $S$.
   现在考虑函数$v(t, s)$如何将这些微小的矩形映射到表面$S$上。

1. In the following animation, I'll make most of the surface a faded grey, and leave just one of the tiny rectangles colored as we watch $T$ transform into $S$.
   在接下来的动画中，我会将大部分的表面变成淡灰色，只留下一个微小的彩色矩形，当我们看着$T$变成$S$时。

2. Parametric function applied to one small rectangle.
   参数函数应用到一个小矩形。

3. Strictly speaking, the rectangle will become slightly curved as It is pasted onto $S$. However, as you consider smaller and smaller rectangles, that curvature becomes more and more negligible, and we can basically treat this tiny piece as If it was flat.
   严格来说，当矩形贴在$S$上时，它会变得稍微弯曲。然而，当你考虑越来越小的矩形时，这个曲率就会变得越来越可以忽略不计，我们基本上可以把这个小片看作是平的。

--- pic\Surface area integrals.pdf_06.png ---

1. In fact, as we consider smaller and smaller rectangles in the parameter space, the portions of the surface S that these rectangles map to will look more and more like parallelograms.
   实际上，当我们考虑参数空间中越来越小的矩形时，这些矩形映射到的表面$S$部分会越来越像平行四边形。
   
2. In the parameter space.
   在参数空间。

3. On the surface $S$.
   表面$S$上。

4. Our first task, then, will be to find a formula giving the area of these parallelograms.
   因此，我们的首要任务是找到一个公式，给出这些平行四边形的面积。

5. Step 2: Seeking the area of a parallelogram piece.
   步骤2：寻找平行四边形片的面积。

6. For one of these tiny rectangles that we chopped $T$ into, let $(t_A, s_A)$ represent its lower left corner, and $(t_B, s_B)$ represent its lower right corner.
   对于我们切割的$T$中的一个小矩形，让$(t_A, s_A)$代表其左下角，$(t_B, s_B)$代表其右下角。

7. Now consider the vector pointing from $V(t_A, s_A)$ to $V(t_B, s_B)$ on the surface.
   现在考虑从表面上的 $V(t_A, s_A)$ 指向 $V(t_B, s_B)$ 的向量。

8. Let's name that vector $a$.
   我们将这个向量命名为 $a$。

--- pic\Surface area integrals.pdf_07.png ---

1. In the parameter space.
   在参数空间。

3. On the surface $S$.
   表面$S$上。

4. Concept check: If we describe the distance between $(t_A, s_A)$ and $(t_B, s_B)$ as being $dt$, which of the following expressions represents a good approximation of $a$? 
   概念检查：如果我们将$(t_A, s_A)$和$(t_B, s_B)$之间的距离描述为$dt$，那么以下哪个表达式可以很好地近似$a$？

5. The third answer choice is correct:
   第三个答案选择正确：


7. If this is confusing, or if it seems unfamiliar, consider reviewing the article on partial derivatives of parametric surfaces.
   如果这令你感到困惑，或者你对此不熟悉，建议你回顾一下关于参数曲面偏导数的文章。

8.  One way to think about this is to imagine traveling in the positive $t$ direction of the parameter space with a speed of $1$.
   想象一下，在参数空间中以速度 $1$ 沿正 $t$ 方向行进，这是一种理解这个问题的方式。

9.  If you map your motion onto the surface $S$, the function $\frac{\partial v}{\partial t}$ describes your velocity vector on that surface as a function of time.
    如果你将你的运动映射到表面 $S$ 上，那么函数 $\frac{\partial v}{\partial t}$ 将描述你在那个表面上的速度矢量作为时间的函数。

--- pic\Surface area integrals.pdf_08.png ---

1. In particular, if we consider the instant when you are passing the point $(t_A, s_A)$ in the parameter space, the corresponding velocity vector for your mapped-motion on $S$ is the partial derivative of $v$ with respect to $t$: $\frac{\partial v}{\partial t}(t_A, s_A)$.
特别的，如果我们考虑你通过参数空间中的点$(t_A, s_A)$的瞬间，你在$S$上的映射运动的对应速度向量是$v$关于$t$的偏导数：$\frac{\partial v}{\partial t}(t_A, s_A)$。

2. This is a three-dimensional vector.
这是一个三维向量。

1. Multiplying it by $dt", which can be thought of as a tiny change in time since your speed in the positive $t$-direction is 1, you will get a tiny change in displacement.
   将其乘以$dt$，可以认为是因为你在正$t$方向上的速度为1的微小时间变化，你将得到一个微小的位移变化。

2. This change in displacement is the vector in question.
   这个位移变化是问题中的向量。

1. It's worth noting that the partial derivative $\frac{\partial v}{\partial t}(t_A, s_A)$ is a vector which doesn't really care about the location of $(t_B, s_B)$.
   值得注意的是，偏导数$\frac{\partial v}{\partial t}(t_A, s_A)$是一个向量，它并不真正关心$(t_B, s_B)$的位置。

2. However, scaling it down by $dt$ is what gives it just the right length to reach $(t_B, s_B)$.
   然而，通过$dt$来缩放它，就能赋予它刚好到达$(t_B, s_B)$的长度。

1. Concept check: Take the same setup as the previous problem, but let $(t_C, s_C)$ be the upper left corner of the tiny rectangle.
   概念检查：取与前一个问题相同的设置，但让$(t_C, s_C)$成为小矩形的左上角。

2. Let's give the vector pointing from $v(t_A, s_A)$ to $v(t_C, s_C)$ a name, $b$.
   我们给从$v(t_A, s_A)$指向$v(t_C, s_C)$的向量一个名字，$b$。

4. In the parameter space.
   在参数空间。

5. On the surface $S$.
   表面$S$上。

6. If we describe the distance between $(t_A, s_A)$ and $(t_C, s_C)$ as being $ds$, which of the following best approximates $b$?
   如果我们描述$(t_A, s_A)$和$(t_C, s_C)$之间的距离为$ds$，那么以下哪个最能近似$b$？

--- pic\Surface area integrals.pdf_09.png ---

1. This time the fourth answer choice is correct:
   这次，第四个答案选项是正确的。

2. The reasoning is essentially identical to that of the previous question.
   其推理基本上与前一个问题相同。

2. Okay, here's where we are so far: We are thinking about a tiny rectangle in the parameter space with the following properties.
   好的，到目前为止我们在这里：我们正在考虑参数空间中具有以下特性的一个小矩形。

1. Bottom left corner: $(t_A, s_A)$
   左下角：$(t_A, s_A)$

2. Width: $dt$
   宽度：$dt$

3. Height: $ds$
   高度：$ds$

4. When you apply the function $v$ to this rectangle, you end up with what is basically a parallelogram on the surface $S$.
   当你将函数$v$应用到这个矩形时，你最终得到的基本上是表面$S$上的一个平行四边形。

5. Based on the previous two questions, the sides of this parallelogram are determined by the vectors $\frac{\partial v}{\partial t}(t_A, s_A)$ and $\frac{\partial v}{\partial s}(t_A, s_A)$
   根据前两个问题，这个平行四边形的边由向量 $\frac{\partial v}{\partial t}(t_A, s_A)$ 和 $\frac{\partial v}{\partial s}(t_A, s_A)$ 确定。

6. In the parameter space.
   在参数空间。

7. On the surface $S$.
   表面$S$上。

--- pic\Surface area integrals.pdf_10.png ---

1. Concept check: If the side lengths of a parallelogram in three-dimensional Space are described with the vectors $a$ and $b$, as pictured to the right, which of the following represents the area of that parallelogram? 
   概念检查：如果三维空间中的一个平行四边形的边长由向量$a$和$b$描述，如右图所示，那么以下哪一项代表该平行四边形的面积？

1. We couldn't grade your answer.
   我们无法评估您的答案。

2. It looks like you left something blank or entered in an invalid answer.
   看起来你可能漏掉了什么或者输入了无效的答案。

1. The second answer choice is correct: 
   第二个答案选项是正确的：

1. Recall how to interpret the cross product.
回忆一下如何解释叉积。

2. It returns a vector which is perpendicular to both $a$ and $b$, and whose magnitude equals the area of a parallelogram spanned by those two vectors.
   它返回一个与$a$和$b$都垂直的向量，其大小等于由这两个向量张成的平行四边形的面积。

1. If this is unfamiliar, consider reviewing the video about cross product intuition.
   如果这个概念不熟悉，可以考虑回顾一下关于叉积直观理解的视频。

3. Concept check: Putting all this together, when $v(t, s)$ maps the little $dt$-by-$ds$ rectangle with lower-left corner $(t_A, s_A)$ onto some parallelagram on the surface $S$, what is the area of that parallelogram? 
   概念检查：将所有这些放在一起，当$v(t, s)$将左下角为$(t_A, s_A)$的小的$dt$-by-$ds$矩形映射到表面$S$上的一些平行四边形时，那个平行四边形的面积是多少？

--- pic\Surface area integrals.pdf_11.png ---

1. The third answer choice is correct:
   第三个答案选择是正确的：

2. Where this gets labor intensive.
   在哪里，这变得劳动密集。

1. Boy is this a complicated expression.
   这真是个复杂的表达式。

2. It involves two partial derivatives of a vector-valued function, taking their cross product, then taking the magnitude.
   它涉及到一个向量值函数的两个偏导数，取它们的叉积，然后取模。

2. It's as if someone was trying to create the most complicated expression they could imagine.
   就好像有人试图创造他们能想象到的最复杂的表达式。

4. Right now we have a purely theoretical expression for the area of one of these little parallelograms: 
   现在我们有了一个纯理论的表达式，用于计算这些小平行四边形中一个的面积：

1. However, if you want to get a feel for what this actually entails, I encourage you to work through it.
   然而，如果你想了解这实际上涉及到什么，我鼓励你去深入研究它。

2. Work it out: Given the definition of $v(t, s)$ that we started with, $v$ evaluate the expression found in the previous question to get a function in terms of $t$, $s$, $dt$, and $ds$.
   解答：给定我们开始时的 $v(t, s)$ 的定义，$v$ 评估上一个问题中找到的表达式，得到一个关于 $t$、$s$、$dt$ 和 $ds$ 的函数。

3. Area of the parallelogram:
   平行四边形的面积：

--- pic\Surface area integrals.pdf_12.png ---

1. Before diving into anything, notice that we can factor out the $dt$ and $ds$ terms from our expression.
   在深入研究任何事情之前，注意到我们可以从我们的表达式中提取出 $dt$ 和 $ds$ 这两项。

2. This is because they are each there to represent some length, which is constant, and both cross products and absolute values each allow us to factor out constants. 
   这是因为它们每一个都在那里代表一些长度，这个长度是常数，而且交叉乘积和绝对值都允许我们提取出常数。

1. Factor out 提取出

1. Next, let's compute each partial derivative.
   接下来，我们计算每个偏导数。

3. Moving right along, now compute the cross product of these two vectors using the usual determinant trick:
   继续向前，现在使用通常的行列式技巧计算这两个向量的叉积：


--- pic\Surface area integrals.pdf_13.png ---

1. Finally, we compute the norm of this vector. 
   最后，我们计算这个向量的范数。

2. That is to say, when you map a tiny $dt$-by-$ds$ rectangle from the parameter space onto the surface $S$ using the function $v(t, s)$, it turns into a parallelogram with the following area: 
   也就是说，当你使用函数$v(t, s)$将参数空间中的一个微小的$dt$乘以$ds$的矩形映射到表面$S$上时，它变成了一个平行四边形，面积如下：

3. Step 3: Integrating everything together.
   步骤3：将所有东西整合在一起。

1. Here's where we are so far.
   到目前为止我们在这里。

2. After breaking up the rectangle $T$ of the parameter space into many tiny little rectangles, I told you that those rectangles get turned into parallelograms on the surface $S$.
   在将参数空间中的矩形$T$分解成许多小矩形后，我告诉你那些矩形在表面$S$上变成了平行四边形。

5. Well, more accurately, they each get turned into some slightly curved piece of $S$, which can be well-approximated by a parallelogram.
   更准确地说，它们每一个都会变成$S$的一部分稍微弯曲的部分，这可以很好地用平行四边形来近似。

6. The smaller your initial rectangle, the more accurate the approximation.
   你的初始矩形越小，近似值就越准确。

7. Then, through many computations, you found an expression for the area of one of these parallelograms: 
   然后，通过许多计算，你找到了这些平行四边形之一的面积表达式：

1. Where $(t, s)$ describes the position of the initial little rectangle.
   其中，$(t, s)$ 描述了初始小矩形的位置。

2. $dt$ is its width.
   $dt$ 是它的宽度。

3. $ds$ is its height.
   $ds$ 是它的高度。

--- pic\Surface area integrals.pdf_14.png ---

1. In the parameter space.
   在参数空间。

7. On the surface $S$.
   表面$S$上。

7. To add up the areas of all these little parallelograms, we take a double integral of this quantity over the region $T$.
   为了加起所有这些小平行四边形的面积，我们在区域$T$上对这个量进行双重积分。

8. As a reminder, $T$ was defined as the region where $-1\leq t\leq 1$, $0\leq s\leq 3$.
   提醒一下，$T$被定义为区域，其中$-1\leq t\leq 1$，$0\leq s\leq 3$。

9. Using those bounds, here is the double integral representing the surface area of $S$: 
   使用这些边界，这就是表示$S$的表面积的双重积分：

--- pic\Surface area integrals.pdf_15.png ---

1. Working this out by hand seems tricky, given that finding the antiderivative of $\sqrt{s^2+4t^2+4t^4}$ will be difficult.
   手动计算这个似乎有些棘手，因为找到 $\sqrt{s^2+4t^2+4t^4}$ 的原函数将会很困难。


2. But using a calculator (or Wolfram Alpha), we can find the answer:
   但是使用计算器（或Wolfram Alpha），我们可以找到答案：

3. The important thing to remember here is how to construct the appropriate double integral, and to think about adding up many tiny pieces of area on the surface itself. 
   这里需要记住的重要一点是如何构建适当的双重积分，并思考在表面上累加许多微小的面积部分。

4. Summary: This ain't easy.
   总结：这并不容易。

5. Generalizing everything we did in the previous example, the surface area of our parametric surface $S$ is expressed using the integral.
   将我们在前面的例子中做的所有事情进行概括，参数表面$S$的表面积是用积分表示的。

6. where $S$ is described using a parametric function $v(t, s)$ applied to a region $T$ of the $ts$-plane.
   其中$S$是用参数函数$v(t, s)$描述的，应用于$ts$-平面的区域$T$。

7. You've already had a glimpse of this, but it's worth pointing out that this can be a really complicated thing to compute.
   你已经瞥见了这一点，但值得指出的是，这可能是一个非常复杂的计算问题。

8. First you have to take two partial derivatives of vector-valued functions, which if you count each component includes 6 partial derivatives in total.
   首先，你必须对向量值函数求两个偏导数，如果你计算每个分量，总共包含6个偏导数。

9. You then have to take the cross product of these two partial derivative vectors, which itself requires taking a determinant whose components are vectors and functions.
   然后，你必须取这两个偏导数向量的叉积，这本身需要取一个其分量是向量和函数的行列式。

10. Then you have to compute the norm of that cross product.
    然后你必须计算那个叉积的范数。

11. After all that, there is still a double integral ahead of you.
    在所有这些之后，你还有一个双重积分在前面。

12. And remember, just setting up a double integral isn't always easy, especially if the region you are integrating over is not rectangular.
    记住，建立一个双重积分并不总是容易的，特别是如果你要积分的区域不是矩形的。

13. And all this is assuming you already know the function $v(t, s)$ and the region $T$.
    所有这些都假设你已经知道函数$v(t, s)$和区域$T$。

14. Sometimes you are just given a surface which is implicitly defined, like a sphere defined by $x^2 + y^2 + z^2=1$.
    有时候你只是给定了一个隐式定义的表面，比如由$x^2 + y^2 + z^2=1$定义的球体。

15. In that case you need to find a function which parameterizes this surface, as well as which specific region of the parameter space corresponds to the surface.
   在这种情况下，你需要找到一个参数化这个表面的函数，以及参数空间的哪个特定区域对应于这个表面。

--- pic\Surface area integrals.pdf_16.png ---

1. The key when going through all of this is to stay organized, and be patient.
   进行所有这些时的关键是要保持有序，并且要有耐心。

2. One way to think about it is that setting up and computing just one of these surface area integrals is akin to doing 10 practice problems in single-variable calculus.
   一种思考方式是，设置并计算这些表面积分的其中一个，就像在单变量微积分中做10个练习问题。

3. The thought process that goes into all of this is actually very useful for thinking about surfaces and three-dimensional geometry in general, beyond the specific case of computing surface area.
   投入到所有这些中的思考过程实际上对于考虑表面和三维几何图形非常有用，超出了计算表面积的特定情况。

4. For example, how do you think computer graphics works?
   例如，你认为计算机图形是如何工作的？

5. Quite often, displaying a three-dimensional figure involves subdividing a surface into polygons, and getting the computer to display those polygons.
   通常，显示三维图形涉及将表面细分为多边形，并让计算机显示这些多边形。

6. Even if this never involves performing a surface area integral, per se, the reasoning associated with how to do this is remarkably similar, using cross products of partial derivatives, etc.
   即使这本身从未涉及到执行表面积积分，但与此相关的推理如何执行此操作却非常相似，使用偏导数的叉积等。

7. If you do choose to work through it, prepare to mark up a lot of paper.
   如果你选择通过它，准备好在很多纸上做标记。