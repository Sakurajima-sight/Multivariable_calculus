
--- pic\Stokes' theorem.pdf_00.png ---
1. Stokes' theorem
   斯托克斯定理

2. This is the $3 d$ version of Green's theorem, relating the surface integral of a curl vector field to a line integral around that surface's boundary.
   这是格林定理的$3d$版本，将旋度矢量场的表面积分与该表面边界的线积分关联起来。

3. Background
   背景

4. Green's theorem
   格林定理

5. Flux in three dimensions
   三维的通量

6. Curl in three dimensions
   三维的旋度

7. Not strictly required, but very helpful for a deeper understanding:
   不是严格要求，但对于深入理解非常有帮助：

8. Formal definition of curl in three dimensions
   三维旋度的正式定义

9. This article is for physical intuition
   这篇文章是为了物理直觉

10. If you would like examples of using Stokes' theorem for computations, you can find them in the next article. Here, the goal is to present the theorem in such a way that you can get a gut feeling for what it is really saying, and why it is true.
    如果你想要使用斯托克斯定理进行计算的例子，你可以在下一篇文章中找到它们。这里，我们的目标是以一种你能够直观理解的方式来阐述这个定理，让你真正理解它在说什么，以及为什么它是正确的。

11. What we're building to
    我们正在构建的是

12. Stokes' theorem is the 3D version of Green's theorem.
    斯托克斯定理是格林定理的3D版本。




--- pic\Stokes' theorem.pdf_01.png ---
1. It relates the surface integral of the curl of a vector field with the line integral of that same vector field around the boundary of the surface:
   它将矢量场的旋度的表面积分与该矢量场在表面边界周围的线积分关联起来：

1. Surface integral of a curl vector field
   曲面积分的旋度矢量场

2. $S$ is a surface in 3D
   $S$ 是一个三维的表面

3. Line integral around boundary of surface
   曲面边界的线积分

1. [Breakdown of terms] 
   [术语分解]（见最后一页）

1. Interpreting a line integral in 3D
   解释三维中的线积分

2. Let $\mathbf{F}(x, y, z)$ represent a three-dimensional vector field.
   让$\mathbf{F}(x, y, z)$表示一个三维矢量场。

3. Think of this vector field as being the velocity vector of some gas, whooshing about through space.
   把这个矢量场想象成某种气体的速度矢量，在空间中飞速移动。

4. Now let $C$ be some closed curve inside this vector field.
   现在让$C$是这个矢量场内的某个闭曲线。


--- pic\Stokes' theorem.pdf_02.png ---

1. How can you interpret the line integral of $\mathbf{F}$ around $C$ ?
   你如何解释$\mathbf{F}$在$C$周围的线积分？
   $$
   \oint_C \mathbf{F} \cdot d \mathbf{r}
   $$
2. Well, first of all, this integral doesn't make sense until the curve is oriented. The differential vector $d \mathbf{r}$ represents a tiny step along the curve, but in which direction? In three dimensions, you can't just say "clockwise" or "counterclockwise", since that will depend on where you are in space when you look at the curve. 
   首先，这个积分在曲线定向之前是没有意义的。微分向量$d \mathbf{r}$表示沿曲线的一个微小步长，但是方向是什么呢？在三维空间中，你不能只是说“顺时针”或“逆时针”，因为这将取决于你在空间中的位置，当你看曲线时。

2. I'll address how we specify orientation mathematically below, but for now, it's easier to just draw an orientation:
   我将在下面解释我们如何在数学上指定方向，但是现在，直接画出方向更容易：

--- pic\Stokes' theorem.pdf_03.png ---

1. Imagine you are a bird, flying through space along the curve $C$ while the wind blows according to the vector field $\mathbf{F}$. (For the purposes of this animation, you are a sphere-shaped bird).
   想象你是一只鸟，沿着曲线$C$在空间中飞翔，同时风按照矢量场$\mathbf{F}$吹动。（为了这个动画，你是一只球形的鸟）。

2. Think of each step (wing-flap?) of your motion along $C$ as being the tiny vector $d \mathbf{r}$. Consider the dot product between $d \mathbf{r}$ and the wind-velocity-vector from the field $\mathbf{F}$ where you are. It will be positive when the wind is helping you, and negative when it is in your face.
   把你沿$C$运动的每一步（翅膀的挥动？）想象成微小的向量$d \mathbf{r}$。考虑$d \mathbf{r}$和你所在位置的场$\mathbf{F}$的风速矢量之间的点积。当风帮助你时，它会是正的，当风在你面前时，它会是负的。

3.  Now look back at the line integral I originally asked about:
    现在回看我原先问的线积分：
    $$
    \oint_C \mathbf{F} \cdot d \mathbf{r}
    $$
4.  You can think of this as adding up how helpful or burdensome the wind was during your flight. It measures the tendency of the fluid flow to circulate around $C$. If it is positive, the wind was generally helpful, and you could say that it tends to circulate around $C$ in the direction of your specified orientation. If it is negative, you could say it tends to circulate the other way.
    你可以把这看作是在计算风在你飞行过程中有多大的帮助或负担。它衡量了流体流动围绕$C$循环的倾向。如果它是正的，风通常是有帮助的，你可以说它倾向于按照你指定的方向围绕$C$循环。如果它是负的，你可以说它倾向于反方向循环。

5.  Chopping up a surface
    切割一个表面

--- pic\Stokes' theorem.pdf_04.png ---

6.  Those of you who read the Green's theorem article will find what follows very familiar.
    那些读过格林定理文章的人会发现接下来的内容非常熟悉。

7.  Consider a surface $S$ in space whose boundary is the curve $C$, as if $C$ was a wire loop that you just dipped in soap, and $S$ is the beginnings of a soap bubble emerging from the loop.
    考虑一个在空间中的表面$S$，其边界是曲线$C$，就好像$C$是你刚刚浸在肥皂中的一个线圈，而$S$是从线圈中出现的肥皂泡的开始。

8.  Slice this surface in half, and name the boundaries of the two resulting pieces $C_1$ and $C_2$. 
    把这个表面切成两半，把两个结果的边界命名为$C_1$和$C_2$。

1. If they are each oriented the same way $C$ was, the line integrals (of the same vector field $F$) around each of these smaller curves cancel out along the slice that you made:
   如果它们每一个都以与 $C$ 相同的方式定向，那么这些较小曲线周围的线积分（相同的矢量场 $F$）在你切割的切片上会相互抵消：

--- pic\Stokes' theorem.pdf_05.png ---

1. The portions of $C_1$ and $C_2$ which remain make up the original boundary $C$. So the sum of the line integrals around the smaller pieces equals the full line integral around $C$ :
   $C_1$和$C_2$的剩余部分构成了原始边界$C$。所以，围绕较小部分的线积分之和等于围绕$C$的完整线积分：
   $$
   \underbrace{\oint_{C_1} \mathbf{F} \cdot d \mathbf{r}+\oint_{C_2} \mathbf{F} \cdot d \mathbf{r}}_{\text {沿着切过$S$的切片抵消}}=\oint_C \mathbf{F} \cdot d \mathbf{r}
   $$

2. More generally, imagine slicing up $S$ into many, many really small pieces, name their boundaries $C_1, \ldots, C_n$, and orient them all the same way as $C$. It gets messy drawing this in 3D, so I'll just steal an image from the Green's theorem article showing the $2 \mathrm{D}$ version, which has essentially the same intuition.
   更一般地，想象将$S$切割成许多许多非常小的片段，将它们的边界命名为$C_1, \ldots, C_n$，并将它们都按照与$C$相同的方式定向。在3D中绘制这个会很混乱，所以我只是从格林定理的文章中借用了一个显示$2D$版本的图像，它基本上具有相同的直觉。

3. The line integrals around all of these little loops will cancel out along the slices within $C$, leaving only something equal to the line integral around $C$ itself.
   所有这些小环的线积分将在$C$内的切片上抵消，只留下等于围绕$C$本身的线积分的东西。
$$
\underbrace{\sum_{k=1}^n \oint_{C_k} \mathbf{F} \cdot d \mathbf{r}}_{\text {沿着切过$S$的切片抵消 } }=\oint_C \mathbf{F} \cdot d \mathbf{r}
$$


1. Curl on each piece
   每一片的旋度

2. The reason for chopping up $S$ like this is that the line integral around a very small loop can be approximated using curl. Specifically, zoom in on a specific one of those pieces. If it's small enough, you can think of it as basically being flat.
   这样切割$S$的原因是，围绕一个非常小的环的线积分可以使用旋度来近似。具体来说，放大其中一个特定的片段。如果它足够小，你可以认为它基本上是平的。

--- pic\Stokes' theorem.pdf_06.png ---

7. Name the boundary of this piece " $C_k$ ".
   将这片的边界命名为"$C_k$ "。

8. Choose some point $\left(x_k, y_k, z_k\right)$ on the surface, inside this little loop.
   在这个小环内的表面上选择一些点$\left(x_k, y_k, z_k\right)$。

9. Let $\hat{\mathbf{n}}$ be a unit normal vector to the surface at the point $\left(x_k, y_k, z_k\right)$. "Pointing which way?", you might ask. Curl the fingers of your right hand around the little loop $C_k$ so that they align with its orientation. Stick out your thumb, and this is the direction of $\hat{\mathbf{n}}$.
   让$\hat{\mathbf{n}}$是在点$\left(x_k, y_k, z_k\right)$处的表面的单位法向量。"指向哪个方向？"你可能会问。将你的右手的手指卷绕在小环$C_k$周围，使它们与其方向对齐。伸出你的拇指，这就是$\hat{\mathbf{n}}$的方向。

10. Let $d \Sigma$ represent the area of this little piece (in anticipation of using an infinitesimal area for a surface integral in just a bit).
    让$d \Sigma$表示这个小片的面积（预期马上就要使用一个无穷小的面积进行表面积分）。

11. Then the line integral of $\mathbf{F}$ around $C_k$ can be approximated as follows:
    然后，围绕$C_k$的$\mathbf{F}$的线积分可以如下近似：
    $$
    \underbrace{\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}}_{\substack{\text { 积分环绕 } \\ \text { 片段的边界 }}} \approx \overbrace{\left(\left(\operatorname{curl} \mathbf{F}\left(x_k, y_k, z_k\right)\right) \cdot \hat{\mathbf{n}}\right)}^{\text {旋度的垂直于片段的分量 }} \underbrace{d \Sigma}_{\text {片段的面积 }}
    $$

12. If you feel uneasy about your intuition for what curl means, or how a vector can represent rotation, consider reviewing this article on curl.
    如果你对旋度的含义，或者向量如何表示旋转的直觉感到不安，可以考虑复习一下关于旋度的这篇文章。



--- pic\Stokes' theorem.pdf_07.png ---

1. Here's the loose intuition for why this approximation works: $\operatorname{curl} \mathbf{F}\left(x_k, y_k, z_k\right)$ is a vector which tells you how the fluid flowing along the vector field $\mathbf{F}$ tends to rotate near the point $\left(x_k, y_k, z_k\right)$. 
   这是为什么这种近似有效的直观理解：$\operatorname{curl} \mathbf{F}\left(x_k, y_k, z_k\right)$是一个向量，它告诉你沿着矢量场$\mathbf{F}$流动的流体在点$\left(x_k, y_k, z_k\right)$附近如何倾向于旋转。

2. For example, if you imagine a small tennis ball floating in space, centered at the point $\left(x_k, y_k, z_k\right)$, the vector $\operatorname{curl} \mathbf{F}\left(x_k, y_k, z_k\right)$ describes the way it will tend to spin due to the wind blowing around it. That is to say, the vector is directed along the axis of rotation, and its magnitude is proportional to the rate of rotation.
   例如，如果你想象一个小网球在空间中漂浮，以点$\left(x_k, y_k, z_k\right)$为中心，向量$\operatorname{curl} \mathbf{F}\left(x_k, y_k, z_k\right)$描述了由于风吹过它，它将倾向于如何旋转。也就是说，这个向量沿着旋转轴方向，其大小与旋转速率成正比。

3. When we take the dot product between this curl vector and $\hat{\mathbf{n}}$, the unit normal vector to the surface, it extract the component of the curl vector which is perpendicular to the surface. This will describe the rate of fluid rotation on the surface itself. On the other hand, that little bit of fluid rotation is also described by the line integral around the boundary of the tiny piece: $\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}$.
   当我们取这个旋度向量和$\hat{\mathbf{n}}$（表面的单位法向量）之间的点积时，它提取了旋度向量的那个垂直于表面的分量。这将描述表面本身的流体旋转速率。另一方面，那一点点的流体旋转也由围绕小片边界的线积分描述：$\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}$。

4. Actually, that line integral produces a really small number (since $C_k$ is very short), but curl $\mathbf{F}\left(x_k, y_k, z_k\right)$ produces a number which doesn't care about the size of the piece containing $\left(x_k, y_k, z_k\right)$. This is why we scale down the relevant component of curl by the area of the tiny piece.
   实际上，那个线积分产生了一个非常小的数（因为$C_k$非常短），但是旋度$\mathbf{F}\left(x_k, y_k, z_k\right)$产生了一个不关心包含$\left(x_k, y_k, z_k\right)$的片段的大小的数。这就是为什么我们通过小片的面积来缩小旋度的相关分量。
    $$
    \underbrace{\oint_{C_k} \mathbf{F} \cdot d \mathbf{r}}_{\substack{\text { 积分环绕 } \\ \text { 片段的边界 }}} \approx \overbrace{\left(\left(\operatorname{curl} \mathbf{F}\left(x_k, y_k, z_k\right)\right) \cdot \hat{\mathbf{n}}\right)}^{\text {旋度的垂直于片段的分量 }} \underbrace{d \Sigma}_{\text {片段的面积 }}
    $$


5. (For a deeper understanding of this approximation, take a look at the formal definition of curl in three dimensions.)
   （为了更深入地理解这种近似，可以看一下三维旋度的正式定义。）

6. Surface integral of curl
   旋度的表面积分

7. Combining the ideas of the last two sections, here's what we get:
   结合最后两节的思想，我们得到了以下结果：
   $$
   \underbrace{\oint_C \mathbf{F} \cdot d \mathbf{r}}_{\begin{array}{c}
   \text { 积分围绕整个表面的 } \\
   \text { 边界 }
   \end{array}}
   $$

--- pic\Stokes' theorem.pdf_08.png ---

1. 
    $$
    \underbrace{\sum_{k=1}^n \oint_{C_k} \mathbf{F} \cdot d \mathbf{r}}_{\text {小片周围的积分之和 }}
    $$

2. 
   $$
   \underbrace{\sum_{k=1}^n \operatorname{curl} \mathbf{F}\left(x_k, y_k, z_k\right) \cdot \hat{\mathbf{n}} d \Sigma}_{\text {将旋度近似应用到每一片}}
   $$

3.  As we chop things up more and more finely, this last sum approaches the surface integral of $(\operatorname{curl} \mathbf{F} \cdot \hat{\mathbf{n}})$ over the surface $S$. (If this does not make sense to you, consider reviewing the article on surface integrals).
    当我们越来越细致地切割，这最后的和趋近于表面$S$上的$(\operatorname{curl} \mathbf{F} \cdot \hat{\mathbf{n}})$的表面积分。（如果这对你来说没有意义，可以考虑复习一下关于表面积分的文章。）
    $$
    \sum_{k=1}^n \operatorname{curl} \mathbf{F}\left(x_k, y_k, z_k\right) \cdot \hat{\mathbf{n}} d \Sigma
    $$
    $\downarrow$ 当$S$被切割得越来越细时
    $$
    \iint_S \operatorname{curl} \mathbf{F} \cdot \hat{\mathbf{n}} d \Sigma
    $$

4.  Putting this together, we have the following marvelous equation, known as Stokes' theorem:
    把这些放在一起，我们得到了以下的奇妙等式，被称为斯托克斯定理：
    $$
    \oint_C \mathbf{F} \cdot d \mathbf{r}=\iint_S \operatorname{curl} \mathbf{F} \cdot \hat{\mathbf{n}} d \Sigma
    $$

--- pic\Stokes' theorem.pdf_09.png ---

1. Okay, a few of you may raise the objection that I started with an approximation for the line integral around each piece, and am now making a conclusion using an approximation-free equality. And you'd be right to do so!
   好的，你们中的一些人可能会提出反对意见，我开始时用的是围绕每一片的线积分的近似值，现在我正在使用一个无近似的等式来得出结论。你们这样做是对的！

2. In the article on Green's theorem, which involves a nearly identical line of reasoning, but in two dimensions, I offered a couple notes to go into the details of how the approximation disappears. If you are curious, I encourage you to go back through that same line of reasoning and think about how it works for Stokes' theorem and surface integrals.
   在关于格林定理的文章中，我提供了一些注释来详细说明近似值是如何消失的，这涉及到几乎相同的推理线路，但是在二维中。如果你感到好奇，我鼓励你回顾那同样的推理过程，并思考它如何适用于斯托克斯定理和表面积分。

3. This exercise will also be made all the more enlightening if you go in armed with the formal definition of curl in three dimensions.
   如果你掌握了三维旋度的正式定义，这个练习将会更加有启发性。

4. Aligning orientation
   对齐方向

5. Surfaces are oriented by the chosen direction for their unit normal vectors. For example, you will often see a surface oriented using outward-facing unit normal vectors (although not all surfaces have a notion of outward-facing vs. inwardfacing unit normal vectors).
   表面的方向由其单位法向量的选定方向决定。例如，你经常会看到一个表面使用向外面的单位法向量来定向（尽管并非所有的表面都有朝向外部和朝向内部的单位法向量的概念）。

6. Curves are oriented by the chosen direction for their tangent vectors.
   曲线的方向由其切向量的选定方向决定。

7. For Stokes' theorem to work, the orientation of the surface and its boundary must "match up" in the right way. Otherwise, the equation will be off by a factor of -1 . Here are several different ways you will hear people describe what this matching up looks like; all are describing the same thing.
   为了使斯托克斯定理起作用，表面和其边界的方向必须以正确的方式“匹配”。否则，等式将会偏离-1的因子。这里有几种不同的方式，你会听到人们描述这种匹配看起来是什么样子；所有的都在描述同一件事。

--- pic\Stokes' theorem.pdf_10.png ---

8. If you look at the surface in such a way that the unit normal vectors are all pointed towards your face, the curve should be oriented counterclockwise.
   如果你以一种单位法向量都指向你的脸的方式来看待表面，曲线应该是逆时针方向的。

9. The curve's orientation should follow the right-hand rule, in the sense that if you stick the thumb of your right hand in the direction of a unit normal vector near the edge of the surface, and curl your fingers, the direction they point on the curve should match its orientation.
   曲线的方向应该遵循右手规则，意思是如果你将你的右手的拇指指向表面边缘附近的一个单位法向量的方向，并卷曲你的手指，它们在曲线上指向的方向应该与其方向匹配。

10. When you are walking along the boundary curve with your body pointing out in the direction of the unit normal vector, you should be walking in such a way that the surface is to your left side.
    当你沿着边界曲线行走，你的身体指向单位法向量的方向时，你应该以一种表面在你左边的方式行走。

11. Blowing bubbles
    吹泡泡

12. Here's something pretty awesome about Stokes' theorem: The surface itself doesn't matter, all that matters is what its boundary is.
    关于斯托克斯定理有一点非常棒：表面本身并不重要，重要的只是它的边界是什么。

13. For example, imagine a particular loop through space, and think about all the different surfaces that could have this loop as a boundary; all the different soap bubbles which could emerge from this one loop:
    例如，想象一个特定的空间环，想想所有可能有这个环作为边界的不同表面；所有可能从这个环中出现的不同的肥皂泡。

14. For any given vector field $\mathbf{F}(x, y, z)$, the surface integral $\iint_S \operatorname{curl} \mathbf{F} \cdot \hat{\mathbf{n}} d \Sigma$ will be the same for each one of these surfaces. Isn't that crazy! These surface integrals involve adding up completely different values at completely different points in space, yet they turn out to be the same simply because they share a boundary.
    对于任何给定的矢量场$\mathbf{F}(x, y, z)$，表面积分$\iint_S \operatorname{curl} \mathbf{F} \cdot \hat{\mathbf{n}} d \Sigma$对于这些表面中的每一个都是相同的。这不是疯了吗！这些表面积分涉及在完全不同的空间点上加上完全不同的值，然而它们却因为共享一个边界而变得相同。

--- pic\Stokes' theorem.pdf_11.png ---

1. What this tells you is just how special curl vector fields are, since with most vector fields, the surface integral absolutely depends on the specific surface at hand. If you learned about conservative vector fields, this is analogous to path independence, and how it indicates just how special gradient vector fields are.
   这告诉你旋度矢量场有多么特殊，因为对于大多数矢量场，表面积分绝对依赖于手头的具体表面。如果你学过保守矢量场，这类似于路径独立性，以及它如何表明梯度矢量场有多么特殊。

2. What if there is no boundary?
   如果没有边界怎么办？

3. If you have a closed surface, like a sphere or a torus, then there is no boundary. This means the "line integral over the boundary" is zero, and Stokes' theorem reads as follows:
   如果你有一个封闭的表面，比如一个球体或一个圆环体，那么就没有边界。这意味着"边界上的线积分"是零，斯托克斯定理如下所示：
   $$
   \iint_S \operatorname{curl} \mathbf{F} \cdot \hat{\mathbf{n}} d \Sigma=0
   $$

4. If you think back to chopping up the surface to get many tiny little line integrals, this basically says all those little line integrals cancel out with nothing left to show for their work.
   如果你回想一下切割表面以获得许多微小的线积分，这基本上说所有那些小的线积分都抵消了，没有什么可以显示他们的工作。

5. Summary
   总结

6. Stokes' theorem is the 3D version of Green's theorem.
   斯托克斯定理是格林定理的3D版本。

1. Surface integral of a curl vector field
   曲面积分的旋度矢量场

2. $S$ is a surface in 3D
   $S$ 是一个三维的表面

3. Line integral around boundary of surface
   曲面边界的线积分

7. The line integral $\int_C \mathbf{F} \cdot d \mathbf{r}$ tells you how much a fluid flowing along $\mathbf{F}$ tends to circulate around the boundary $C$ of the surface $S$.
   线积分$\int_C \mathbf{F} \cdot d \mathbf{r}$告诉你沿着$\mathbf{F}$流动的流体倾向于在表面$S$的边界$C$周围循环多少。

8. The left-hand side surface integral can be seen as adding up all the little bits of fluid rotation on the surface $S$ itself. The vector curl $\mathbf{F}$ describes the fluid rotation at each point, and dotting it with a unit normal vector to the surface, $\hat{\mathbf{n}}$, extracts the component of that fluid rotation which happens on the surface itself.
   左侧的表面积分可以被看作是在表面$S$本身上累加所有的小流体旋转。矢量旋度$\mathbf{F}$描述了每个点的流体旋转，与表面的单位法向量$\hat{\mathbf{n}}$点乘，提取出在表面本身发生的流体旋转的分量。

--- pic\Stokes' theorem.pdf_12.png ---

$$
 \underbrace{\iint_S(\operatorname{curl} \mathbf{F} \cdot \hat{\mathbf{n}}) d \Sigma}=\underbrace{\int_C \mathbf{F} \cdot d \mathbf{r}}
$$

1. $\mathbf{F}(x, y, z)$ is a three-dimensional vector field.
   $\mathbf{F}(x, y, z)$是一个三维矢量场。

2.  $\operatorname{curl} \mathbf{F}$ means the same thing as $\nabla \times \mathbf{F}$. It is the three-dimensional curl of $\mathbf{F}$, which is a vector field.
    $\operatorname{curl} \mathbf{F}$与$\nabla \times \mathbf{F}$的含义相同。它是矢量场$\mathbf{F}$的三维旋度。

3.  $S$ is a surface in three dimensions.
    $S$是三维中的一个表面。

4.  $\hat{\mathbf{n}}$ represents a function that gives unit normal vectors to $S$.
    $\hat{\mathbf{n}}$表示一个给出$S$的单位法向量的函数。

5.  $C$ is the boundary of $S$
    $C$是$S$的边界

6.  $C$ is oriented using the right-hand rule, meaning if you point the thumb of your right hand in the direction of a unit normal vector $\hat{\mathbf{n}}$ near the edge of $S$ and curl your fingers, the direction they point indicates the direction you should integrate around $C$.
    $C$是使用右手规则定向的，意味着如果你将右手的拇指指向$S$边缘附近的单位法向量$\hat{\mathbf{n}}$的方向并卷曲你的手指，它们指向的方向指示了你应该围绕$C$积分的方向。





