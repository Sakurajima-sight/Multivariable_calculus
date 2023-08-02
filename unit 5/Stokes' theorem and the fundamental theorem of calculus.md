
--- pic\Stokes' theorem and the fundamental theorem of calculus.pdf_00.png ---

1. Stokes' theorem and the fundamental theorem of calculus
   斯托克斯定理和微积分的基本定理

2. Both Green's theorem and Stokes' theorem are higher-dimensional versions of the fundamental theorem of calculus, see how!
   格林定理和斯托克斯定理都是微积分基本定理的高维版本，看看如何！

3. Background
   背景

4. Fundamental theorem of calculus (video)
   微积分基本定理（视频）

5. Green's theorem
   格林定理

6. Stokes' theorem
   斯托克斯定理

7. What we're building to
   我们正在构建的是

8. Both Green's theorem and Stokes' theorem, as well as several other multivariable calculus results, are really just higher dimensional analogs of the fundamental theorem of calculus.
   格林定理和斯托克斯定理，以及其他一些多元微积分的结果，实际上只是微积分基本定理的高维类比。

9. Quick review of the fundamental theorem of calculus
   对微积分基本定理的快速回顾

10. Remember the fundamental theorem of calculus? Here's what it says:
    记得微积分的基本定理吗？这就是它的内容：
    $$
    \int_a^b f^{\prime}(x)=f(b)-f(a)
    $$

--- pic\Stokes' theorem and the fundamental theorem of calculus.pdf_01.png ---

1. In other words, when you integrate the derivative of a function on a region $[a, b]$ of the number line, it's the same as evaluating the function itself on the boundary of that region, meaning the numbers $a$ and $b$, and taking the difference.
    换句话说，当你在数轴的一个区域$[a, b]$上积分一个函数的导数时，它等同于在该区域的边界上评估函数本身，也就是数字$a$和$b$，并取差值。

12. Green's theorem
    格林定理

13. Green's theorem can be seen as completely analogous to the fundamental theorem, but for two dimensions.
    格林定理可以被看作是与基本定理完全类似，但是对于二维。
    $$
    \iint_R 2 \mathrm{~d}-\operatorname{curl} \mathbf{F} d A=\oint_C \mathbf{F} \cdot d \mathbf{r}
    $$

14. Instead of taking the derivative of a single-variable function $f$, it involves the $2 \mathrm{~d}$-curl of a twovariable vector-valued function $\mathbf{F}(x, y)$.
    它不是取单变量函数$f$的导数，而是涉及到双变量向量值函数$\mathbf{F}(x, y)$的$2 \mathrm{~d}$-旋度。

15. Instead of integrating this over a region $[a, b]$ of the number line, take its double integral over a region $R$ of the $x y$-plane.
    它不是在数轴的一个区域$[a, b]$上积分，而是在$x y$平面的一个区域$R$上取它的双重积分。

16. The boundary of the one-dimensional range $[a, b]$ is just the pair of points $a$ and $b$. But because $R$ is two-dimensional, its boundary is a curve $C$.
    一维范围$[a, b]$的边界只是点$a$和$b$的一对。但是因为$R$是二维的，所以它的边界是一个曲线$C$。

17. Instead of evaluating $f$ at the two boundary points $a$ and $b$ and taking the difference, take the line integral of $\mathbf{F}$ around the boundary $C$ oriented counterclockwise.
    不是在两个边界点$a$和$b$处评估$f$并取差值，而是取$\mathbf{F}$在逆时针方向的边界$C$周围的线积分。

18. The underlying idea here is that when you integrate the "derivative" of a thing over a region, the value only depends on the value of that thing on the boundary of the region. It's just that in two dimensions, the relevant notion of a derivative is $2 \mathrm{~d}$-curl, and the boundary of a region involves an entire curve rather than a pair of points.
    这里的基本思想是，当你在一个区域上积分一个东西的"导数"时，值只依赖于该区域边界上那个东西的值。只是在二维中，导数的相关概念是$2 \mathrm{~d}$-旋度，而一个区域的边界涉及到一个完整的曲线，而不是一对点。

19. Stoke's theorem
    斯托克斯定理

20. Stokes' theorem takes this to three dimensions. Instead of just thinking of a flat region $R$ on the $x y$-plane, you think of a surface $S$ living in space. This time, let $C$ represent the boundary to this surface.
    斯托克斯定理将这个推广到三维。你不仅仅是想象在$x y$平面上的一个平面区域$R$，而是想象一个生活在空间中的表面$S$。这次，让$C$代表这个表面的边界。


--- pic\Stokes' theorem and the fundamental theorem of calculus.pdf_02.png ---

1. $$
   \iint_S \operatorname{curl} \mathbf{F} \cdot \hat{\mathbf{n}} d \Sigma=\oint_C \mathbf{F} \cdot d \mathbf{r}
   $$


2. Instead of a single variable function $f$, or a two-dimensional vector field, $\mathbf{F}(x, y, z)$ is a three-dimensional vector field.
   与单变量函数$f$或二维矢量场不同，$\mathbf{F}(x, y, z)$是一个三维矢量场。

3. Instead of taking the derivative $f^{\prime}(x)$, or the 2 d-curl, take the full-blown three-dimensional curl of $\mathrm{F}$.
   不是取导数$f^{\prime}(x)$或2d旋度，而是取$\mathrm{F}$的完全三维旋度。

4. Instead of taking the single integral over an interval $[a, b]$, or a double integral in a two-dimensional region, take the surface integral over $S$ in three-dimensions. Taking the surface integral of a vector field involves dotting that vector field with unit normal vectors.
   不是在区间$[a, b]$上取单重积分，或在二维区域内取双重积分，而是在三维中取$S$上的表面积分。对矢量场取表面积分涉及将该矢量场与单位法向量点乘。

5. On the right-hand side, instead of writing $f(b)-f(a)$, which involves evaluating $f$ on the boundary of the interval $[a, b]$ and taking the difference, we have the line integral of our function $\mathrm{F}$ around the boundary $C$ of the surface $S$, just as we did for Green's theorem.
   在右侧，不是写$f(b)-f(a)$，这涉及在区间$[a, b]$的边界上评估$f$并取差值，我们有围绕表面$S$的边界$C$的函数$\mathrm{F}$的线积分，就像我们对格林定理所做的那样。

6. More generalizations
   更多泛化

7. The divergence theorem, covered in just a bit, is yet another version of this phenomenon. It relates the triple integral of the divergence of a threedimensional vector field in a three-dimensional volume to the surface integral of that vector field on the boundary of that volume.
   散度定理是这一现象的另一个版本。它将三维矢量场在三维体积中的散度的三重积分与该矢量场在该体积边界上的表面积分关联起来。

--- pic\Stokes' theorem and the fundamental theorem of calculus.pdf_03.png ---

1. The fundamental theorem of line integrals also falls under the same overarching principle, relating the line integral of the gradient of a function to the values of that function on the bounds of the line.
   线积分的基本定理也符合同样的总体原则，将函数的梯度的线积分与该函数在线的边界上的值关联起来。

9. In general, it seems that the universe is trying to tell us that when you integrate the "derivative" of a function within a region, where the type of integration/derivative/region/function involved might be multidimensional, you get something that just depends on the value of that function on the boundary of that region. I think this is just one of the most beautiful things in math.
   一般来说，宇宙似乎在告诉我们，当你在一个区域内积分一个函数的“导数”，其中涉及的积分/导数/区域/函数的类型可能是多维的，你得到的东西只取决于该函数在该区域边界上的值。我认为这是数学中最美丽的事物之一。

10. The generalized Stokes' theorem
    广义斯托克斯定理

11. In case you are curious, pure mathematics does have a deeper theorem which captures all these theorems (and more) in a very compact formula. It is called the generalized Stokes' theorem. The language to describe it is a bit technical, involving the ideas of "differential forms" and "manifolds", so I won't go into it here. But if you understand all the examples above, you already understand the underlying intuition and beauty of this unifying theorem.
    如果你感到好奇，纯数学确实有一个更深层次的定理，它以非常紧凑的公式捕捉了所有这些定理（以及更多）。它被称为广义斯托克斯定理。描述它的语言有点技术性，涉及“微分形式”和“流形”的概念，所以我不会在这里深入讨论。但是，如果你理解了上面的所有示例，你已经理解了这个统一定理的基本直觉和美感。