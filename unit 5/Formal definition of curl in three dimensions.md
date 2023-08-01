
--- pic\Formal definition of curl in three dimensions.pdf_00.png ---
1. Formal definition of curl in three dimensions
三维旋度的正式定义

1. After learning how two-dimensional curl is defined, you are ready to learn about the formal definition of three-dimensional curl.
   在学习了如何定义二维旋度后，你就准备好学习三维旋度的正式定义了。

2. This is advanced, so be prepared to take things slowly.
   这是高级的，所以请准备慢慢来。

1. Background 
   背景

1. Curl in three dimensions
三维的旋度

2. Formal definition of curl in two dimensions.
   二维旋度的正式定义。

4. Understanding this article really does require these two prerequisites.
   理解这篇文章确实需要这两个先决条件。

5. The definition of curl in three dimensions has so many moving parts that having a solid mental grasp of the two-dimensional analogy, as well as the three-dimensional concept we are trying to capture, is crucial.
   三维旋度的定义有很多变化的部分，所以必须要对二维比喻以及我们试图捕捉的三维概念有一个坚实的理解。

6. In particular, if you did not just come from reading the article giving the formal definition of curl in two dimensions, I would highly recommend taking a quick look at it right now, even if you've seen it before, and even if it's just the summary.
   特别是，如果你不是刚刚读完关于二维旋度正式定义的文章，我强烈推荐你现在就快速看一下，即使你以前看过，即使只是总结。

7. What we're building to: We define three-dimensional curl one component at a time, looking at the components of fluid rotation which are parallel to the $xy$-plane, the $yz$ plane, and the $xz$-plane.
   我们正在构建的内容：我们一次定义一个三维旋度的组成部分，观察与$xy$平面，$yz$平面和$xz$平面平行的流体旋转的组成部分。

8. You can capture all three of these coordinate-by-coordinate definitions of curl $\nabla \times F$ by defining what the dot product between curl $\nabla \times F$ and any arbitrary unit vector $\hat{u}$ should be.
   你可以通过定义旋度$\nabla \times F$与任意单位向量$\hat{u}$的点积应该是什么，来捕捉到所有这三个坐标逐一定义的旋度。

--- pic\Formal definition of curl in three dimensions.pdf_01.png ---

1. $\mathbf{F}$ is a three-dimensional vector field.
   $\mathbf{F}$ 是一个三维向量场。

2. $(x, y, z)$ is some specific point in 3d space.
   $(x, y, z)$ 是三维空间中的某个特定点。

3. $\operatorname{curl} \mathbf{F}(x, y, z)$ returns a three-dimensional vector.
   $\operatorname{curl} \mathbf{F}(x, y, z)$ 返回一个三维向量。

4. $\hat{\mathbf{n}}$ is an arbitrary unit vector in three-dimensions.
   $\hat{\mathbf{n}}$ 是三维空间中的任意单位向量。

5. $A_{((x, y, z), \hat{\mathbf{n}})}$ represents some two-dimensional region around the point $(x, y, z)$ on a plane perpendicular to the vector $\hat{\mathbf{n}}$.
   $A_{((x, y, z), \hat{\mathbf{n}})}$ 表示在与向量 $\hat{\mathbf{n}}$ 垂直的平面上，围绕点 $(x, y, z)$ 的某个二维区域。

6. $\left|A_{((x, y, z), \hat{\mathbf{n}})}\right|$ indicates the area of $A_{((x, y, z), \hat{\mathbf{n}})}$.
   $\left|A_{((x, y, z), \hat{\mathbf{n}})}\right|$ 表示 $A_{((x, y, z), \hat{\mathbf{n}})}$ 的面积。

7. $\left|A_{((x, y, z), \hat{\mathbf{n}})}\right| \rightarrow 0$ indicates we are considering the limit as the area of $A_{((x, y, z), \hat{\mathbf{n}})}$ goes to zero, meaning that region shrinks around $(x, y, z)$.
   $\left|A_{((x, y, z), \hat{\mathbf{n}})}\right| \rightarrow 0$ 表示我们正在考虑 $A_{((x, y, z), \hat{\mathbf{n}})}$ 的面积趋向于零的极限，意味着该区域在 $(x, y, z)$ 周围收缩。

8. $C$ is the boundary of $A_{((x, y, z), \hat{\mathbf{n}})}$.
   $C$ 是 $A_{((x, y, z), \hat{\mathbf{n}})}$ 的边界。

9. The orientation of $C$ is determined based on the right-hand rule: Stick the thumb of your right hand in the direction of $\hat{\mathbf{n}}$, and the direction your fingers point as they wrap around $C$ is the direction of integration.
   $C$ 的方向是根据右手规则确定的：将你的右手的拇指指向 $\hat{\mathbf{n}}$ 的方向，然后你的手指包围 $C$ 指向的方向就是积分的方向。

10. $\oint_{C}$ is the line integral around $C$, written as $\oint$ instead of $\int$ to emphasize that $C$ is a closed curve.
    $\oint_{C}$ 是围绕 $C$ 的线积分，写作 $\oint$ 而不是 $\int$ 是为了强调 $C$ 是一个闭曲线。

1. Limit our view to one plane.
   将我们的视角限制在一个平面上。

12. Curl in three-dimensions is a rather complicated thing to think about.
    三维的旋度是一个相当复杂的概念。

13. For example, let $\mathbf{F}(x, y, z)$ be a three-dimensional vector field:

    $$\mathbf{F}(x, y, z)=\left[\begin{array}{c}
    F_{1}(x, y, z) \\
    F_{2}(x, y, z) \\
    F_{3}(x, y, z)
    \end{array}\right]$$
    
    例如，让 $\mathbf{F}(x, y, z)$ 是一个三维向量场：

    $$\mathbf{F}(x, y, z)=\left[\begin{array}{c}
    F_{1}(x, y, z) \\
    F_{2}(x, y, z) \\
    F_{3}(x, y, z)
    \end{array}\right]$$

14. An example of what this could look like is shown in the following video.
    下面的视频展示了这可能是什么样子的一个例子。

--- pic\Formal definition of curl in three dimensions.pdf_02.png ---
Example 3d vector field

1. Now imagine the three-dimensional fluid flow that $\mathbf{F}$ could represent.
   现在想象一下$\mathbf{F}$可能表示的三维流体流动。

2. As you know, $\operatorname{curl} \mathbf{F}\left(x_{0}, y_{0}, z_{0}\right)$ is a way to measure rotation in that fluid flow near the point $\left(x_{0}, y_{0}, z_{0}\right)$, but this is a tricky concept to quantify rigorously.
   如你所知，$\operatorname{curl} \mathbf{F}\left(x_{0}, y_{0}, z_{0}\right)$是一种在点$\left(x_{0}, y_{0}, z_{0}\right)$附近的流体流动中测量旋转的方法，但这是一个严谨量化的棘手概念。

3. There are some good analogies out there to gain an intuition for curl.
   有一些好的类比可以帮助我们对旋度有一个直观的理解。

4. One of my favorites is to think of a tiny tennis ball centered at the point $\left(x_{0}, y_{0}, z_{0}\right)$, and how the surrounding fluid flow would cause it to rotate.
   我最喜欢的一个是想象一个以点$\left(x_{0}, y_{0}, z_{0}\right)$为中心的小网球，以及周围的流体流动如何使它旋转。

5. In this analogy, $\operatorname{curl} \mathbf{F}\left(x_{0}, y_{0}, z_{0}\right)$ gives the vector of the tennis ball's resulting rotation.
   在这个类比中，$\operatorname{curl} \mathbf{F}\left(x_{0}, y_{0}, z_{0}\right)$给出了网球旋转的结果向量。

6. However, these descriptions can only go so far when the goal is to formally define what curl is; to capture this intuition with mathematical rigour.
   然而，当目标是正式定义旋度是什么时，这些描述只能到这里；要用数学的严谨性捕捉这种直观感觉。

7. Our basic strategy moving forward will be to limit our view to the rotation in a specific plane.
   我们向前的基本策略将是将我们的视角限制在特定平面中的旋转上。

1. For example, the following video shows a plane representing a constant $x$ value, $x=1.6$ to be specific, as well as the vectors from $\mathbf{F}$ which stem from this plane.
   例如，下面的视频显示了一个代表常数 $x$ 值的平面，具体来说，$x=1.6$，以及从这个平面发出的 $\mathbf{F}$ 的向量。

--- pic\Formal definition of curl in three dimensions.pdf_03.png ---

1. In formulas, you might describe this as all the vectors of the form $\mathbf{F}(1.6, y, z)$.
   在公式中，你可能会将其描述为所有形如$\mathbf{F}(1.6, y, z)$的向量。

2. Here, $y$ and $z$ range freely.
   这里，$y$和$z$的范围是自由的。

3. When we project those vectors onto the plane and lay it out flat as a picture, we'd get something like this.
   当我们将这些向量投影到平面上并平铺成一幅图时，我们将得到如下的东西。

4. Note, the axes are labeled "$y$" and "$z$" because this plane was originally parallel to the $yz$-plane in three-dimensional space.
   注意，轴标记为"$y$"和"$z$"，因为这个平面原本与三维空间中的$yz$-平面平行。

5. We could describe this two-dimensional vector field with a new two-dimensional function $\mathbf{F}_{1.6}(y, z)$ defined as follows: $\mathbf{F}_{1.6}(y, z)=\left[\begin{array}{c}F_{2}(1.6, y, z) \\ F_{3}(1.6, y, z)\end{array}\right]$.
   我们可以用一个新的二维函数$\mathbf{F}_{1.6}(y, z)$来描述这个二维向量场，定义如下：$\mathbf{F}_{1.6}(y, z)=\left[\begin{array}{c}F_{2}(1.6, y, z) \\ F_{3}(1.6, y, z)\end{array}\right]$。

6. More generally, if we slice the vector field with any plane of the form $x=x_{0}$ for some constant $x_{0}$, then project the vectors stemming from that plane onto the plane itself, we will get a two-dimensional vector field described by a function that looks like this: $\mathbf{F}_{x_{0}}(y, z)=\left[\begin{array}{c}F_{2}\left(x_{0}, y, z\right) \\ F_{3}\left(x_{0}, y, z\right)\end{array}\right]$.
   更一般地，如果我们用形如$x=x_{0}$的任何平面来切割向量场，其中$x_{0}$是某个常数，然后将源自该平面的向量投影到平面本身，我们将得到一个由如下函数描述的二维向量场：$\mathbf{F}_{x_{0}}(y, z)=\left[\begin{array}{c}F_{2}\left(x_{0}, y, z\right) \\ F_{3}\left(x_{0}, y, z\right)\end{array}\right]$。

--- pic\Formal definition of curl in three dimensions.pdf_04.png ---
1. Concept check: Why does the definition of $\mathbf{F}_{x_{0}}(y, z)$ not include $F_{1}$, the $x$ component of $\mathbf{F}(x, y, z)$?
   概念检查：为什么$\mathbf{F}_{x_{0}}(y, z)$的定义不包括$F_{1}$，即$\mathbf{F}(x, y, z)$的$x$分量？

2. Choose 1 answer:
   选择一个答案：

3. Because it represents the projection of vectors $\mathbf{F}\left(x_{0}, y, z\right)$ onto a plane parallel to the $y z$-plane, and that projection involves ignoring the $F_{1}$ component.
   因为它表示向量$\mathbf{F}\left(x_{0}, y, z\right)$投影到平行于$y z$平面的平面上，这种投影涉及到忽略$F_{1}$分量。

4. This first answer is correct.
   第一个答案是正确的。

5. Leaving off the first coordinate of a three-dimensional vector corresponds to projecting it onto the $y z$-plane.
   省略三维向量的第一坐标相当于将其投影到$y z$平面上。

6. The fact that only $y$ and $z$ vary indicates that $\mathbf{F}_{x{0}}$ is a function on the $y z$-plane, but says nothing about how the output of that function should look.
只有 $y$ 和 $z$ 变化，这表明 $\mathbf{F}_{x{0}}$ 是 $y z$ 平面上的函数，但并没有说明该函数的输出应该是什么样的。

7. Concept check: For a given point $\left(y_{0}, z_{0}\right)$ in the plane above, what does $2 \mathrm{~d}$-curl $\mathbf{F}_{x_{0}}\left(y_{0}, z_{0}\right)$ represent?
   概念检查：对于上面平面上的一个给定点$\left(y_{0}, z_{0}\right)$，$2 \mathrm{~d}$-curl $\mathbf{F}_{x_{0}}\left(y_{0}, z_{0}\right)$表示什么？

8. Choose all answers that apply:
   选择所有适用的答案：

9. How much the fluid flow defined by $\mathbf{F}$ rotates parallel to the $y z$ -plane near the point $\left(x_{0}, y_{0}, z_{0}\right)$
流体流动由 $\mathbf{F}$ 定义，其在点 $\left(x_{0}, y_{0}, z_{0}\right)$ 附近平行于 $y z$ 平面的旋转程度。

10. The $x$-component of $\operatorname{curl} \mathbf{F}\left(x_{0}, y_{0}, z_{0}\right)$
    $\operatorname{curl} \mathbf{F}\left(x_{0}, y_{0}, z_{0}\right)$的$x$-分量


--- pic\Formal definition of curl in three dimensions.pdf_05.png ---
1. Both answers are correct. In fact, they are two ways of saying the same thing.
   两个答案都是正确的。事实上，他们是表达同一件事的两种方式。

2. $\mathbf{F}_{x_{0}}$ takes vectors from $\mathbf{F}$ stemming from points in the plane $x=x_{0}$, and projects them onto that same plane.
   $\mathbf{F}_{x_{0}}$从平面$x=x_{0}$中的点出发，取$\mathbf{F}$中的向量，并将它们投影到同一平面上。

3. In terms of fluid flow, this means if you follow the three-dimensional motion of particles starting in the plane $x=x_{0}$ according to the velocity vectors given by $\mathbf{F}$, then project those trajectories onto the plane $x=x_{0}$, you get the twodimensional fluid motion described by $\mathbf{F}_{x_{0}}$.
   在流体流动方面，这意味着，如果你按照$\mathbf{F}$给出的速度向量追踪起始于平面$x=x_{0}$的粒子的三维运动，然后将这些轨迹投影到平面$x=x_{0}$上，你将得到由$\mathbf{F}_{x_{0}}$描述的二维流体运动。

4. So what does this mean for $2 \mathrm{~d}$-curl $\mathbf{F}_{x_{0}}$, which measures the rotation in the two-dimensional fluid flow defined by $\mathbf{F}_{x_{0}}$ ?
   那么，对于$2 \mathrm{~d}$-curl $\mathbf{F}_{x_{0}}$，这是什么意思呢？它衡量的是由$\mathbf{F}_{x_{0}}$定义的二维流体流动中的旋转。

5. It measures the extent to which the three-dimensional fluid flow described by $\mathbf{F}$ rotates in the plane $x=x_{0}$.
   它测量了由$\mathbf{F}$描述的三维流体流动在平面$x=x_{0}$中的旋转程度。

6. You could aptly describe this as the component of threedimensional rotation which is parallel to the $y z$-plane.
   你可以适当地将此描述为与$y z$-平面平行的三维旋转的分量。

7. On the other hand, since the vector $\operatorname{curl} \mathbf{F}\left(x_{0}, y_{0}, z_{0}\right)$ represents the total three-dimensional rotation near $\left(x_{0}, y_{0}, z_{0}\right)$, the component of this vector pointing in the $x$-direction also represents the component of fluid rotation which is parallel to the $y z$-plane.
   另一方面，由于向量$\operatorname{curl} \mathbf{F}\left(x_{0}, y_{0}, z_{0}\right)$代表了在$\left(x_{0}, y_{0}, z_{0}\right)$附近的总的三维旋转，这个向量在$x$方向的分量也代表了与$y z$-平面平行的流体旋转的分量。

1. A component-wise definition
   以分量为基础的定义

8. So why am I talking about projecting vectors and trajectories in three dimensions onto a two-dimensional plane? Basically, it's hard to think about three dimensions, so it's worth doing everything you can to frame things twodimensions at a time.
   那么，我为什么要讨论将三维向量和轨迹投影到二维平面上呢？基本上，想象三维是困难的，所以尽可能地一次考虑两个维度是值得的。

9. The importance of this last concept check is that we can describe the $x$ component of the three-dimensional curl of $\mathbf{F}$ purely in terms of the twodimensional curl of the function $\mathbf{F}_{x}$ :
   这最后一个概念检查的重要性在于，我们可以完全用函数$\mathbf{F}_{x}$的二维旋度来描述$\mathbf{F}$的三维旋度的$x$分量：

10. 
   $$
   x \text {-component of } \underbrace{\operatorname{curl} \mathbf{F}(x, y, z)}_{3d \text { vector }}=\underbrace{2 \mathrm{~d}-\operatorname{curl} \mathbf{F}_{x}(y, z)}_{\text {Scalar value }}
   $$

11. We can also more elegantly pull out the $x$-component of curl $\mathbf{F}$ by dotting it with the unit vector in the $x$-direction,
   我们还可以通过将$\mathbf{F}$的旋度与$x$方向的单位向量点乘，更优雅地提取出$x$-分量，

12.
   $$
   \hat{\mathbf{i}}=\left[\begin{array}{l}
   1 \\
   0 \\
   0
   \end{array}\right]
   $$

--- pic\Formal definition of curl in three dimensions.pdf_06.png ---
1. This means our expression looks like this:

   $$
   (\operatorname{curl} \mathbf{F}(x, y, z)) \cdot \hat{\mathbf{i}}=2 \mathrm{~d}-\operatorname{curl} \mathbf{F}_{x}(y, z)
   $$

   这意味着我们的表达式看起来是这样的：

   $$
   (\operatorname{curl} \mathbf{F}(x, y, z)) \cdot \hat{\mathbf{i}}=2 \mathrm{~d}-\operatorname{curl} \mathbf{F}_{x}(y, z)
   $$

2. In terms of the formula you already know, this explains why the $x$-component of curl $\mathbf{F}$ has the form that it does,
   就你已经知道的公式而言，这解释了旋度$\mathbf{F}$的$x$分量为何具有它所具有的形式，

3. But remember, the whole point of this article is that curl is one of those funny operations where the formula we use to compute it is not its definition.
   但是请记住，这篇文章的重点是旋度是那些有趣的操作之一，我们用来计算它的公式并不是它的定义。

4. Our goal is to find a definition of curl by directly representing fluid rotation. With that in mind, the significance of representing the $x$-component of $\operatorname{curl} \mathbf{F}$ using a two-dimensional curl is that we can take the line-integral-limit definition of $2 \mathrm{~d}$-curl found in the last article, and use it to define the $x$-component of curl $\mathbf{F}$.
   我们的目标是通过直接表示流体旋转来找到旋度的定义。考虑到这一点，用二维旋度表示$\operatorname{curl} \mathbf{F}$的$x$分量的重要性在于，我们可以采用上一篇文章中找到的$2 \mathrm{~d}$-旋度的线积分极限定义，并用它来定义旋度$\mathbf{F}$的$x$分量。

5. $$
   (\operatorname{curl} \mathbf{F}(x, y, z)) \cdot \hat{\mathbf{i}} \overbrace{=}^{\text {definition }} \lim _{A \rightarrow 0}\left(\frac{1}{|A|} \oint_{C} \mathbf{F} \cdot d \mathbf{r}\right)
   $$

   $$
   (\operatorname{curl} \mathbf{F}(x, y, z)) \cdot \hat{\mathbf{i}} \overbrace{=}^{\text {definition }} \lim _{A \rightarrow 0}\left(\frac{1}{|A|} \oint_{C} \mathbf{F} \cdot d \mathbf{r}\right)
   $$

6. $A$ is some two-dimensional region in the plane perpendicular to $\hat{\mathbf{i}}$, and passing through the point $(x, y, z)$.
   $A$是平面上的某个二维区域，垂直于$\hat{\mathbf{i}}$，并通过点$(x, y, z)$。

7. $C$ is the boundary of $A$.
   $C$是$A$的边界。

8. The orientation of $C$ is determined based on the right-hand rule: Stick the thumb of your right hand in the direction of $\hat{\mathbf{i}}$, and curl your fingers. The direction your fingers point as they wrap around $C$ is the direction of integration.
   $C$的方向是基于右手规则确定的：将你的右手的拇指指向$\hat{\mathbf{i}}$的方向，然后卷曲你的手指。你的手指包围$C$时所指的方向是积分的方向。

9. $|A|$ represents the area of $A$.
   $|A|$表示$A$的面积。

10. $\lim _{|A| \rightarrow 0}$ indicates that we are considering the limit as $A$ shrinks to the point $(x, y, z)$ on the plane where $x$ is constant. 
    $\lim _{|A| \rightarrow 0}$表明我们正在考虑当$A$缩小到平面上$x$为常数的点$(x, y, z)$时的极限。

--- pic\Formal definition of curl in three dimensions.pdf_07.png ---
1. Although it will clutter things up, for clarity's sake it will help if our formula expresses the fact that the region $A$ must always include the point $(x, y, z)$, and that it is perpendicular to $\hat{\mathbf{i}}$. To do this, I'll write $A$ with subscripts, $A_{(x, y, z), \hat{\mathrm{i}}}$.
   虽然这会使事情变得混乱，但为了清晰起见，如果我们的公式能够表达出区域$A$必须始终包含点$(x, y, z)$，并且它垂直于$\hat{\mathbf{i}}$，这将有所帮助。为此，我将用下标来写$A$，即$A_{(x, y, z), \hat{\mathrm{i}}}$。

2. This means our full definition looks like this:
   这意味着我们的完整定义如下：

   $$
   (\operatorname{curl} \mathbf{F}(x, y, z)) \cdot \hat{\mathbf{i}} \overbrace{=}^{\text {definition }} \lim _{\left|A_{((x, y, z), \hat{\mathbf{i}})}\right| \rightarrow 0}\left(\frac{1}{\left|A_{((x, y, z), \hat{\mathbf{i}})}\right|} \oint_{C} \mathbf{F} \cdot d \mathbf{r}\right)
   $$

1. Full definition
   完整定义

3. This is a very heavy definition, which assumes a lot of prior knowledge from the reader. And that's just for one component! The key to understanding this is to:
   这是一个非常重的定义，它假定读者有很多先验知识。而这只是一个组件！理解这一点的关键是：

4. Make sure you have a full grasp of the definition of curl in two-dimensions.
   确保你完全理解了二维旋度的定义。

5. Understand how this definition is applying that same concept to a plane sitting in three-dimensional space.
   理解这个定义是如何将同样的概念应用到位于三维空间中的平面上的。

6. Make sure you understand why two-dimensional curl of $\mathbf{F}_{x_{0}}$ should represent the $x$-component of the curl of $\mathbf{F}$.
   确保你理解为什么$\mathbf{F}_{x_{0}}$的二维旋度应该表示$\mathbf{F}$的旋度的$x$-分量。

7. There is of course nothing special about the $x$-direction, we can also define the other two coordinates of curl $\mathbf{F}$ similarly:
   当然，$x$-方向没有什么特别的，我们也可以以类似的方式定义旋度$\mathbf{F}$的另外两个坐标：

   $$
   \begin{aligned}
   & (\operatorname{curl} \mathbf{F}(x, y, z)) \cdot \hat{\mathbf{j}}=\lim _{\left|A_{((x, y, z), \hat{\jmath})}\right| \rightarrow 0}\left(\frac{1}{\left|A_{((x, y, z), \hat{\mathbf{j}})}\right|} \oint_{C} \mathbf{F} \cdot d \mathbf{r}\right) \\
   & (\operatorname{curl} \mathbf{F}(x, y, z)) \cdot \hat{\mathbf{k}}=\lim _{\left|A_{((x, y, z), \hat{\mathbf{k}})}\right| \rightarrow 0}\left(\frac{1}{\left|A_{((x, y, z), \hat{\mathbf{k}})}\right|} \oint_{C} \mathbf{F} \cdot d \mathbf{r}\right)
   \end{aligned}
   $$

8. Concept check: What does $A_{((x, y, z), \hat{\mathbf{j}})}$ represent?
   概念检查：$A_{((x, y, z), \hat{\mathbf{j}})}$表示什么？

1. A region in the plane passing through the point $(x, y, z)$ which is parallel to the $x z$-plane.
  通过点$(x, y, z)$并与$x z$平面平行的平面中的区域。


--- pic\Formal definition of curl in three dimensions.pdf_08.png ---
1. $A_{((x, y, z), \hat{\mathbf{j}})}$ represents a region in the plane passing through the point $(x, y, z)$ which is perpendicular to $\hat{\mathbf{j}}$. 
   $A_{((x, y, z), \hat{\mathbf{j}})}$代表通过点$(x, y, z)$且垂直于$\hat{\mathbf{j}}$的平面中的一个区域。

2. The plane perpedicular to $\hat{\mathbf{j}}$ is parallel to the $x z$-plane.
   垂直于$\hat{\mathbf{j}}$的平面与$xz$-平面平行。

3. This gives a full definition, since each component of curl $\mathbf{F}$ is accounted for.
   这给出了完整的定义，因为包含了旋度$\mathbf{F}$的每个分量。

1. Arbitrary unit normal vectors
   任意单位法向量

4. However, it is a little inelegant to define curl with three separate formulas. 
   然而，用三个单独的公式来定义旋度有点不够优雅。

5. Also, when curl is used in practice, it is common to find yourself taking the dot product between the vector curl $\mathbf{F}$ and some other vector, so it is handy to have a definition suited to interpreting the dot product between curl $\mathbf{F}$ and any vector, not just $\hat{\mathbf{i}}, \hat{\mathbf{j}}$ and $\hat{\mathbf{k}}$.
   另外，当实际使用旋度时，常常会发现自己需要计算旋度$\mathbf{F}$与其他某个向量之间的点积，所以有一个能适用于解释旋度$\mathbf{F}$与任何向量（不仅仅是$\hat{\mathbf{i}}, \hat{\mathbf{j}}$和$\hat{\mathbf{k}}$）之间的点积的定义会很方便。

2. Think about an arbitrary plane cutting through the vector field $\mathbf{F}(x, y, z)$.
   想象一个任意平面穿过向量场 $\mathbf{F}(x, y, z)$。

7. Suppose that this plane is defined to be perpendicular to some unit vector $\hat{\mathbf{n}}$, such as
   假设这个平面被定义为垂直于某个单位向量$\hat{\mathbf{n}}$，比如


--- pic\Formal definition of curl in three dimensions.pdf_09.png ---
1. Now imagine mimicking everything we did before with the plane $x=x_{0}$.
   现在想象一下，模仿我们之前在平面$x=x_{0}$上所做的所有事情。

2. Considering the vectors which stem from points on this plane.
   考虑起源于这个平面上的点的向量。

3. Project them onto the plane.
   将它们投影到平面上。

4. Measure the resulting two-dimensional curl on that plane.
   测量在那个平面上产生的二维旋度。

5. This will let us define the component of three-dimensional curl in the $\hat{\mathbf{n}}$ direction:
   这将使我们能够定义三维旋度在$\hat{\mathbf{n}}$方向上的分量：
   
6. $(\operatorname{curl} \mathbf{F}(x, y, z)) \cdot \hat{\mathbf{n}}=\lim _{\left|A_{((x, y, z), \hat{\mathbf{n}})}\right| \rightarrow 0}\left(\frac{1}{\left|A_{((x, y, z), \hat{\mathbf{n}})}\right|} \oint_{C} \mathbf{F} \cdot d \mathbf{r}\right)$


1. $\mathbf{F}$ is a three-dimensional vector field.
   $\mathbf{F}$是一个三维向量场。

2. $(x, y, z)$ is some specific point in 3d space.
   $(x, y, z)$是三维空间中的某个特定点。

3. $\operatorname{curl} \mathbf{F}(x, y, z)$ returns a three-dimensional vector.
   $\operatorname{curl} \mathbf{F}(x, y, z)$返回一个三维向量。

4.  $\hat{\mathbf{n}}$ is an arbitrary unit vector in three-dimensions.
    $\hat{\mathbf{n}}$是三维空间中的任意单位向量。

5.  $A_{((x, y, z), \hat{\mathbf{n}})}$ represents some two-dimensional region around the point $(x, y, z)$ on a plane perpendicular to the vector $\hat{\mathbf{n}}$.
    $A_{((x, y, z), \hat{\mathbf{n}})}$表示向量$\hat{\mathbf{n}}$垂直的平面上点$(x, y, z)$周围的一些二维区域。

6.  $\left|A_{((x, y, z), \hat{\mathbf{n}})}\right|$ indicates the area of $A_{((x, y, z), \hat{\mathbf{n}})}$.
    $\left|A_{((x, y, z), \hat{\mathbf{n}})}\right|$表示$A_{((x, y, z), \hat{\mathbf{n}})}$的面积。

7.  $\left|A_{((x, y, z), \hat{\mathbf{n}})}\right| \rightarrow 0$ indicates we are considering the limit as the area of $A_{((x, y, z), \hat{\mathbf{n}})}$ goes to zero, meaning that region shrinks around $(x, y, z)$.
    $\left|A_{((x, y, z), \hat{\mathbf{n}})}\right| \rightarrow 0$表示我们正在考虑$A_{((x, y, z), \hat{\mathbf{n}})}$的面积趋近于零的极限，这意味着该区域在$(x, y, z)$周围收缩。

8.  $C$ is the boundary of $A_{((x, y, z), \hat{\mathbf{n}})}$.
    $C$是$A_{((x, y, z), \hat{\mathbf{n}})}$的边界。

9.  The orientation of $C$ is determined based on the right-hand rule: Stick the thumb of your right hand in the direction of $\hat{\mathbf{n}}$, and the direction your fingers point as they wrap around $C$ is the direction of integration.
    $C$的方向是根据右手规则确定的：将你的右手的拇指指向$\hat{\mathbf{n}}$的方向，当你的手指包围$C$时，它们所指的方向就是积分的方向。

10. $\oint_{C}$ is the line integral around $C$, written as $\oint$ instead of $\int$ to emphasize that $C$ is a closed curve.
    $\oint_{C}$是$C$周围的线积分，写为$\oint$而不是$\int$，以强调$C$是一个闭合的曲线。

--- pic\Formal definition of curl in three dimensions.pdf_10.png ---

1. This is the definition of curl that you might come across in other texts. It's a weird definition, since instead of defining the vector curl $\mathbf{F}$ itself, it only defines what the dot product between this vector and anything else would be.
   这是你可能在其他文本中遇到的旋度定义。这是一个奇怪的定义，因为它没有定义旋度向量$\mathbf{F}$本身，而只定义了这个向量和其他任何东西之间的点积会是什么。

2. But here's why it kind of makes sense to do things this way, even if it feels convoluted: Rotation is an inherently two-dimensional idea, and when we try to talk about rotation in three dimensions (e.g. rotation of the earth) we are somewhat awkwardly forced to use vectors.
   但是这就是为什么即使感觉复杂，这样做仍然有点意义：旋转是一个本质上的二维概念，当我们试图谈论三维中的旋转（例如地球的旋转）时，我们有些尴尬地被迫使用向量。

3. A given rotation vector is saying "the rotation is really happening in some two-dimensional plane, and I'm just telling you what plane that is."
   给定的旋转向量是在说：“旋转真的发生在某个二维平面中，我只是告诉你那是哪个平面。”

4. When it comes to fluid rotation, what we really want is a way of taking any possible rotation vector (which is the same as saying any possible plane in which rotation occurs), and asking "how much does the fluid rotation near a given point look like this vector?" The curl gives us a way to answer this question.
   当涉及到流体旋转时，我们真正想要的是一种获取任何可能的旋转向量（也就是说，旋转发生的任何可能的平面）的方法，并询问“在给定点附近的流体旋转看起来像这个向量多少？”旋度给了我们一个回答这个问题的方法。

5. For a given vector, representing some rotation, when you dot that vector against the curl of a fluid flow, it tells you how much the fluid rotation resembles the rotation represented by that vector.
   对于表示某种旋转的给定向量，当你将该向量点乘流体流动的旋度时，它会告诉你流体旋转有多少类似于该向量所表示的旋转。

6. Summary
   总结

7. To define curl in three dimensions, we take it two dimensions at a time. Project the fluid flow onto a single plane and measure the twodimensional curl in that plane.
   要在三维中定义旋度，我们每次处理两个维度。将流体流动投影到一个平面上，并在该平面中测量二维的旋度。

8. Using the formal definition of curl in two dimensions, this gives us a way to define each component of three-dimensional curl. For example, the $x$ component is defined like this:
   使用二维中旋度的正式定义，这给了我们定义三维旋度每个分量的方法。例如，$x$分量的定义如下：

9.  $
   (\operatorname{curl} \mathbf{F}(x, y, z)) \cdot \hat{\mathbf{i}} \overbrace{=}^{\text {definition }} \lim _{\left|A_{((x, y, z), \hat{i})}\right| \rightarrow 0}\left(\frac{1}{\left|A_{((x, y, z), \hat{\mathbf{i}})}\right|} \oint_{C} \mathbf{F} \cdot d \mathbf{r}\right)
   $

10. You can replace $\hat{i}$ with any unit vector, thus defining what the component of curl $\mathbf{F}$ should be in any direction.
    你可以用任何单位向量替换$\hat{i}$，从而定义在任何方向上旋度$\mathbf{F}$的分量应该是什么。

11. Understanding this complicated definition fully is a sign that you have fully grasped both curl and line integrals, each of which are formidable concepts in their own right.
    充分理解这个复杂的定义是一个信号，表明你已经充分掌握了旋度和线积分，每一种都是非常强大的概念。

--- pic\Formal definition of curl in three dimensions.pdf_11.png ---
1. Also, this definition will prepare you very well for understanding Stokes' theorem, a topic which stands at the very pinnacle of multivariable calculus.
   此外，这个定义将很好地为你理解斯托克斯定理做准备，这是一个位于多变量微积分顶峰的话题。

