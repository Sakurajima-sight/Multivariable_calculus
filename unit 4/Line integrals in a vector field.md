
--- pic\Line integrals in a vector field.pdf_00.png ---

1. Line integrals in a vector field
矢量场中的线积分

1. After learning about line integrals in a scalar field, learn about how line integrals work in vector fields.
在学习了标量场中的线积分之后，了解线积分在矢量场中是如何工作的。

1. Background
背景

1. Line integrals in scalar fields
标量场中的线积分

1. Vector fields
矢量场

1. Interpreting the derivative of a vector-valued function
解释矢量值函数的导数

1. What we are building to
我们正在构建什么

1. This animation will be described in more detail below.
这个动画将在下面详细描述。

1. Let's say there is some vector field $F$ and a curve $C$ wandering through that vector field.
假设有一个矢量场 $F$ 和一条曲线 $C$ 穿过这个矢量场。

1.  Imagine walking along the curve, and at each step taking the dot product between the following two vectors:
想象沿着曲线走，每走一步都取以下两个向量的点积：

1.  The vector from the field $F$ at the point where you are standing. 
你站立的点处的场 $F$ 的向量。

1. The displacement vector associated with the next step you take along this curve.
与你沿这条曲线走的下一步关联的位移向量。

1. If you add up those dot products, you have just approximated the line integral of $F$ along $C$.
如果你把这些点积加起来，你就近似地计算了$F$沿$C$的线积分。

--- pic\Line integrals in a vector field.pdf_01.png ---

1. The shorthand notation for this line integral is $\int_C F \cdot dr$.
这个线积分的简写表示法是 $\int_C F \cdot dr$。

13. (Pay special attention to the fact that this is a dot product)
（特别注意这是一个点积）

14. The more explicit notation, given a parameterization $r(t)$ of $C$, is $\int_a^b F(r(t)) \cdot r'(t) dt$.
给定 $C$ 的参数化 $r(t)$，更明确的表示法是 $\int_a^b F(r(t)) \cdot r'(t) dt$。

15. Line integrals are useful in physics for computing the work done by a force on a moving object.
线积分在物理中很有用，可以用来计算力对移动物体做的功。

1. If you parameterize the curve such that you move in the opposite direction as $t$ increases, the value of the line integral is multiplied by $-1$.
如果你参数化曲线，使得当 $t$ 增加时你在相反的方向移动，那么线积分的值就会乘以 $-1$。

2. Whale falling from the sky
从天空中掉下的鲸鱼

16. Let's say we have a whale, whom I'll name Whilly, falling from the sky.
假设我们有一只名叫 Whilly 的鲸鱼从天空中坠落。

17. Suppose he falls along a curved path, perhaps because the air currents push him this way and that.
假设他沿着一条曲线路径坠落，可能是因为空气流将他推向这个方向和那个方向。

18. In this example, I am assuming you are familiar with the idea from physics that a force does work on a moving object, and that work is defined as the dot product between the force vector and the displacement vector.
在这个例子中，我假设你已经熟悉了物理中的这个概念：力对一个移动的物体做功，这个功定义为力向量和位移向量的点积。

--- pic\Line integrals in a vector field.pdf_02.png ---

1. When there is a force, such as gravity, and an object moving in the region where the force acts, the force is said to "do work" on the object.
当存在一个力，如重力，并且有一个物体在这个力作用的区域内移动时，这个力被认为对物体“做功”。

20. For example, suppose Whilly falls straight down 100m from the sky (over some specified period of time):
例如，假设 Whilly 从天空直接下降100米（在某个指定的时间段内）：

21. The force of gravity on this whale is $F = mg$.
重力在这只鲸鱼身上的力是 $F = mg$。

22. And the work that gravity does on Whilly is the force times displacement: $W = F \cdot s$.
重力对 Whilly 做的功是力乘以位移：$W = F \cdot s$。

23. Actually, this formula is not quite right. Suppose Whilly does not move straight down.
实际上，这个公式不完全正确。假设 Whilly 并不是直接向下移动。

1. Perhaps instead his displacement vector is down and to the right, with a $y$-component of $-60m$, and an $x$-component of $80m$:
也许他的位移向量是向下和向右的，$y$分量为$-60m$，$x$分量为$80m$：

--- pic\Line integrals in a vector field.pdf_03.png ---

1. Gravity still does work on Whilly, but all that matters is the component of the Whilly's displacement vector in the direction of gravity.
   重力仍然对Whilly产生作用，但重要的是Whilly的位移向量在重力方向上的分量。

2. In other words, work is the dot product between the force vector and the displacement vector. 
   换句话说，工作是力向量和位移向量之间的点积。

3. In this case, since gravity points purely in the $-j$ direction, performing the dot product ends up being the same as pulling out the vertical component from the displacement vector.
   在这种情况下，由于重力纯粹指向$-j$方向，执行点积最终等同于从位移向量中提取垂直分量。

4. Key question: What is the work done on Whilly by gravity as he falls along the curved path $C$?   
   关键问题：当Whilly沿曲线路径$C$下落时，重力对他做了多少工作？

5. Usually, computing work is done with respect to a straight force vector and a straight displacement vector, so what can we do with this curved path?
   通常，计算工作是相对于直力向量和直位移向量完成的，那么我们能用这个曲线路径做什么？

1. You can start by imagining the curve is broken up into many little displacement vectors:
你可以开始想象曲线被分解成许多小的位移向量：

--- pic\Line integrals in a vector field.pdf_04.png ---

1. Go ahead and give each one of these displacement vectors a name, 
   继续为这些位移向量命名，

2. The work done by gravity along each one of these displacement vectors is the gravity force vector, which I'll denote $F_g$, dotted with the displacement vector itself.
   沿着这些位移向量，重力所做的工作是重力力矢量，我将表示为$F_g$，与位移矢量本身的点积。

1. The total work done by gravity along the entire curve is then estimated by
沿整个曲线，重力做的总功被估计为

3. But of course, this is calculus, so we don't just look at a specific number of finite steps along the curve $C$.
   当然，这是微积分，所以我们不仅仅看曲线$C$上的有限步数。

4. We consider what limiting value this sum approaches as the size of those steps shrinks smaller and smaller. This is captured with the following integral.
   我们考虑当这些步骤的大小逐渐缩小时，这个和会趋近于什么极限值。这通过下面的积分表达。

5.  This is very similar to line integration in a scalar field, but there is the key difference: The tiny step $ds$ is now thought of as a vector, not a scalar length. 
    这与标量场中的线积分非常相似，但有一个关键区别：微小步长$ds$现在被认为是一个向量，而不是标量长度。

6.  In the integral above, I wrote both $F$ and $ds$ with little arrows on top to emphasize that they are vectors.
    在上述积分中，我在$F$和$ds$上都加了小箭头以强调它们是向量。

2. A more subtle and more common way to emphasize that these are vector quantities is to write the variable in bold:
一种更微妙且更常见的强调这些是矢量量的方式是将变量写成粗体：

--- \text\pic\Line integrals in a vector field.pdf\05.png ---

1. Key takeaway: The thing we're adding up as we wander along $C$ is not the full value of $F_g$ at each point, but the component of $F_g$ pointed in the same direction as the vector $ds$.   
    关键点：我们在沿$C$路径时所加的不是每一点的$F_g$的全值，而是$F_g$的分量，其指向与向量$ds$相同的方向。

13. That is, the component of force in the direction of the curve. 
    也就是说，是沿曲线方向的力的分量。

14. Example 1: Putting numbers on Whilly's fall. 
    例1：为Whilly的下落插入数字。

1. Let's see how this plays out when we go through the computation. 
当我们进行计算时，让我们看看这是如何发挥作用的。

1. Suppose the curve of Whilly's fall is described by the parametric function
假设Whilly的下落曲线由参数函数描述

15. The vector $ds$ representing a tiny step along the curve can be given as the derivative of this function, times $dt$: $ds= \frac{ds}{dt} dt=s'(t)dt$.
   表示沿曲线的微小步长的向量$ds$可以表示为该函数的导数乘以$dt$: $ds=\frac{ds}{dt} dt=s'(t)dt$.

16. If these seem unfamiliar, consider taking a look at the article describing derivatives of parametric functions. 
    如果这些看起来不熟悉，考虑看看描述参数函数导数的文章。

17. The way to visualize this is to think of a tiny increase to the parameter $t$ of size $dt$.
    可视化这一点的方法是考虑参数$t$的微小增加，大小为$dt$。

1.  This results in a tiny nudge along the curve described by $s(t)$, which is given by the vector $s'(t)dt$.
这导致沿着由$s(t)$描述的曲线微微移动，这由向量$s'(t)dt$给出。

1. Evaluating this derivative vector simply requires taking the derivative of each component:
评估这个导数向量只需要求每个分量的导数：

--- \text\pic\Line integrals in a vector field.pdf\06.png ---

1. The force of gravity is given by the acceleration $9.8 \, \text{m/s}^2$, multiplied by the mass of Whilly. 
    重力是由加速度$9.8 \, \text{m/s}^2$乘以Whilly的质量给出的。

19. Not that it matters, but I looked up the typical mass of a blue whale, and it's around 170,000 kg, so let's use that number. 
    虽然这并不重要，但我查了一下蓝鲸的典型质量，大约是170,000公斤，所以我们就用这个数字。

20. Since this force is directed purely downward, gravity as a force vector looks like this: 
    由于这个力完全向下，所以重力作为一个力向量看起来是这样的：

21. Let's say we want to find the work done by gravity between times $t = 0$ and $t = 10$. 
    假设我们想找到在$t = 0$和$t = 10$之间由重力做的工作。

22. What do you get when you plug in all this information to the integral $\int_C F \cdot ds$ and evaluate the integral? 
    当你将所有这些信息插入积分$\int_C F \cdot ds$并计算积分时，你会得到什么？

23. Take a moment to try writing this out for yourself before peeking at the answer. 
    在偷看答案之前，花点时间自己试着写出来。

--- \text\pic\Line integrals in a vector field.pdf\07.png ---
1. To those physics students among you who notice that it would be easier to just compute the gravitational potential of Whilly at the start and end of his fall and find the difference, you are going to love the topic of conservative fields!
   对于你们中间的物理学生，如果你注意到只需要计算Whilly跌落开始和结束时的重力势能并找出差值更为简单，你一定会喜欢保守场的主题！

2. Visualizing more general line integrals through a vector field
   通过向量场来可视化更一般的线积分

3. In the previous example, the gravity vector field is constant. Gravity points straight down with the same magnitude everywhere.
   在前一个例子中，重力矢量场是常数。重力在每个地方都直接向下指，大小相同。

4. With most line integrals through a vector field, the vectors in the field are different at different points In space, so the value dotted against $ds$ changes.
   对于通过向量场的大部分线积分，场中的矢量在空间的不同点处是不同的，所以与$ds$点乘的值会改变。

5. The following animation shows what this might look like.
   下面的动画展示了这可能看起来是什么样的。

6. Note, the animation uses the variable $r$ instead of $s$ to parameterize the curve, but of course, it does not make a difference.
   注意，动画使用变量$r$而不是$s$来参数化曲线，但当然，这并没有区别。

7. Let's dissect what's going on here.
   让我们解析一下这里发生了什么。

1. The line integral itself is written as
线积分本身可以写成

--- pic\Line integrals in a vector field.pdf_08.png ---

1. $\int F(r) \cdot dr = \int F(r(t)) \cdot r'(t)dt$
   $\int F(r) \cdot dr = \int F(r(t)) \cdot r'(t)dt$

1. where $F$ is a vector field, associating each point in space with a vector.
   其中 $F$ 是一个向量场，将空间中的每个点与一个向量关联起来。

2. You can think of this as a force field.
   你可以将这看作是一个力场。

3. $C$ is a curve through space.
   $C$ 是穿过空间的一条曲线。

1. $r(t)$ is a vector-valued function parameterizing the curve $C$ in the range $a \leq t \leq b$.
$r(t)$ 是一个向量值函数，它在范围 $a \leq t \leq b$ 内参数化曲线 $C$。


4. $r'(t)$ is the derivative of $r$, representing the velocity vector of a particle whose position is given by $r(t)$ while $t$ increases at a constant rate.
   $r'(t)$ 是 $r$ 的导数，表示粒子的速度向量，该粒子的位置由 $r(t)$ 给出，而 $t$ 以恒定的速率增加。

5. When you multiply this by a tiny step in time, $dt$, it gives a tiny displacement vector, which I like to think of as a tiny step along the curve.
   当你将其与微小的时间步长 $dt$ 相乘时，它会产生一个微小的位移向量，我倾向于将其视为曲线上的微小步长。

6. Technically, it is a tiny step in the tangent direction to the curve, but for small enough $dt$ this amounts to the same thing.
   从技术上讲，它是曲线切线方向上的微小步长，但对于足够小的 $dt$，这可以视为同一件事。

7. Note, in this animation the length of $(t)$ stays constant.
   注意，在这个动画中，$(t)$ 的长度保持恒定。

8. This is not necessarily true for most parameterizations of $C$, which may have you speeding up or slowing down as your position varies according to $r$.
   这对于大多数参数化的$C$并不一定成立，因为当你的位置根据$r$变化时，你可能会加速或减速。

9. For example, Whilly was probably speeding up during his fall, making the velocity vector grow over time.
   例如，Whilly在下落过程中可能在加速，使得速度向量随着时间的推移而增长。

10. The rotating circle in the bottom right of the diagram is a bit confusing at first.
   图表右下角的旋转圆圈一开始可能有点让人困惑。

1. It represents the extent to which the vector $F(\mathbf{r}(t))$ lines up with the tangent vector $\mathbf{r}'(t)$.
它表示向量 $F(\mathbf{r}(t))$ 与切向量 $\mathbf{r}'(t)$ 对齐的程度。

12. The grey $x$ and $y$ vectors are shown to see how these vectors are oriented relative to $xy$-plane as a whole.
   灰色的$x$和$y$向量显示了这些向量相对于整个$xy$平面的方向。

13. Concept check : What does the dot product $F(\mathbf{r}(t)) \cdot \mathbf{r}'(t) dt$ represent?
概念检查：点积 $F(\mathbf{r}(t)) \cdot \mathbf{r}'(t) dt$ 代表什么？

1. The component of $F(\mathbf{r}(t))$ pointing in the same direction as a tiny step along the curve at the point $\mathbf{r}(t)$, multiplied by the size of that tiny step.
$F(\mathbf{r}(t))$ 在点 $\mathbf{r}(t)$ 处沿曲线方向的微小步长的分量，乘以该微小步长的大小。

1. The dot product of any two vectors $w \cdot v$ gives the component of $w$ pointing in the same direction as $v$ multiplied by the magnitude of $v$.
任意两个向量的点积 $w \cdot v$ 给出了 $w$ 在与 $v$ 同方向的分量，乘以 $v$ 的大小。

--- pic\Line integrals in a vector field.pdf_09.png ---

1. In this case, $r'(t)dt$ represents a tiny step along the curve.
   在这种情况下，$r'(t)dt$ 代表沿曲线的微小步长。

2. In physics terms, you can think about this dot product $F(r(t)) \cdot r'(t)dt$ as $dW$
   用物理术语来说，你可以把这个点积 $F(r(t)) \cdot r'(t)dt$ 看作是 $dW$

3. That is, a tiny amount of work done by the force field $F$ on a particle moving along $C$.
   也就是说，由力场 $F$ 对沿 $C$ 运动的粒子所做的微小量的功。

4. Example 2: Work done by a tornado
   示例2：龙卷风做的功

5. Consider the vector field described by the function
   考虑由函数描述的向量场

1. The vector field looks like this:
向量场看起来像这样：

--- pic\Line integrals in a vector field.pdf_10.png ---

1. Thought of as a force, this vector field pushes objects in the counterclockwise direction about the origin.
   从力的角度来看，这个向量场在原点周围逆时针方向推动物体。

2. For example, maybe this represents the force due to air resistance inside a tornado.
   例如，这可能代表着龙卷风内部由于空气阻力产生的力。

3. This is a little unrealistic because it would imply that force continually gets stronger as you move away from the tornado's center, but we can just euphemistically say it's a "simplified model" and continue on our merry way.
   这有点不现实，因为它暗示着当你离龙卷风的中心远离时，力会持续变强，但我们可以委婉地说它是一个"简化模型"，然后继续我们的愉快旅程。

4. Suppose we want to compute a line integral through this vector field along a circle of radius 1 centered at $(2,0)$.
   假设我们想要计算一个线积分，这个线积分穿过这个向量场，沿着一个半径为1、中心在$(2,0)$的圆进行。

5. I should point out that orientation matters here.
   我应该指出方向在这里是重要的。

6. The work done by the tornado force field as we walk counterclockwise around the circle could be different from the work done as we walk clockwise around it.
   当我们逆时针走过这个圆时，龙卷风力场所做的功可能与我们顺时针走过它时所做的功不同。

7. (We'll see this explicitly in a bit).
   （我们稍后会明确地看到这一点）。

1. If we choose to consider a counterclockwise walk around this circle, we can parameterize the curve with the function.
如果我们选择考虑逆时针绕这个圆行走，我们可以用函数参数化这个曲线。

2. $r(t)$ where $t$ is in the range from $0$ to $2\pi$.
$r(t)$，其中 $t$ 的范围从 $0$ 到 $2\pi$。

1. Again, to set up the line integral representing work, you consider the force vector at each point, $F(x, y)$, and you dot it with a tiny step along the curve, $dr$:
再次，为了建立代表工作的线积分，你考虑每一点的力向量$F(x, y)$，并与曲线上的一个微小步长$dr$点乘：

--- pic\Line integrals in a vector field.pdf_11.png ---

1. Step 1: Expand the integral.
   步骤1：扩展积分。

2. Concept check: Which of the following integrals represents the same thing as $\int F \cdot dr$? 
   概念检查：以下哪个积分代表了与 $\int F \cdot dr$ 相同的东西？

1. See the previous section.
参见前一节。

3. Step 2: Expand each component.
   步骤2：扩展每个组件。

4. Concept check: Based on the definitions above, what is $F(\mathbf{r}(t))$?
   概念检查：基于以上定义，$F(\mathbf{r}(t))$ 是什么？

1. $F(x, y)$ is defined as $F(x, y) = \begin{bmatrix} -y \\ x \end{bmatrix}$ and $r(t)$ is defined as $r(t) = \begin{bmatrix} \cos(t) + 2 \\ \sin(t) \end{bmatrix}$。
定义函数 $F(x, y) = \begin{bmatrix} -y \\ x \end{bmatrix}$，以及函数 $r(t) = \begin{bmatrix} \cos(t) + 2 \\ \sin(t) \end{bmatrix}$。

--- pic\Line integrals in a vector field.pdf_12.png ---

1. For $F(\mathbf{r}(t))$, plug in the components of $\mathbf{r}(t)$ as the inputs $x$ and $y$ of $F$: 
   对于 $F(\mathbf{r}(t))$，将 $\mathbf{r}(t)$ 的组成部分作为 $F$ 的输入 $x$ 和 $y$ 插入：

2. Concept check: What is $\mathbf{r}'(t)$? 
   概念检查：$\mathbf{r}'(t)$ 是什么？

3. Step 3: Solve the integral.
   步骤3：解积分。

4. Concept check: Put the last three answers together to solve the integral. 
   概念检查：将最后三个答案放在一起求解积分。

以下是按照您的要求翻译的句子，其中包含了使用 LaTeX 的数学公式和函数变量：

--- pic\Line integrals in a vector field.pdf_13.png ---

1. This final answer gives the amount of work that the tornado force field does on a particle moving counterclockwise around the circle pictured above.
这个最终答案给出了龙卷风力场对一个沿着上图所示的圆逆时针移动的粒子所做的工作量。

2. Reflection question: Why should it be intuitive that this answer is positive?
   反思问题：为什么这个答案是正的应该是直观的？

3. Since the circle is oriented counterclockwise, you walk up the right half, and down the left half.
   因为圆是逆时针方向的，所以你沿着右半部分向上走，然后沿着左半部分向下走。

4. The vectors touching the right half of the circle are relatively long, and that you walk, thus contributing a lot of positive work.
   触及圆右半部分的向量相对较长，并且你走过，从而贡献了大量的正功。

5. The vectors touching the left half of the circle are still pointing roughly up, which is now against the direction you are walking, and hence contribute negative work.
   触及圆的左半部分的向量仍然大致指向上方，这现在与你行走的方向相反，因此贡献了负功。

6. However, these vectors are relatively short, so they do not cancel out the positive work done while walking up the right half.
   然而，这些向量相对较短，所以它们并没有抵消在右半部分向上行走时所做的正功。

1. Orientation matters
方向很重要

--- pic\Line integrals in a vector field.pdf_14.png ---

1. What would have happened if in the preceding example, we had oriented the circle clockwise?
如果在前面的例子中，我们让圆按顺时针方向定向，会发生什么呢？

8. For instance, we could have parameterized it with the function $r(t)$.
例如，我们可以用函数$r(t)$对其进行参数化。

8. You can, if you want, plug this in and work through all the computations to see what happens.
   如果你愿意，你可以把这个插入并完成所有的计算来看看会发生什么。

9. However, there is a simpler way to reason about what will happen.
   然而，有一个更简单的方式来推理将会发生什么。

10. In the integral $\int_C F \cdot dr$, each vector $dr$ representing a tiny step along the curve will get turned around to point in the opposite direction.
   在积分$\int_C F \cdot dr$中，每个表示沿曲线微小步长的向量$dr$都会反向指向相反的方向。

9. Concept check: Suppose you have two vectors $v$ and $w$, and $v \cdot w = 3$.
概念检查：假设你有两个向量$v$和$w$，并且$v \cdot w = 3$。

10. You turn $v$ around to point in the opposite direction, getting a new vector $v_\text{new} = -v$.
你将$v$反转，使其指向相反的方向，得到一个新的向量$v_\text{new} = -v$。

11. What happens to the dot product?
点积会发生什么变化？

--- pic\Line integrals in a vector field.pdf_15.png ---

1. Since the dot product inside the integral gets multiplied by $-1$ when you swap the direction of each $dr$.
   由于在你交换每个$dr$的方向时，积分内的点积被乘以$-1$。

2. We can conclude the following: 
   我们可以得出以下结论：

1. Key Takeaway: The line integral through a vector field gets multiplied by $-1$ when you reverse the orientation of a curve.
关键点：当你反转曲线的方向时，通过向量场的线积分会被乘以$-1$。

1. Summary
   总结

2.  The shorthand notation for a line integral through a vector field is $\int_C F \cdot dr$.  
    通过向量场的线积分的简写符号是$\int_C F \cdot dr$。

3.  The more explicit notation, given a parameterization $r(t)$ of $C$, is $\int_a^b F(r(t)) \cdot r'(t) dt$.
    给定$C$的参数化$r(t)$，更明确的符号是$\int_a^b F(r(t)) \cdot r'(t) dt$。

4.  Line integrals are useful in physics for computing the work done by a force on a moving object.
    线积分在物理学中很有用，用于计算力对移动物体所做的工作。

5.  If you parameterize the curve such that you move in the opposite direction as $t$ increases, the value of the line integral is multiplied by $-1$.
    如果你将曲线参数化为随着$t$的增加而移动的反方向，那么线积分的值会被乘以$-1$。
