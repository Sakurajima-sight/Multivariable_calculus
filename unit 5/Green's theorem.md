
--- pic\Green's theorem.pdf_00.png ---
1. Green's theorem
格林定理

1. Green's theorem relates the double integral curl to a certain line integral.
   格林定理将双重积分旋度与某个线积分关联起来。

2. It's actually really beautiful.
   它实际上非常美丽。

1. Background
背景知识

2. Double integrals.
   双重积分。

3. Line integrals in a vector field.
   矢量场中的线积分。

4. Two-dimensional curl.
   二维旋度。

5. Not strictly required, but helpful for a fuller understanding:
   不是严格要求，但有助于更全面的理解：

    Formal definition of curl in two dimensions.
二维旋度的正式定义。

1. Other resources
其他资源

1. You can find examples of how Green's theorem is used to solve problems in the next article.
   在下一篇文章中，你可以找到格林定理如何用来解决问题的例子。

2. Here, I will walk through what I find to be a beautiful line of reasoning for why it is true.
   在这里，我将走过我发现的一条美丽的推理线，解释为什么它是真的。

3. You can find a different perspective in Sal's video on the topic.
   你可以在Sal's video的主题中找到一个不同的视角。

1. One lesson, four times the payoff
一次学习，四倍的收益

1. Green's theorem is one of four major theorems at the culmination of multivariable calculus: Green's theorem, 2D divergence theorem, Stokes' theorem, 3D Divergence theorem.
   格林定理是多元微积分高潮部分的四个主要定理之一：格林定理，二维散度定理，斯托克斯定理，三维散度定理。

8. Here's the good news: All four of these have very similar intuitions.
   这是个好消息：这四个定理都有非常相似的直觉。

9. So if you really get to the point where you feel Green's theorem in your bones, you're already most of the way there to understanding these other three!
   所以，如果你真的能深刻理解格林定理，你已经大部分理解了其他三个定理！

1. What we're building to
我们正在构建的

9. Setup:
   设置：

--- pic\Green's theorem.pdf_01.png ---
1. $\mathbf{F}$ is a two-dimensional vector field.
   $\mathbf{F}$ 是一个二维向量场。

2. $R$ is some region in the $x y$ plane.
   $R$ 是$x y$ 平面中的某个区域。

3. $C$ is the boundary of that region, oriented counterclockwise.
   $C$ 是该区域的边界，按逆时针方向定向。

4. Green's theorem states that the line integral of $\mathbf{F}$ around the boundary of $R$ is the same as the double integral of the curl of $\mathbf{F}$ within $R$ :
   格林定理表明，$\mathbf{F}$在$R$边界上的线积分与$\mathbf{F}$在$R$内部的旋度的二重积分相同：
   $$
   \iint_R 2 \mathrm{~d}-\operatorname{curl} \mathbf{F} d A=\oint_C \mathbf{F} \cdot d \mathbf{r}
   $$

5. You think of the left-hand side as adding up all the little bits of rotation at every point within a region $R$, and the right-hand side as measuring the total fluid rotation around the boundary $C$ of $R$.
   你可以把左边看作是将$R$区域内每一点的所有小旋转量累加起来，而右边则是测量围绕$R$的边界$C$的总体流体旋转。

6. Often times $\mathbf{F}$ is written component-wise as follows:
   通常，$\mathbf{F}$按分量写成如下形式：
   $$
   \mathbf{F}(x, y)=P(x, y) \hat{\mathbf{i}}+Q(x, y) \hat{\mathbf{j}}
   $$

7. In terms of $P$ and $Q$, here's what Green's theorem looks like:
   用$P$ 和 $Q$表示，格林定理可以写为：
   $$
   \oint_C P d x+Q d y=\iint_R\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d A
   $$

8. Fluid rotation around a boundary.
   流体围绕边界旋转。

1. As you read on, the picture to have in your head is a blob in a vector field.
   当你继续阅读时，你脑海中应该想象的画面是一个在向量场中的斑点。

10. $\mathbf{F}(x, y)$ is the function for the vector field.
$\mathbf{F}(x, y)$ 是向量场的函数。

11. And, as you're probably getting used to if you've read other articles like this involving vector fields, imagine that $\mathbf{F}$ represents a fluid flow.
如果你阅读过其他涉及向量场的文章，你可能已经习惯了将 $\mathbf{F}$ 想象为流体流动。

1. $R$ is some region in the $x y$ -plane.
   $R$ 是 $x y$ 平面上的某个区域。

2. In practice, and in problems, it will be some well-defined shape like a circle or the boundary between two graphs, but while thinking abstractly I like to just draw it as a blob.
   在实践和问题中，它将是一个像圆或两个图形之间的边界这样的明确定义的形状，但在抽象思考时，我喜欢将其画成一个斑点。

--- pic\Green's theorem.pdf_02.png ---

1. $C$ is the boundary of $R$, oriented counterclockwise.
   $C$是$R$的边界，以逆时针方向定向。

2. Remember that orientation, because it actually matters when you solve problems. 
   请记住这个方向，因为在解决问题时，这实际上是很重要的。

4. Counterclockwise. Are you remembering it? Counterclockwise.
   逆时针。你记住了吗？逆时针。

5. Concept check: How can you interpret the following line integral in terms of a fluid flow?
   概念检查：你如何在流体流动的角度解释以下线积分？

   $$
   \oint_C \mathbf{F} \cdot d \mathbf{r}
   $$

1. (Remember, in a line integral through a vector field, the term $d \mathbf{r}$ represents a tiny step along the curve, as a vector, which in this case will always point in the counterclockwise direction.)
（记住，在向量场中的线积分中，项$d \mathbf{r}$代表曲线上的一个微小步长，作为一个向量，在这种情况下它总是指向逆时针方向。）

6. Choose 1 answer: 
   选择1个答案：

1. It will be positive if the fluid has an overall counterclockwise rotation around the boundary of $R$, and negative if that overall rotation is clockwise.
  如果流体在$R$的边界周围有整体的逆时针旋转，那么它将是正的，如果整体旋转是顺时针的，那么它将是负的。

1. Here's one way to think about the line integral $\oint_C \mathbf{F} \cdot d \mathbf{r}$ : Image rowing a boat around the line $C$, counterclockwise.
   这是一种思考线积分$\oint_C \mathbf{F} \cdot d \mathbf{r}$的方法：想象在线$C$周围逆时针划船。

2. At each point of your journey, the vector $d \mathbf{r}$ gives the direction of your motion.
在你旅程的每一个点，向量 $d \mathbf{r}$ 给出了你的运动方向。

1. The dot product $\mathbf{F} \cdot d \mathbf{r}$ will be positive at points where the fluid flow is with you, and negative at points where it's against you.
   点积 $\mathbf{F} \cdot d \mathbf{r}$ 在流体流动与你同向的点处为正，在流体流动与你反向的点处为负。

3. $\mathbf{F} \cdot d \mathbf{r}>0 \Rightarrow$ Flow helps
   $\mathbf{F} \cdot d \mathbf{r}>0 \Rightarrow$ 流动有帮助

4.  $\mathbf{F} \cdot d \mathbf{r}<0 \Rightarrow$ Flow impedes
    $\mathbf{F} \cdot d \mathbf{r}<0 \Rightarrow$ 流动有阻碍

--- pic\Green's theorem.pdf_03.png ---
1. On the whole, the line integral $\oint_C \mathbf{F} \cdot d \mathbf{r}$ adds up all these dot products to tell you if the flow was generally helpful or burdensome.
   总的来说，线积分 $\oint_C \mathbf{F} \cdot d \mathbf{r}$ 将所有这些点积加起来，告诉你流动是总体上有帮助还是有负担。

2. So this line integral is positive when the fluid flow has a general counterclockwise tendency around the boundary $C$ (meaning it was generally helpful), and it will be negative if it has a clockwise tendency (generally burdensome).
   因此，当流体流动在边界 $C$ 周围具有一般的逆时针趋势时（意味着它通常是有帮助的），这个线积分是正的，如果它有一个顺时针趋势（通常是有负担的），它将是负的。

3. Bringing the boundary to the interior
   将边界带入内部

4. Green's theorem is all about taking this idea of fluid rotation around the boundary of $R$, and relating it to what goes on inside $R$. Conceptually, this will involve chopping up $R$ into many small pieces.
   格林定理就是要将液体在 $R$ 的边界周围旋转的这个概念，与 $R$ 内部的情况联系起来。从概念上讲，这将涉及将 $R$ 切成许多小块。

5. In formulas, the end result will be taking the double integral of $2 \mathrm{~d}$-curl $\mathbf{F}$.
   在公式中，最终结果将是取 $2 \mathrm{~d}$-curl $\mathbf{F}$ 的双重积分。

6. Cut the region
   切割区域

7. Imagine chopping up the region $R$ with a line straight down the middle, giving two subregions $R_1$ and $R_2$.
   想象一下，用一条直线从中间切割区域 $R$，得到两个子区域 $R_1$ 和 $R_2$。


8. Name the boundaries of these two regions $C_1$ and $C_2$.
   给这两个区域的边界命名为 $C_1$ 和 $C_2$。

9. What happens if we take the line integral of $\mathbf{F}$ around these two boundaries, and add them up?
   如果我们在这两个边界周围取 $\mathbf{F}$ 的线积分，并将它们加起来，会发生什么呢？
   
10. $
   \oint_{C_1} F \cdot d \mathbf{r}+\oint_{C_2} F \cdot d \mathbf{r}
   $

11. Notice, these line integrals will cancel out along the vertical line cut that you made.
    注意，这些线积分将沿着你所做的垂直线切割抵消。

1. Namely, the integral around $C_1$ goes "up" this line, while the integral around $C_2$ integrates "down" this line.
   也就是说，围绕 $C_1$ 的积分在这条线上"上升"，而围绕 $C_2$ 的积分在这条线上"下降"。

--- pic\Green's theorem.pdf_04.png ---
1. (Remember, when performing a line integral in a vector field, changing the direction along a curve multiplies your result by -1 ).
   （记住，当在矢量场中进行线积分时，改变曲线上的方向会使你的结果乘以-1）。

2. This means the sum of our two integrals is the same as just going around the full boundary $C$.
   这意味着我们的两个积分的和就等于绕整个边界$C$进行积分。

3. You could do this one more time, maybe with a horizontal cut this time.
   你可以再做一次，这次可能是横切。

4. If you integrate around the boundaries of the resulting four subregions, the integrals will all cancel out along the cuts you made in the interior of $R$.
   如果你对产生的四个子区域的边界进行积分，那么你在$R$的内部所做的切割将使所有的积分都抵消。

5. In a formula, this means the sum of the line integrals around all four subregions end up just equalling the line integral around the full region.
   在公式中，这意味着所有四个子区域周围的线积分的和最终等于围绕整个区域的线积分。

6. I should emphasize that this only works if we make sure that all the boundaries $C_1, \ldots, C_4$ are oriented the same way.
   我应该强调，这只在我们确保所有的边界$C_1, \ldots, C_4$方向相同的情况下才有效。

7. Otherwise, they might not cancel each other out along the cuts.
   否则，它们可能无法沿着切口相互抵消。

8. It's common to think of counterclockwise as being the positive direction, so think about everything as being oriented counterclockwise.
   我们通常认为逆时针是正方向，所以要把所有的东西都看作是逆时针方向。

1. Cut it many, many times.
   将其切割很多很多次。


9. You might be able to see where I'm going with this.
   你可能能看出我这是要干什么。

10. Imagine chopping off the region $R$ into many, many tiny pieces, $R_1, \ldots, R_n$.
   想象一下将区域$R$切成许多许多小块，$R_1, \ldots, R_n$。

2. Orient all of their boundaries $C_1 , \ldots , C_n$ counterclockwise, and integrate the function $F$ over each one.
   将所有的边界 $C_1 , \ldots , C_n$ 逆时针排列，并对每一个边界上的函数 $F$ 进行积分。

--- pic\Green's theorem.pdf_05.png ---

1. The integrals will cancel out along all the cuts inside $R$ itself.
   在$R$内部的所有切割线上，积分将会互相抵消。

2. This is because for any cut, one of the integrals will go along it in one direction, while another goes along it in the other direction.
   这是因为对于任何切割，一个积分将沿着一个方向进行，而另一个积分将沿着另一个方向进行。

3. In the end, the only parts where these integrals don't cancel are the pieces of the boundary $C$.
   最后，这些积分不会取消的唯一部分是边界$C$的部分。

4. This means adding up the line integrals along the tiny boundaries of the pieces will give the same result as just integrating across the full region:
   这意味着，加起来沿着各小块边界的线积分将得到与仅在全区域进行积分相同的结果：
   $$
   \sum_{k=1}^n\left(\oint_{C_k} F \cdot d \mathbf{r}\right)=\oint_C F \cdot d \mathbf{r}
   $$

5. Integrating curl.
   积分旋度。

6. So... why am I doing this? It's because there is another way to interpret each of these line integrals around a tiny piece using two-dimensional curl.
   那么...我为什么要这么做？这是因为有另一种方式可以解释使用二维旋度围绕一个小片段的每个线积分。

7. Pick one of those pieces and zoom in on it.
   挑选其中一片并放大查看。

8. Let $R_k$ be the piece you chose, with boundary $C_k$.
   设$R_k$为你选择的那片，边界为$C_k$。

9.  Let $\left|R_k\right|$ represent the area of $R_k$, which we are thinking of as being some very small number.
    让 $\left|R_k\right|$ 表示 $R_k$ 的面积，我们认为这是一个非常小的数。

10. Let $\left(x_k, y_k\right)$ be some point sitting inside this piece, any point really.
    让 $\left(x_k, y_k\right)$ 是这块区域内的某个点，实际上可以是任何点。

11. The fluid rotation around this piece due to $\mathbf{F}$ can be measured with the line integral $\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}$.
   由于 $\mathbf{F}$ ，围绕这一部分的流体旋转可以用线积分 $\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}$ 来测量。

12. Think tiny row boat. But since this is a really small piece, there is another multivariable calculus concept that measures fluid rotation: Curl.
   想象一艘小船。但由于这是一个非常小的部分，还有另一个多元微积分概念可以衡量流体旋转：旋度。

--- pic\Green's theorem.pdf_06.png ---
1. This line integral can be approximated by taking the $2 \mathrm{~d}$-curl of $\mathrm{F}$ at any point within $R_k$, and multiplying it by the (tiny) area $\left|R_k\right|$ :
   这个线积分可以通过取$R_k$中任意一点的$\mathrm{F}$的$2 \mathrm{~d}$-curl，并将其乘以(微小的)面积$\left|R_k\right|$来近似表示：

2. $$
   \underbrace{\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}}_{\substack{\text { Integral around a } \\ \text { tiny piece } R_k}} \approx(2 \mathrm{~d}-\operatorname{curl} \mathbf{F} \underbrace{\left(x_k, y_k\right)}_{\text {Point in } R_k}) \underbrace{\left|R_k\right|}_{\text {Area of } R_k}
   $$
   $$\underbrace{\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}}_{\substack{\text { 围绕一个微小的部分 } R_k \\ \text { 的积分 }}} \approx(2 \mathrm{~d}-\operatorname{curl} \mathbf{F} \underbrace{\left(x_k, y_k\right)}_{R_k中的点}) \underbrace{\left|R_k\right|}_{R_k的面积}$$

3. Also, and this is important, the smaller $R_k$ is, the better this approximation is.
   另外，这一点很重要，$R_k$越小，这个近似就越好。


4. For those of you who read the article on the formal definition of curl in two dimensions, this approximation might feel very familiar.
   对于那些阅读过二维旋度的正式定义的文章的人来说，这个近似可能感到非常熟悉。

5. In fact, it's very close to the formal definition of curl itself, where you imagine shrinking a region around a point:
   事实上，它非常接近旋度本身的正式定义，你可以想象缩小一个点周围的区域：

6. $$
   2 \mathrm{~d}-\operatorname{curl} \mathbf{F}(x, y)=\lim _{\left|R_{(x, y)}\right| \rightarrow 0}\left(\frac{1}{\left|R_{(x, y)}\right|} \oint_{C_{(x, y)}} \mathbf{F} \cdot d \mathbf{r}\right)
   $$

7. Here, I'm using $R_{(x, y)}$ to represent any region containing the point $(x, y)$.
   在这里，我用$R_{(x, y)}$来表示包含点$(x, y)$的任何区域。

8. The meaning of the limit as $\left|R_{(x, y)}\right| \rightarrow 0$ is that the smaller the area of the region, the closer the following approximation will be:
   当$\left|R_{(x, y)}\right| \rightarrow 0$的极限意味着区域的面积越小，下面的近似就越接近：

9. $$
   2 \mathrm{~d}-\operatorname{curl} \mathbf{F}(x, y) \approx \frac{1}{\left|R_{(x, y)}\right|} \oint_{C_{(x, y)}} \mathbf{F} \cdot d \mathbf{r}
   $$

10. This is essentially what the approximation written above says, except rather than starting with a point $(x, y)$ and considering a region $R_{(x, y)}$ around that point, I started with a tiny region $R_k$ and took some point $\left(x_k, y_k\right)$ inside of it:
   这本质上就是上面写的近似说的，除了从一个点$(x, y)$开始并考虑那个点周围的一个区域$R_{(x, y)}$，我从一个微小的区域$R_k$开始，并取它内部的一些点$\left(x_k, y_k\right)$：

11. $$
    (2 \mathrm{~d}-\operatorname{curl} \mathbf{F} \underbrace{\left(x_k, y_k\right)}_{\text {Point in } R_k}) \approx \frac{1}{\left|R_k\right|} \underbrace{\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}}_{\begin{array}{c}
    \text { Integral around a } \\
    \text { tiny piece } R_k
    \end{array}}
    $$
    $$ (2 \mathrm{~d}-\operatorname{curl} \mathbf{F} \underbrace{\left(x_k, y_k\right)}_{R_k中的点}) \approx \frac{1}{\left|R_k\right|} \underbrace{\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}}_{\begin{array}{c}
    \text { 围绕一个微小的 } \\
    \text { 部分 } R_k 的积分
    \end{array}} $$

1. Now just multiply both sides by $\left|R_k\right|$, and you get the approximation I originally claimed:
   现在只需将等式两边都乘以 $\left|R_k\right|$，你就得到了我最初提出的近似值：

--- pic\Green's theorem.pdf_07.png ---

1. $$\underbrace{\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}}_{\substack{\text { 积分围绕一个 } \\ \text { 微小片段 } R_k}} \approx(2 \mathrm{~d}-\operatorname{curl} \mathbf{F} \underbrace{\left(x_k, y_k\right)}_{\text { 点在 } R_k}) \underbrace{\left|R_k\right|}_{\text R_{k} { 的面积 }}$$

2. Moreover, if you really want to wrap your mind around the technical details here, you can make the following observation: We started with a certain approximation, whose error goes to zero for smaller pieces.
   此外，如果你真的想理解这里的技术细节，你可以做以下观察：我们从一个特定的近似开始，其误差对于较小的片段趋向于零。

1. Since our final approximation came from multiplying both sides by the area $\left|R_k\right|$, its error not only goes to zero, but it must remain significantly smaller than $\left|R_k\right|$ as it does so.
   由于我们的最终近似是通过将两边都乘以面积 $\left|R_k\right|$ 得到的，它的误差不仅会趋向于零，而且在这样做的过程中，它必须保持明显小于 $\left|R_k\right|$。

4. It's okay if you want to ignore this fact, but it becomes important for a technical detail down the road.
   如果你想忽略这个事实，那也没关系，但是这对于以后的技术细节会变得重要。

5. Adding up these approximations over all of the tiny pieces $R_k$, here's what you get:
   把所有的小片段 $R_k$ 上的这些近似值加起来，你会得到：

$$
\sum_{k=1}^n\left(\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}\right) \approx \sum_{k=1}^n(2 \mathrm{~d}-\operatorname{curl} \mathbf{F} \underbrace{\left(x_k, y_k\right)}_{\text { 点在 } R_k}\left|R_k\right|)
$$

6. Taking the conclusion from the previous section, the left-hand side above is the same as a single line integral around the full boundary of $R$, so we can rewrite this approximation as follows:
   从前一节的结论来看，上面的左边就等于围绕 $R$ 的完整边界的单个线积分，所以我们可以按如下方式重写这个近似：

$$
\oint_C \mathbf{F} \cdot d \mathbf{r} \approx \sum_{k=1}^n(2 \mathrm{~d}-\operatorname{curl} \mathbf{F} \underbrace{\left(x_k, y_k\right)}_{\text { 点在 } R_k}\left|R_k\right|)
$$

7. Now take a close look at the sum on the right-hand side.
   现在仔细看看右边的总和。

8. It includes a scalar-valued function, $2d$-curl $F$.
   它包含一个标量值函数，$2d$-curl $F$。

9. The sum is taken over many tiny pieces $R_k$ of a two-dimensional region, $R$.
   总和是在二维区域 $R$ 的许多小片段 $R_k$ 上取得的。

--- pic\Green's theorem.pdf_08.png ---
1. For each piece within the sum, the function is evaluated on a point inside that piece, then multiplied by its area.
   对于和中的每一部分，函数在该部分内的一个点上进行评估，然后乘以它的面积。

2. Sound familiar? This is all the recipe for a double integral! (If this does not sound familiar, consider taking a look at this article on double integrals).
   听起来熟悉吗？这就是双重积分的所有配方！（如果这听起来不熟悉，可以考虑看一下关于双重积分的这篇文章）。

3. In particular, if you imagine chopping up the region $R$ more and more finely, you can replace the sum above with a double integral of $2 \mathrm{d}$-curl $\mathbf{F}$ over $R$ :
   特别是，如果你想象将区域$R$越来越细微地切割，你可以将上面的和替换为对$R$的$2 \mathrm{d}$-旋度 $\mathbf{F}$的双重积分：
   
   $$
   \sum_{k=1}^n(2 \mathrm{d}-\operatorname{curl} \mathbf{F} \underbrace{\left(x_k, y_k\right)}_{\text {Point in } R_k}\left|R_k\right|) \rightarrow \iint_R 2 \mathrm{d}-\operatorname{curl} \mathbf{F} d A
   $$
   
4. Putting everything together, here's what we have:
   将所有的东西放在一起，这就是我们得到的：
   
   $$
   \begin{aligned}
   \oint_C \mathbf{F} \cdot d \mathbf{r} & =\sum_{k=1}^n\left(\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}\right) \\
   & \approx \sum_{k=1}^n(2 \mathrm{d}-\operatorname{curl} \mathbf{F} \underbrace{\left(x_k, y_k\right)}_{\text {Point in } R_k}\left|R_k\right|) \\
   & \rightarrow \iint_R 2 \mathrm{d}-\operatorname{curl} \mathbf{F} d A
   \end{aligned}
   $$

5. This is actually more than a mere approximation, the line integral around the boundary equals the double integral of two-dimensional curl:
   这实际上不仅仅是一个近似，边界周围的线积分等于二维旋度的双重积分：
   
   $$
   \oint_C \mathbf{F} \cdot d \mathbf{r}=\iint_R 2 \mathrm{d}-\operatorname{curl} \mathbf{F} d A
   $$

6. [Wait, how did that approximation turn into an equality?].
   [等一下，那个近似怎么变成等式了？] 见最后一页（补充）

7. This marvelous fact is called Green's theorem.
   这个神奇的事实被称为格林定理。

8. When you look at it, you can read it as saying that the rotation of a fluid around the full boundary of a region (the left-hand side) is the same as looking at all the little "bits of rotation" inside the region and adding them up (the right-hand side).
   当你看它时，你可以把它理解为：一个区域完整边界上的流体旋转（左侧）等同于观察该区域内的所有小的“旋转位”并将它们加起来（右侧）。

--- pic\Green's theorem.pdf_09.png ---
1. Alternative notation
   备选符号表示法

2. It is very common to see Green's theorem written like this:
   常常可以看到格林定理被这样写出：

   $$
   \oint_C P dx+Q dy=\iint_R\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) dA
   $$

3. This is just spelling out the dot product in the left-hand side line integral, as well as the curl in the right-hand side double integral.
   这只是将左侧线积分中的点积以及右侧双重积分中的旋度详细写出。

4. For whatever reason, it is common to use the letters $P$ and $Q$ to denote the components of the vector-valued function $\mathrm{F}(x, y)$ :
   不论出于何种原因，通常用字母$P$和$Q$来表示向量值函数$\mathbf{F}(x, y)$的组成部分：

   $$
   \mathbf{F}(x, y)=P(x, y) \hat{\mathbf{i}}+Q(x, y) \hat{\mathbf{j}}=\left[\begin{array}{c}
   P(x, y) \\
   Q(x, y)
   \end{array}\right]
   $$

5. In the line integral $\oint_C \mathbf{F} \cdot d \mathbf{r}$, the differential term $d \mathbf{r}$ is a vector representing a small step along the curve $C$.
   在线积分$\oint_C \mathbf{F} \cdot d \mathbf{r}$中，微分项$d \mathbf{r}$是表示沿曲线$C$的一个小步骤的向量。

6. You can break it down as the $x$-component of that small step, $dx$, and the $y$-component of that step, $dy$ :
   你可以将它拆分为那个小步骤的$x$分量，$dx$，和那个步骤的$y$分量，$dy$：

   $$
   d \mathbf{r}=\left[\begin{array}{l}
   dx \\
   dy
   \end{array}\right]
   $$

7. This means the dot product within the integral expands as follows:
   这意味着积分中的点积可以如下展开：

   $$
   \oint_C \mathbf{F} \cdot d \mathbf{r}=\oint_C\left[\begin{array}{l}
   P \\
   Q
   \end{array}\right] \cdot\left[\begin{array}{l}
   dx \\
   dy
   \end{array}\right]=\oint_C P dx+Q dy
   $$

--- pic\Green's theorem.pdf_10.png ---
1. The formula for $2 \mathrm{~d}$-curl $\mathrm{F}$ is as follows:
   $2 \mathrm{~d}$-旋度 $\mathrm{F}$ 的公式如下：

$$
2 \mathrm{~d}-\operatorname{curl}\left(\left[\begin{array}{c}
P(x, y) \\
Q(x, y)
\end{array}\right]\right)=\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}
$$

2. A memory trick for this is to think about the following determinant:
   记住这个的一个技巧是，考虑以下的行列式：

$$
\operatorname{det}\left(\left[\begin{array}{cc}
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} \\
P(x, y) & Q(x, y)
\end{array}\right]\right)
$$

3. If you are rusty on this, or wish to see a bit of intuition for why this formula relates to fluid rotation, see this article on two-dimensional curl.
   如果你对这个不太熟悉，或者希望了解为什么这个公式与流体旋转相关，可以查看关于二维旋度的文章。

4. In the next article, you will find examples of how this formula can be used to make either line integrals or double integrals simpler.
   在下一篇文章中，你将会看到一些例子，说明如何使用这个公式来简化线积分或双重积分。

5. Summary:
   总结：

6. You can think about the line integral $\oint_C \mathbf{F} \cdot d \mathbf{r}$ as measuring the rotation of the fluid flow represented by the vector field $\mathbf{F}(x, y)$ around the curve $C$.
   你可以将线积分 $\oint_C \mathbf{F} \cdot d \mathbf{r}$ 理解为测量由向量场 $\mathbf{F}(x, y)$ 表示的流体流动围绕曲线 $C$ 的旋转。

7. It is conventional to think of counterclockwise rotation as being positive, in which case $C$ should be oriented counterclockwise.
   按照惯例，我们将逆时针旋转视为正方向，因此 $C$ 应该是逆时针方向的。

8. Imagine chopping up the two-dimensional region $R$ enclosed by $C$ into many tiny pieces.
   想象将由 $C$ 包围的二维区域 $R$ 切割成许多小块。

9. Name the boundaries of these pieces $C_1, \ldots, C_n$, and orient them all counterclockwise.
   将这些小块的边界命名为 $C_1, \ldots, C_n$，并且它们都是逆时针方向的。

10. Then adding up the line integrals of $\mathbf{F}$ around each piece-boundary $C_k$ boils down to the same thing as the line integral around the full boundary $C$.
    然后，将每个边界 $C_k$ 上的 $\mathbf{F}$ 的线积分相加，其结果与整个边界 $C$ 上的线积分相同。

$$
\sum_{k=1}^n\left(\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}\right)=\oint_C \mathbf{F} \cdot d \mathbf{r}
$$

11. That is to say, the little line integrals cancel out along all the cuts within $R$.
    也就是说，所有在 $R$ 内部的切割线上的小线积分都会相互抵消。

12. As you consider smaller and smaller pieces, the line integral around each tiny piece can be approximated using two-dimensional curl:
    当你考虑越来越小的块，每个小块周围的线积分可以使用二维旋度进行近似：

--- pic\Green's theorem.pdf_11.png ---

1. 
$$
\underbrace{\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}}_{\begin{array}{c}
\text { Integral around a } \\
\text { tiny piece } R_k
\end{array}} \approx(2 \mathrm{~d}-\operatorname{curl} \mathbf{F} \underbrace{\left(x_k, y_k\right)}_{\text {Point in } R_k}) \underbrace{\left|R_k\right|}_{\text {Area of } R_k}
$$

$$
\underbrace{\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}}_{\begin{array}{c}
\text {环绕一个小片段 } R_k \\
\text { 的积分}
\end{array}} \approx(2 \mathrm{~d}-\operatorname{curl} \mathbf{F} \underbrace{\left(x_k, y_k\right)}_{\text {在 } R_k \text { 中的点}}) \underbrace{\left|R_k\right|}_{\text R_k{的面积}}
$$

2. Adding up these little "bits of curl" using a double integral over $R$, and applying the fact that the sum of the line integrals cancels out along interior cuts, you get Green's theorem:
   使用对$R$的双重积分将这些小的"旋度位"加起来，并应用线积分的和沿内部切割取消的事实，你可以得到格林定理：

$$
\oint_C \mathbf{F} \cdot d \mathbf{r}=\iint_R 2 \mathrm{~d}-\operatorname{curl} \mathbf{F} d A
$$

--- pic\Green's theorem.pdf_12.png ---

1. Okay, there are some technicalities I should mention for the detail-oriented among you.
   好的，我有一些技术性的细节要向你们这些注重细节的人提及。

2. Remember the step of adding up all the individual line-integral-to-curl approximations? That's what gave us this approximation:
   还记得加总所有单个线积分至旋度近似值的步骤吗？这就是我们得到这个近似值的方式：

$$
\sum_{k=1}^n\left(\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}\right) \approx \sum_{k=1}^n(2 \mathrm{~d}-\operatorname{curl} \mathbf{F} \underbrace{\left(x_k, y_k\right)}_{\text {Point in } R_k}\left|R_k\right|)
$$

3. For all we know, without further investigation, the errors for each of these approximations add up to something substantial.
   就我们所知，如果不进行进一步的调查，这些近似值的每一个误差加起来可能会非常大。

4. This might mean that when we chop up $R$ more and more finely, and the sum gets bigger and bigger, the accumulation of errors gets out of hand, even though each individual error per piece approaches 0.
   这可能意味着，当我们将$R$划分得越来越细，总和越来越大时，误差的累积可能会失控，即使每个单元的单个误差接近0。

5. Luckily, this does not happen.
   幸运的是，这种情况并没有发生。

6. For those of you who read the end of the little technical note above justifying the original approximation using the formal definition of curl, do you remember what I said at the end?
   对于那些阅读了上面那段小小的技术注释的人，这段注释使用旋度的正式定义来证明原始近似，你还记得我最后说了什么吗？

7. The error of that approximation is significantly smaller than the area of $R_k$.
   那个近似的误差明显小于$R_k$的面积。

8. Since the sum of the areas of each piece $R_k$ is the area of the full region $R$, a constant, this means the sum of the error terms will be significantly smaller than a constant.
   由于每个部分$R_k$的面积的总和是整个区域$R$的面积，即一个常数，这意味着误差项的总和将明显小于一个常数。

9. That is to say, they will be significantly small, period.
   也就是说，它们将会非常小，就是这样。

10. This means the overall approximation really does approach equality when we pass to the double integral, so we can feel justified in writing this equation:
    这意味着，当我们转向双重积分时，整体的近似值确实接近相等，因此我们在写下这个等式时可以感到合理：

$$
\oint_C \mathbf{F} \cdot d \mathbf{r}=\iint_R 2 \mathrm{~d}-\operatorname{curl} \mathbf{F} d A
$$