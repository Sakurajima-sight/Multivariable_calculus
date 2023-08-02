
--- pic\2D divergence theorem.pdf_00.png ---

1. 2D divergence theorem
   二维散度定理

2. This is the analog of Green's theorem, but for divergence instead of curl.
   这是格林定理的类比，但是用散度代替旋度。

3. Background
   背景

4. Green's theorem
   格林定理

5. Two-dimensional flux
   二维流量

6. Constructing the unit normal vector of a curve
   构造曲线的单位法向量

7. Divergence
   散度

8. Not strictly required, but helpful for a deeper understanding:
   不是严格要求，但有助于深入理解：

9. Formal definition of divergence
   散度的正式定义

10. What we're building to
    我们正在构建的是

11. The 2D divergence theorem is to divergence what Green's theorem is to curl. It relates the divergence of a vector field within a region to the flux of that vector field through the boundary of the region.
    二维散度定理之于散度就像格林定理之于旋度。它将一个区域内的矢量场的散度与该矢量场通过该区域的边界的通量联系起来。

12. Setup:
    设置：

13. $\mathbf{F}(x, y)$ is a two-dimensional vector field.
    $\mathbf{F}(x, y)$是一个二维矢量场。

14. $R$ is some region in the $x y$-plane.
    $R$是$x y$平面中的某个区域。

15. $C$ is the boundary of $R$.
    $C$是$R$的边界。

16. $\hat{\mathbf{n}}$ is a function which gives outward-facing unit normal vectors to $C$.
    $\hat{\mathbf{n}}$是一个函数，它给出了指向$C$的外向单位法向量。

17. The 2D divergence theorem says that the flux of $\mathbf{F}$ through the boundary curve $C$ is the same as the double integral of $\operatorname{div} \mathbf{F}$ over the full region $R$.
    二维散度定理说，$\mathbf{F}$通过边界曲线$C$的通量与$\operatorname{div} \mathbf{F}$在整个区域$R$上的双重积分相同。
    $$
    \underbrace{\int_C \mathbf{F} \cdot \hat{\mathbf{n}} d s}_{\text {通量积分 }}=\iint_R \operatorname{div} \mathbf{F} d A
    $$

--- pic\2D divergence theorem.pdf_01.png ---

1.  The intuition here is that if $\mathbf{F}$ represents a fluid flow, the total outward flow rate from $R$, as measured by the flux integral, equals the sum over all the little bits of outward flow at each point, as measured by divergence.
    这里的直觉是，如果$\mathbf{F}$表示流体流动，那么从$R$出来的总的外流速率，如通过通量积分所测量的，等于每个点的所有小块外流的总和，如通过散度所测量的。

2.  Often the component functions of $\mathbf{F}(x, y)$ are given as $P(x, y)$ and $Q(x, y)$ :
    通常，$\mathbf{F}(x, y)$的组成函数被给定为$P(x, y)$和$Q(x, y)$：
    $$
    \mathbf{F}(x, y)=\left[\begin{array}{l}
    P(x, y) \\
    Q(x, y)
    \end{array}\right]
    $$

3.  In this case, once you write both integrals in terms of $P$ and $Q$, the 2D divergence theorem looks like this:
    在这种情况下，一旦你用$P$和$Q$的形式写出两个积分，二维散度定理就像这样：
    $$
    \oint_C P d y-Q d x=\iint_R \frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}
    $$

4.  Written in this form, it's easier to see that the 2D divergence theorem is secretly just saying the same thing as Green's theorem.
    以这种形式写出来，更容易看出二维散度定理实际上只是在说与格林定理相同的事情。

5.  Intuition: Connecting two outward flow measures
    直觉：连接两个外向流量度量

6.  The global view: Flux
    全局视角：通量

7.  Here, I am assuming you have already learned about two-dimensional flux, and what it represents. Namely, it gives the rate at which a flowing fluid passes through a curve, such as $C$. When that curve encloses some region, such as $R$, the flux is a measure of the rate at which fluid is exiting that region.
    在这里，我假设你已经学过了二维通量，以及它代表什么。也就是说，它给出了流动的流体通过如$C$这样的曲线的速率。当该曲线围绕着某个区域，如$R$，通量就是流体退出该区域的速率的度量。

8.  Given a vector field $\mathbf{F}(x, y)$, representing the velocity vector field of the fluid, the flux of $\mathrm{F}(x, y)$ through $C$ is measured with the following integral:
    给定一个矢量场$\mathbf{F}(x, y)$，表示流体的速度矢量场，$\mathrm{F}(x, y)$通过$C$的通量用以下积分来测量：
    $$
    \underbrace{\int_C \mathbf{F} \cdot \hat{\mathbf{n}} d s}_{\text {通量积分}}
    $$

1. This integral walks over each point on the boundary $C$, and picks up the component of the vector from $\mathbf{F}$ which is in the direction of the outward facing unit normal vector $\hat{\mathbf{n}}$. The larger that value is, the faster fluid is flowing out of $R$ at that point; the more negative it is, the more fluid is flowing in at that point.
   这个积分遍历边界 $C$ 上的每一点，并获取来自 $\mathbf{F}$ 的向量的分量，该分量在朝外的单位法向量 $\hat{\mathbf{n}}$ 的方向上。该值越大，流体在该点处流出 $R$ 的速度越快；该值越负，流体在该点处流入的速度越快。

--- pic\2D divergence theorem.pdf_02.png ---

1. The local view: Divergence
   局部视图：散度

2. I am also assuming you have learned about a different measure of "outward flow" in fluid movements: Divergence. The divergence of $\mathrm{F}(x, y)$ is a function that tells you how much the fluid tends to diverge away from each point $(x, y)$.
   我也假设你已经学习了关于流体运动中"向外流动"的另一种度量：散度。$\mathrm{F}(x, y)$的散度是一个函数，它告诉你流体在每个点$(x, y)$处有多少趋向于发散。

3. The 2D divergence theorem connects these two ideas:
   二维散度定理将这两个概念联系起来：

$$\overbrace{\underbrace{\int_C \mathbf{F} \cdot \hat{\mathbf{n}} d s}_{\text {从 } R \text { 外流出 }}}^{\text {通量积分 }}=\underbrace{\iint_R \operatorname{div} \mathbf{F} d A}_{\text {所有小块的外流之和 }}$$


1. Want a deeper understanding?
   想要更深入的理解？

2. This intuition should feel very similar to the one behind Green's theorem, in which the total fluid rotation in a region equals the sum of all the little bits of rotation represented by $2 \mathrm{~d}-\mathrm{curl} \mathrm{F}$ :
   这种直觉应该与格林定理背后的直觉非常相似，在格林定理中，一个区域内的总流体旋转等于由$2 \mathrm{~d}-\mathrm{curl} \mathrm{F}$表示的所有小旋转的和：
   $$
   \underbrace{\oint_C \mathbf{F} \cdot d \mathbf{r}}_{\text {围绕 } R \text{ 的流体旋转}}=\underbrace{\iint_R 2 \mathrm{~d}-\operatorname{curl} \mathbf{F} d A}_{\text {所有小旋转的总和}}
   $$

3. However, for both Green's theorem and the 2D divergence theorem, talking about adding up little bits of rotation or outward flow is pretty vague. Although each provides a great intuition, they are not exactly rigorous math, are they?
   然而，对于格林定理和二维散度定理，谈论加起来的小旋转或向外流动是相当模糊的。虽然每一个都提供了很好的直觉，但它们并不完全是严谨的数学，对吗？

4. In the article on Green's theorem, I stepped through a more precise line of reasoning for where the double integral of curl comes into play. This involved chopping up the region $R$, and seeing how certain line integrals canceled each other out along the slices through $R$.
   在关于格林定理的文章中，我详细阐述了旋度的双重积分在何处起作用的更精确的推理过程。这涉及到将区域 $R$ 切割，并观察在通过 $R$ 的切片上，某些线积分如何相互抵消。

--- pic\2D divergence theorem.pdf_03.png ---


1.  An almost identical line of reasoning can be used to demonstrate the 2D divergence theorem. For anyone wishing to gain deeper insight, a good exercise would be to go back and walk through that same line of reasoning, but replace the line integral $\oint_C \mathbf{F} \cdot d \mathbf{r}$, which measures flow around $R$, with the flux integral $\oint_C \mathbf{F} \cdot \hat{\mathbf{n}} d s$, which measures flow out of $R$.
    几乎相同的推理过程可以用来证明二维散度定理。对于任何希望深入理解的人来说，一个好的练习是回去走一遍同样的推理过程，但是将测量$R$周围流动的线积分$\oint_C \mathbf{F} \cdot d \mathbf{r}$替换为测量$R$流出的通量积分$\oint_C \mathbf{F} \cdot \hat{\mathbf{n}} d s$。

2.  And if this deeper understanding is what you seek, I would also recommend going in armed with knowledge of the formal definition of divergence.
    如果你寻求的是更深入的理解，我也建议你带着散度的正式定义的知识去理解。

3.  Proof: Flux integrals + Unit normal vector + Green's theorem
    证明：通量积分 + 单位法向量 + 格林定理

4.  This exercise in deeper understanding is not necessary to prove the 2D divergence theorem. In fact, when you start spelling out how each integral is actually computed, you'll find that this theorem is really just saying the same thing as Green's theorem.
    这种深入理解的练习并不是证明二维散度定理的必要条件。实际上，当你开始详细说明每个积分是如何实际计算的时候，你会发现这个定理实际上只是在说和格林定理相同的事情。

5.  Start by writing out $\mathbf{F}$ in terms of the component functions $P(x, y)$ and $Q(x, y)$ :
    首先，用组成函数$P(x, y)$和$Q(x, y)$来写出$\mathbf{F}$：
    $$
    \mathbf{F}(x, y)=\left[\begin{array}{l}
    P(x, y) \\
    Q(x, y)
    \end{array}\right]
    $$

6.  Applying the formula for a unit normal vector to the flux integral, here's another way to represent that flux integral.
    将单位法向量的公式应用到通量积分，这里有另一种表示通量积分的方式。
    $$
    \int_C \mathbf{F} \cdot \hat{\mathbf{n}} d s=\int_C\left[\begin{array}{l}
    P(x, y) \\
    Q(x, y)
    \end{array}\right] \cdot \hat{\mathbf{n}} d s
    $$

7.  Next, let's write out the unit normal vector explicitly.
    接下来，让我们明确地写出单位法向量。

--- pic\2D divergence theorem.pdf_04.png ---

1. Concept check: If we think of the vector $\left[\begin{array}{l}d x \\ d y\end{array}\right]$ as representing a tiny step in the counterclockwise direction around the curve $C$, with $d s=\sqrt{d x^2+d y^2}$ as its magnitude, which of the following represents an outward facing unit normal vector?
   概念检查：如果我们认为向量$\left[\begin{array}{l}d x \\ d y\end{array}\right]$代表在曲线$C$周围逆时针方向的一个微小步骤，其中$d s=\sqrt{d x^2+d y^2}$为其大小，那么下列哪个代表一个向外的单位法向量？

   
1. (B) $\frac{1}{d s}\left[\begin{array}{c}d y \\ -d x\end{array}\right]$



--- pic\2D divergence theorem.pdf_05.png ---

1. The second answer choice is correct:
   第二个答案选项是正确的：
   $$
   \frac{1}{d s}\left[\begin{array}{c}
   d y \\
   -d x
   \end{array}\right]
   $$

2. Both the second and the third answer choices give unit normal vectors, but only the second one is outward facing. If any of the following explanation seems unclear, consider reviewing the article on constructing a unit normal vector to a curve.
   第二个和第三个答案选项都给出了单位法向量，但只有第二个是向外的。如果以下的解释有任何不清楚的地方，可以考虑复习一下关于构造曲线的单位法向量的文章。

3. When constructing a unit normal vector, you think about taking the tangent vector $\left[\begin{array}{l}d x \\ d y\end{array}\right]$ and rotating it $90^{\circ}$. In this case, since we are thinking of the tangent vector as being in the counterclockwise direction, and we want an outward-facing unit normal vector, we need to rotate this vector clockwise.
   当构造单位法向量时，你可以想象取切线向量$\left[\begin{array}{l}d x \\ d y\end{array}\right]$并旋转它$90^{\circ}$。在这种情况下，因为我们认为切线向量是逆时针方向的，而我们想要一个向外的单位法向量，所以我们需要顺时针旋转这个向量。

4. To rotate a vector by $90^{\circ}$, you swap the two components and make one of them negative. Personally, I can never remember which one to make negative for which direction of rotation, so I just try one and draw it out. For example, suppose you perform a transformation like this:
   要旋转一个向量$90^{\circ}$，你交换两个分量并使其中一个为负。我个人永远记不住哪一个应该为负以适应哪个方向的旋转，所以我只是尝试一个并画出来。例如，假设你进行了这样的变换：
   $$
   \left[\begin{array}{l}
   x \\
   y
   \end{array}\right] \rightarrow\left[\begin{array}{c}
   -y \\
   x
   \end{array}\right]
   $$

5. Drawing it out might look like this:
   画出来可能是这样的：


--- pic\2D divergence theorem.pdf_06.png ---

1. So evidently that gives a counterclockwise rotation. Since we need to go the other way for our outward facing normal vector, we negate the second coordinate:
   所以显然这给出了一个逆时针旋转。由于我们需要为我们的外向法向量走另一条路，我们否定了第二个坐标：
   $$
   \left[\begin{array}{l}
   d x \\
   d y
   \end{array}\right] \rightarrow\left[\begin{array}{c}
   d y \\
   -d x
   \end{array}\right]
   $$

2. Finally, to make this a unit vector, divide it by its magnitude:
   最后，为了使这成为一个单位向量，我们将它除以它的大小：
   $$
   \frac{1}{d s}\left[\begin{array}{c}
   d y \\
   -d x
   \end{array}\right]
   $$

3. Plugging this into our flux integral and simplifying, here's what we get:
   将这个插入我们的通量积分并简化，我们得到的是：
   $$
   \begin{aligned}
   \int_C\left[\begin{array}{l}
   P(x, y) \\
   Q(x, y)
   \end{array}\right] \cdot \hat{\mathbf{n}} d s & =\int_C\left[\begin{array}{c}
   P(x, y) \\
   Q(x, y)
   \end{array}\right] \cdot\left(\frac{1}{d s}\left[\begin{array}{c}
   d y \\
   -d x
   \end{array}\right]\right) d s \\
   & =\int_C P d y-Q d x
   \end{aligned}
   $$

4. Written in this form, we can directly apply Green's theorem.
   以这种形式写出来，我们可以直接应用格林定理。

5. Concept check: Which of the following is Green's theorem, where $C$ represents a closed curve encompassing region $R$ ?
   概念检查：以下哪一个是格林定理，其中$C$表示包围区域$R$的闭曲线？

6. Choose 1 answer:
   选择1个答案：

7. (A) $\oint_C P d x+Q d y=\iint_R\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d A$
   

--- pic\2D divergence theorem.pdf_07.png ---


1.  The first answer choice is correct:
    第一个答案选项是正确的：
    $$
    \oint_C P d x+Q d y=\iint_R\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d A
    $$

2.  Remember, the expression $\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}$ represents the two-dimensional curl of $\mathbf{F}$.
    记住，表达式$\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}$表示$\mathbf{F}$的二维旋度。

3.  If this seems unfamiliar, consider reviewing the article on Green's theorem.
    如果这看起来不熟悉，可以考虑复习一下关于格林定理的文章。

4.  Concept check: What do you get when you apply Green's theorem to the flux integral $\int_C P d y-Q d x$ ?
    概念检查：当你将格林定理应用到通量积分$\int_C P d y-Q d x$时，你会得到什么？

5.  Choose 1 answer:
    选择1个答案：

6.  (A) $\oint_C P d y-Q d x=\iint_R\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}\right) d A$
    (A) $\oint_C P d y-Q d x=\iint_R\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}\right) d A$

--- pic\2D divergence theorem.pdf_08.png ---

1. The first answer choice is correct:
   第一个答案选项是正确的：
   $$
   \oint_C P d y-Q d x=\iint_R\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}\right) d A
   $$

2. This might get confusing because both this expression and Green's theorem are using $P^{\prime}$ s and $Q^{\prime}$ 's, but the roles of each are switched. Here's how the two look lined up:
   这可能会让人感到困惑，因为这个表达式和格林定理都在使用$P^{\prime}$和$Q^{\prime}$，但是每个的角色都被交换了。以下是两者对齐的样子：
   $$
   \begin{aligned}
   & \underbrace{\oint_C P d x+Q d y=\iint_R\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d A}_{\text {格林定理 }} \\
   & \underbrace{\oint_C-Q d x+P d y=\iint_R\left(\frac{\partial P}{\partial x}-\frac{\partial(-Q)}{\partial y}\right) d A}_{\text {用 }-Q \text { 替换 } P, \text { 用 } P \text { 替换 } Q} \\
   & \underbrace{\oint_C P d y-Q d x=\iint_R\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}\right) d A}_{\text {重排后的形式，以及这个问题的答案 }}
   \end{aligned}
   $$


4. Notice, the expression inside the double integral of the answer to the last question is indeed the divergence of $\mathbf{F}$ :
   注意，最后一个问题的答案中的双重积分内的表达式确实是$\mathbf{F}$的散度：
   $$
   \operatorname{div} \mathbf{F}=\operatorname{div}\left[\begin{array}{c}
   P(x, y) \\
   Q(x, y)
   \end{array}\right]=\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}
   $$

5. Using the 2D divergence theorem?
   使用二维散度定理？

6. When it comes to translating between line integrals and double integrals, the $2 \mathrm{D}$ divergence theorem is saying basically the same thing as Green's theorem. So any of the actual computations in an example using this theorem would be indistinguishable from an example using Green's theorem (such as those in this article on Green's theorem examples).
   当涉及到线积分和双重积分之间的转换时，$2D$散度定理基本上在说与格林定理相同的事情。所以，使用这个定理的任何实际计算都无法与使用格林定理的例子区分开来（比如在这篇关于格林定理例子的文章中的那些）。

7. However, the usefulness of learning the 2D divergence theorem is two-fold:
   然而，学习二维散度定理的有用之处有两个：

8. Conceptual benefit: It's a great way to deepen your understanding of flux, divergence, and Green's theorem.
   概念上的好处：这是深化你对流量、散度和格林定理理解的好方法。

1. Strategic benefit: Sometimes an example where Green's theorem is used lends itself more naturally to a divergence-based description. For example, if the line integral you want to compute begins its life as a flux integral, rather than expanding out this line integral to make it look like $\int P dx+Q dy$ and applying Green's theorem, you could recognize immediately that it's the same as doubly integrating divergence.
   策略性的好处：有时，使用格林定理的例子更自然地适用于基于散度的描述。例如，如果你想计算的线积分开始时是一个通量积分，而不是将这个线积分展开使其看起来像 $\int P dx+Q dy$ 并应用格林定理，你可以立即认出它与双重积分散度是相同的。

--- pic\2D divergence theorem.pdf_09.png ---


1.  Summary
    总结

2.  The 2D divergence theorem relates two-dimensional flux and the double integral of divergence through a region.
    二维散度定理关联了二维流量和通过一个区域的散度的双重积分。
   $$
    \underbrace{\int_C \mathbf{F} \cdot \hat{\mathbf{n}} d s}_{\text {从 } R \text { 外部流出 }}=\underbrace{\iint_R \operatorname{div} \mathbf{F} d A}_{\text {所有小块外部流出的总和 }}
    $$


3.  Often the vector field $\mathbf{F}(x, y)$ is expressed component-wise:
    通常，矢量场$\mathbf{F}(x, y)$是按分量表示的：
    $$
    \mathbf{F}(x, y)=\left[\begin{array}{l}
    P(x, y) \\
    Q(x, y)
    \end{array}\right]
    $$

4.  In this case, here's how the 2D divergence theorem looks:
    在这种情况下，二维散度定理是这样的：
    $$
    \oint_C P d y-Q d x=\iint_R\left(\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}\right) d A
    $$

5.  In this form, it is easier to see that the 2D divergence theorem really just states the same thing as Green's theorem.
    在这种形式下，更容易看出二维散度定理实际上只是陈述了与格林定理相同的事情。









