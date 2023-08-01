
--- pic\Formal definition of curl in two dimensions.pdf_00.png ---

1. Formal definition of curl in two dimensions.
   二维中旋度的正式定义。

2. Learn how curl is really defined, which involves mathematically capturing the intuition of fluid rotation.
   学习如何真正定义旋度，这涉及到数学地捕捉流体旋转的直观感觉。

3. This is good preparation for Green's theorem.
   这是对格林定理的良好准备。

1. Background
   背景

2. Curl in two dimensions
   二维的旋度

3. Line integrals in a vector field
   向量场中的线积分

1. If you haven't already, you may also want to read "Why care about the formal definitions of divergence and curl" for motivation.
   如果你还没有阅读过，你可能也想阅读"为什么要关心散度和旋度的正式定义"以获取动力。

4. What we're building to
   我们正在构建的内容


5. In two dimensions, curl is formally defined as the following limit of a line integral: 
   在二维中，旋度被正式定义为线积分的以下极限：   

6. $F$ is a two-dimensional vector field.
   $F$是一个二维向量场。

5. $(x, y)$ is some specific point in the plane.
   $(x, y)$ 是平面上的某个特定点。
7. $A_{(x,y)}$ For instance, it could be a circle centered at $(x, y)$.
   $A_{(x,y)}$ 例如，它可以是以$(x, y)$为中心的圆。

8. $|A_{(x,y)}|$ indicates the area of $A_{(x,y)}$.
   $|A_{(x,y)}|$ 表示 $A_{(x,y)}$的面积。

9. A $\lim_{|A_{(x,y)}| }\to 0$ indicates we are considering the limit as the area of $A_{(x,y)}$ goes to zero, meaning the region is shrinking to the point $(x, y)$.
   一个 $\lim_{|A_{(x,y)}| }\to 0$ 表示我们正在考虑$A_{(x,y)}$的面积趋近于零的极限，意味着区域正在缩小到点$(x, y)$。

6. $C$ is the boundary of $A_{(x,y)}$, oriented counterclockwise.
   $C$ 是 $A_{(x,y)}$ 的边界，方向为逆时针。

7. $\oint_C$ is the line integral around $C$, written as $\oint$ instead of $\int$ to emphasize that $C$ is a closed curve.
   $\oint_C$ 是围绕 $C$ 的线积分，写作 $\oint$ 而不是 $\int$，以强调 $C$ 是一个闭合的曲线。

--- pic\Formal definition of curl in two dimensions.pdf_01.png ---

1. The line integral $\oint F \cdot dr$ can be thought of as measuring the total fluid rotation around $C$.
   线积分$\oint F \cdot dr$可以被视为测量环绕$C$的总流体旋转。

2. This is complicated, but it will make sense as we build up to it one piece at a time.
   这很复杂，但随着我们一步一步地建立起来，它将变得有意义。

3. Formalizing fluid rotation.
   形式化流体旋转。

4. Suppose you have a flowing fluid whose velocity is given by a vector field $F(x, y)$, such as the one we looked at in the two-dimensional curl article.
   假设你有一个流动的流体，其速度由矢量场$F(x, y)$给出，比如我们在二维旋度文章中看到的那个。

5. Fluid flow with four points of cur interest.
   具有四个关注点的流体流动。

6. If you didn't already know about curl, but you did just learn about line integrals through a vector field, how would you measure fluid rotation in a region?
   如果你还不了解旋度，但你刚刚学习了通过矢量场的线积分，你将如何测量一个区域的流体旋转？

1. To take a relatively simple example, consider the vector field $F(x,y)$.
   举一个相对简单的例子，考虑向量场 $F(x,y)$。

2. This is the quintessential counterclockwise rotation vector field.
   这是典型的逆时针旋转向量场。

--- pic\Formal definition of curl in two dimensions.pdf_02.png ---

1. How can we make the idea of fluid rotation mathematical (before knowing about curl)? 
   我们如何使流体旋转的概念数学化（在知道旋度之前）？

2. One way to do this is to imagine walking around the perimeter of some region, like a unit circle centered at the origin, and measuring if the fluid seems to flow with you or against you at each point.
   做到这一点的一种方法是想象自己走在某个区域的边缘，比如以原点为中心的单位圆，然后在每个点测量流体是否似乎与你同向或逆向流动。

3. Concept check: Let $C$ represent the circumference of a unit circle centered at the origin, oriented counterclockwise.
   概念检查：让$C$代表以原点为中心，逆时针方向的单位圆的周长。

4. Given the picture of the vector field $F$ above, consider the following line integral: $\oint_C \mathbf{F} \cdot d\mathbf{r}$.
   给出上述向量场$F$的图片，考虑以下线积分：$\oint_C \mathbf{F} \cdot d\mathbf{r}$。

5. Without calculating it, what is the sign of this integral?
   不计算它，这个积分的符号是什么？

6. Recall that the symbol $\oint$ just emphasizes the fact that the line integral is being done over a closed loop, but it's computed the same way as any other line integral.
   请记住，符号$\oint$只是强调线积分是在封闭环上进行的事实，但其计算方式与任何其他线积分相同。

7. Choose 1 answer: 
   选择一个答案：

8. Positive.
正数。

9. As you walk around the circle, the arrows of the vector field, $F$, always point in the same direction as your motion, $d\mathbf{r}$.
当你走在圆周上时，向量场$F$的箭头始终指向与你的运动$d\mathbf{r}$相同的方向。

9. Therefore the dot product $F \cdot d\mathbf{r}$ will always be positive, and hence the integral as a whole must be positive.
   因此，点积$F \cdot d\mathbf{r}$总是正的，因此积分整体必须是正的。

1. More generally, if a fluid tends to flow counterclockwise around a region, you would expect that the line integral of that fluid's velocity vector field around the perimeter of the region would be positive (when it's oriented counterclockwise).
   更一般地，如果一个流体倾向于逆时针方向绕一个区域流动，你会期望该流体的速度矢量场在该区域的周边的线积分是正的（当它是逆时针方向的时候）。

--- pic\Formal definition of curl in two dimensions.pdf_03.png ---

1. You could also imagine a more complicated vector field, in which the fluid flows with you at some points on your counterclockwise walk around the circle, but against you at others.
   你也可以想象一个更复杂的矢量场，其中流体在你逆时针走动圆时的某些点处与你一起流动，而在其他点处却反向流动。

2. The value $F \cdot dr$ will be positive while the flow is with you, and negative when it's against you.
   当流动与你同方向时，$F \cdot dr$ 的值将为正，而当它与你反向时，$F \cdot dr$ 的值将为负。

3. In a way, the integral $\oint_C F \cdot dr$ is like a voting system that counts up how much these different directions cancel each other out and which one wins overall.
   从某种程度上说，积分$\oint_C F \cdot dr$就像一个计票系统，计算出这些不同方向互相抵消的程度和哪个方向最终占优。

4. Letting the size of the region change
   改变区域的大小

1. So, after mathematically expressing the idea of fluid rotation around a region, you might want to capture the more elusive idea of fluid rotation at a point.
因此，在数学表达了流体围绕区域旋转的概念后，你可能希望捕捉到流体在点处旋转的更难以捉摸的概念。

5. How might you go about that?
你可能如何进行呢？

1. You could start by considering smaller and smaller regions around that point, such as circles of smaller and smaller radii, and seeing what the fluid flow around those regions looks like.
你可以开始考虑该点周围越来越小的区域，例如半径越来越小的圆，看看这些区域周围的流体流动看起来如何。


1. Concept check: Back to our vector field $F=\begin{bmatrix} -y \\ x \end{bmatrix}$, rather than just looking at the unit circle, let $C_R$ represent a circle centered at the origin with radius $R$.
   概念检查：回到我们的向量场 $F=\begin{bmatrix} -y \\ x \end{bmatrix}$，我们不仅仅看单位圆，让 $C_R$ 表示一个以原点为中心，半径为 $R$ 的圆。

2. This circle will still be oriented counterclockwise.
   这个圆仍然是逆时针方向。

1. Compute the line integral of $F$ around this circle as a function of $R$.
   计算$F$在此圆周围的线积分作为$R$的函数。

--- pic\Formal definition of curl in two dimensions.pdf_04.png ---

1. First we need to parameterize this circle.
   首先，我们需要对这个圆进行参数化。

2. We can do this with the function $r(t)$.
   我们可以用函数$r(t)$来实现这一点。

3. For this parameterization to cover the circle exactly once, let $t$ range from 0 to $2\pi$.
   为了让这种参数化恰好覆盖一次圆，让$t$的范围从0到$2\pi$。

4. With this, we expand the line integral as follows: 
   有了这个，我们将线积分扩展如下：

5. Now plug the components of $r(t)$ into the definition of $F(x, y)$.
   现在将$r(t)$的组件插入$F(x, y)$的定义中。

6. Also, take the derivative of $r(t)$.
   同时，求$r(t)$的导数。


7. The fact that $F(r(t)) = r'(t)$ in this case is a coincidence, peculiar to this example.
   在这种情况下，$F(r(t)) = r'(t)$这一事实是一个巧合，特殊于这个例子。

8.  It makes the completion of the line integral pretty smooth, though.
    尽管如此，它使得线积分的完成变得非常平滑。


--- pic\Formal definition of curl in two dimensions.pdf_05.png ---

1. How does this value relate to the circle $C_R$?
   这个值如何与圆$C_R$相关？

2. It is twice the area enclosed by the circle $C_R$. 
   这是圆$C_R$所围成的面积的两倍。

3. Average rotation per unit area
   每单位面积的平均旋转量

4. The answer to this last question suggests something interesting.
   这最后一个问题的答案暗示了一些有趣的事情。

5. The rotation around a region seems to be proportional to the area of that region.
   一个区域周围的旋转似乎与该区域的面积成正比。

6. Of course, you've only shown this for circles centered at the origin, not all possible regions, but it is nevertheless suggestive.
当然，你只是为以原点为中心的圆圈展示了这一点，并非所有可能的区域，但它仍然富有启发性。

1. This might give you an idea.
这可能会给你一些想法。

1. Key idea: Maybe if you take $\oint F \cdot dr$, which measures the fluid flow around a region, and divide it by the area of that region, it can give you some notion of the average rotation per unit area. 
   关键想法：也许如果你取$\oint F \cdot dr$，它测量的是一个区域周围的流体流动，并将其除以该区域的面积，它可以给你一些关于每单位面积的平均旋转量的概念。

2. The idea of "average rotation per unit area" might feel a bit strange, but if you think back to the interpretation of curl, that's kind of what we want curl to represent. 
   “每单位面积的平均旋转量”的想法可能感到有点奇怪，但如果你回想一下旋度的解释，这正是我们希望旋度代表的。

3. Rather than thinking about fluid rotation in a large region, curl is supposed to measure how fluid tends to rotate near a point. 
   旋度应该测量流体在一个点附近的旋转倾向，而不是在大区域内思考流体旋转。

4. Concept check: The vector field from the previous example is a little bit special in that the "rotation-per-unit-area" of circles around the origin is the same value for all circles. 
   概念检查：上一个例子中的向量场有点特别，因为围绕原点的圆的“每单位面积的旋转量”对所有圆来说都是相同的值。

5. What is that value?
那个值是多少？

--- pic\Formal definition of curl in two dimensions.pdf_06.png ---

2. When I say "rotation-per-unit-area", what I mean by "rotation" is the value of the integral $\oint F \cdot dr$.
   当我说"单位面积的旋转"时，我所说的"旋转"是积分 $\oint F \cdot dr$ 的值。

2. This is because this integral indicates how much the fluid is flowing counterclockwise around the curve $C$.
   这是因为这个积分指示了流体在曲线$C$周围逆时针流动的量。

3. The "unit area" in question is the area enclosed by $C$.
   所讨论的“单位面积”是由$C$围起的面积。

4. We found in the previous question that, for our example, the integral equals $2\pi R^2$.
   我们在上一个问题中发现，对于我们的例子，积分等于$2\pi R^2$。

5. Since the area of the circle is $\pi R^2$.
   由于圆的面积是$\pi R^2$。

6. Concept check: Recall that the formula for $2d-{curl}$ is 
   概念检查：回忆一下，$2d-{curl}$的公式是

7. Where $F_1$, and $F_2$ are the components of $F$. 
   其中$F_1$和$F_2$是$F$的组成部分。

8. Given the definition $F ( x , y )$, compute the curl of $F$.
   给定定义 $F ( x , y )$，计算 $F$ 的旋转。

--- pic\Formal definition of curl in two dimensions.pdf_07.png ---

1. Applying the formula, plug in the following values: 
   应用公式，插入以下值：

2. Here's what we get: 
   这是我们得到的结果：

3. I should point out that the fact that $2d-{curl}$ $F$ is constant in this example and the fact that the average rotation per unit area was constant for all circles are both peculiar to this example.
   我应该指出，这个例子中$2d-{curl}$ $F$是常数，以及单位面积的平均旋转对所有圆都是常数的事实，都是特定于这个例子的。

4. In general, the curl varies from point to point, and the average rotation per unit area depends on the size of the area.
   通常来说，旋度从点到点是变化的，单位面积的平均旋转取决于面积的大小。

5. Defining two-dimensional curl
   定义二维旋度

6. Those last two questions show that the "average rotation per unit area” in circles centered at the origin happens to be the same as the curl of the function, at least for our specific example.
   最后两个问题显示，以原点为中心的圆中的“单位面积的平均旋转”恰好与函数的旋度相同，至少对于我们的特定示例来说。

7. This turns out to apply more broadly.
   这更广泛地适用。

1. In fact, the way we define the curl of a vector field $F$ at a point $(x, y)$ is to be the limit of this average rotation per unit area in smaller and smaller regions around the point $(x, y)$.
   实际上，我们定义向量场 $F$ 在点 $(x, y)$ 处的旋度的方式是，将这个平均旋转速度除以单位面积在点 $(x, y)$ 周围越来越小的区域的极限。

9. Specifically, (drumroll please), Here's the formula defining two-dimensional curl: 
   具体来说（请鼓掌），这是定义二维旋度的公式：

1. Average rotation per unit area
   单位面积的平均旋转量

--- pic\Formal definition of curl in two dimensions.pdf_08.png ---

6. $F$ is a two-dimensional vector field.
   $F$是一个二维向量场。

5. $(x, y)$ is some specific point in the plane.
   $(x, y)$ 是平面上的某个特定点。
7. $A_{(x,y)}$ For instance, it could be a circle centered at $(x, y)$.
   $A_{(x,y)}$ 例如，它可以是以$(x, y)$为中心的圆。

8. $|A_{(x,y)}|$ indicates the area of $A_{(x,y)}$.
   $|A_{(x,y)}|$ 表示 $A_{(x,y)}$的面积。

9. A $\lim_{|A_{(x,y)}| }\to 0$ indicates we are considering the limit as the area of $A_{(x,y)}$ goes to zero, meaning the region is shrinking to the point $(x, y)$.
   一个 $\lim_{|A_{(x,y)}| }\to 0$ 表示我们正在考虑$A_{(x,y)}$的面积趋近于零的极限，意味着区域正在缩小到点$(x, y)$。

6. $C$ is the boundary of $A_{(x,y)}$, oriented counterclockwise.
   $C$ 是 $A_{(x,y)}$ 的边界，方向为逆时针。

7. $\oint_C$ is the line integral around $C$, written as $\oint$ instead of $\int$ to emphasize that $C$ is a closed curve.
   $\oint_C$ 是围绕 $C$ 的线积分，写作 $\oint$ 而不是 $\int$，以强调 $C$ 是一个闭合的曲线。

1. This formula is impractical for computation, but the connection between this and fluid rotation is very clear once you wrap your mind around it.
   这个公式对于计算来说并不实用，但是一旦你理解了它，这个公式与流体旋转之间的联系就非常清楚了。

2. It is a very beautiful fact that this definition gives the same thing as the formula used to compute two-dimensional curl.
   这是一个非常美妙的事实，即这个定义给出的结果与用来计算二维旋度的公式是一样的。

5. One more feature of conservative vector fields.
   保守矢量场的另一个特点。

6. Background: Conservative vector fields.
   背景：保守向量场。

7. If $F(x, y)$ is a conservative vector field, all line integrals over closed loops are $0$.
   如果$F(x, y)$是一个保守向量场，所有关于闭环的线积分都是$0$。

8. Looking at the integral above, what does this imply?
   观察上面的积分，这意味着什么？

1. Choose 1 answer: 
选择1个答案：

9.  Two-dimensional curl is always $0$.
    二维旋度总是$0$。

--- pic\Formal definition of curl in two dimensions.pdf_09.png ---

1. The expression $\oint_C F \cdot dr$ is always 0, so the definition of two-dimensional curl reads.
   表达式$\oint_C F \cdot dr$总是0，所以二维旋度的定义如下。

1. Line integral
   线积分

2. Hence, the 2d-curl of a conservative vector field is always zero.
   因此，保守矢量场的2d旋度总是零。

3. This gives an important fact: If a vector field is conservative, it is irrotational, meaning the curl is zero everywhere.
   这给出了一个重要的事实：如果一个矢量场是保守的，那么它是无旋的，意味着旋度在任何地方都是零。

4. In particular, since gradient fields are always conservative, the curl of the gradient is always zero.
   特别地，由于梯度场总是保守的，梯度的旋度总是零。

3. That is a fact you could find just by chugging through the formulas.
   这是一个你可以通过公式推导得出的事实。

4. However, I think it gives much more insight to understand it using the definition of curl together with the intuition for why gradient fields are conservative.
   然而，我认为使用旋度的定义和对梯度场为什么是保守的直觉来理解它，会有更多的启示。

6. What about the converse? If a vector field has zero curl everywhere, does that mean it must be conservative?
   那么反过来呢？如果一个矢量场在任何地方的旋度都是零，那么是否意味着它必须是保守的？

7. It does, but unfortunately, you must wait until learning about Green's theorem to see why.
   是的，但不幸的是，你必须等到学习了格林定理才能理解原因。

1. Summary
   总结

2.  If a vector field represents fluid flow, you can quantify "fluid rotation in a region" by taking the line integral of that vector field along the border of that region.
    如果一个矢量场代表流体流动，你可以通过沿着该区域的边界对该矢量场进行线积分来量化"区域内的流体旋转"。

--- pic\Formal definition of curl in two dimensions.pdf_10.png ---

1. To go from the idea of fluid rotation in a region to fluid flow around a point (which is what curl measures), we introduce the idea of "average rotation per unit area" in a region.
   为了从区域内的流体旋转的概念转到围绕点的流体流动（这就是旋度衡量的），我们引入了“区域内单位面积的平均旋转”的概念。

2. Then consider what this value approaches as your region shrinks around a point.
   然后考虑当你的区域围绕一个点收缩时，这个值会接近什么。

3. In formulas, this gives us the definition of two-dimensional curl as follows: 
   在公式中，这给我们提供了二维旋度的定义如下：

4. Average rotation per unit area
   单位面积的平均旋转

5. This relationship between curl and closed-loop line integrals implies that irrotational fields and conservative fields are one and the same.
   旋度和闭环线积分之间的这种关系表明，无旋场和保守场是一样的。