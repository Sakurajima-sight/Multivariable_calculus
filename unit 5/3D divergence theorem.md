
--- pic\3D divergence theorem.pdf_00.png ---

1. 3D divergence theorem
   三维散度定理

2. Also known as Gauss's theorem, the divergence theorem is a tool for translating between surface integrals and triple integrals.
   也被称为高斯定理，散度定理是一个用于在表面积分和三重积分之间转换的工具。

3. Background
   背景

4. Flux in three dimensions
   三维的通量

5. Divergence
   散度

6. Triple integrals
   三重积分

7. 2D divergence theorem
   二维散度定理

8. Not strictly necessary, but useful for intuition:
   不是严格必要的，但对于直觉有用：

9. Formal definition of divergence in three dimensions
   三维散度的正式定义

10. What we're building to
    我们正在构建的是

11. Setup
    设置

12. $\mathbf{F}(x, y, z)$ is a three-dimensional vector field.
    $\mathbf{F}(x, y, z)$是一个三维矢量场。

13. $V$ is some three-dimensional volume (think of a blob floating in space).
    $V$是一些三维体积（想象一个在空间中漂浮的斑点）。

14. $S$ is the surface of $V$.
    $S$是$V$的表面。

15. The divergence theorem relates the divergence of $\mathbf{F}$ within the volume $V$ to the outward flux of $\mathbf{F}$ through the surface $S$.
    散度定理将体积$V$内的$\mathbf{F}$的散度与通过表面$S$的$\mathbf{F}$的外向通量联系起来。

--- pic\3D divergence theorem.pdf_01.png ---

1. The intuition here is that divergence measures the outward flow of a fluid at individual points, while the flux measures outward fluid flow from an entire region, so adding up the bits of divergence gives the same value as
flux. 
    这里的直觉是，散度测量了流体在单个点的外向流动，而通量测量了来自整个区域的外向流体流动，所以加起来的散度给出了与通量相同的值。

$$
\underbrace{\iiint_V \operatorname{div} \mathbf{F} d V}_{\begin{array}{c}
\text { 在 } V \text { 中加起小块的 } \\
\text { 外向流 }
\end{array}} = \overbrace{\underbrace{\iint_S \mathbf{F} \cdot \hat{\mathbf{n}} d \Sigma}_{\begin{array}{c}
\text { 测量通过 } V \text{'s 边界的总外向流 } \\
\end{array}}}^{\text { 流量积分 }}
$$

1.  Surface must be closed
    表面必须是封闭的

2.  In what follows, you will be thinking about a surface in space. But unlike, say, Stokes' theorem, the divergence theorem only applies to closed surfaces, meaning surfaces without a boundary. For example, a hemisphere is not a closed surface, it has a circle as its boundary, so you cannot apply the divergence theorem.
    在接下来的内容中，你将会思考空间中的一个表面。但是不像，比如说，斯托克斯定理，散度定理只适用于封闭的表面，也就是没有边界的表面。例如，半球不是一个封闭的表面，它有一个圆作为它的边界，所以你不能应用散度定理。

3.  However, if you add on the disk on the bottom of this hemisphere, and consider the disk and the hemisphere to make up a single surface, you now have a closed surfaces whose interior volume is half a ball.
    然而，如果你在这个半球的底部加上一个圆盘，并考虑圆盘和半球构成一个单一的表面，你现在有一个内部体积是半个球的封闭表面。


--- pic\3D divergence theorem.pdf_02.png ---

1. In this case, given some vector field, the divergence theorem can be used on this two-part surface and this half ball.
   在这种情况下，给定一些矢量场，可以在这个两部分的表面和这个半球上使用散度定理。

2. The reason for this is that we need to be able to talk about the three-dimensional volume enclosed by a surface, which doesn't make any sense for open surfaces.
   这样做的原因是我们需要能够讨论由表面包围的三维体积，这对于开放的表面没有任何意义。

3. The intuition
   直觉

4. If you understand the intuition behind flux in $3 \mathrm{~d}$, triple integrals, and the $2 \mathrm{~d}$ divergence theorem, you basically already understand the three-dimensional divergence theorem. It's just a matter of fitting these conceptual ideas together.
   如果你理解了$3 \mathrm{~d}$中通量、三重积分和$2 \mathrm{~d}$散度定理背后的直觉，你基本上已经理解了三维散度定理。这只是一个将这些概念性的想法组合在一起的问题。

5. Global view of outward flow: flux
   外流的全局视图：通量

1. When a three-dimensional vector field $\mathbf{F}(x, y, z)$ is thought of as representing a fluid flow, the flux of $\mathbf{F}$ through a surface $S$ is a measure of how much fluid passes through that surface per unit time. It is measured with the following integral:
   当三维向量场 $\mathbf{F}(x, y, z)$ 被视为表示流体流动时，$\mathbf{F}$ 通过表面 $S$ 的通量是一个度量单位时间内通过该表面的流体量。它用以下积分来衡量：

--- pic\3D divergence theorem.pdf_03.png ---

1. 
   $$
   \iint_S \mathbf{F} \cdot \hat{\mathbf{n}} d \Sigma
   $$

2. You can think of this integral as breaking apart the surface into many tiny pieces, where $d \Sigma$ represents the area of one of these pieces. That little hatted fellow $\hat{n}$ represents a function that gives a unit normal vector at each point on the surface.
   你可以把这个积分想象成把表面分解成许多小片，其中$d \Sigma$代表这些片中的一个的面积。那个小帽子的家伙$\hat{n}$代表一个函数，它在表面的每一点给出一个单位法向量。

3. When the dot product $\mathbf{F} \cdot \hat{\mathbf{n}}$ is large, it means the fluid is flowing strongly in the same direction as $\hat{\mathrm{n}}$, and hence the fluid is passing the surface rapidly at that point. Notice, this means the flux integral counts fluid flow positively when it goes in the same direction as the unit normal vectors $\hat{n}$, and negatively when it flows against those vectors.
   当点积$\mathbf{F} \cdot \hat{\mathbf{n}}$很大时，它意味着流体正在强烈地沿着$\hat{\mathrm{n}}$的同一方向流动，因此流体在那一点迅速地通过表面。注意，这意味着当流体流动的方向与单位法向量$\hat{n}$的方向相同时，通量积分正向计数流体流动，而当流体流动与这些向量相反时，通量积分负向计数。

4.  For this article, think about the case where $S$ is a closed surface, encapsulating some three-dimensional volume $V$. ("Closed" means it has no edges). If $S$ is oriented with outward facing unit normal vectors, the flux of $\mathrm{F}$ through $S$ measures how quickly fluid is leaving the volume $V$. It's like going to all the doors at the boundary of a region and adding up how much fluid leaves each one while subtracting how much fluid enters each one.
    对于这篇文章，考虑$S$是一个封闭的表面，包围着一些三维体积$V$的情况（"封闭"意味着它没有边缘）。如果$S$是以面向外的单位法向量定向的，那么$\mathrm{F}$通过$S$的通量就测量了流体离开体积$V$的速度。这就像去一个区域的边界的所有门，加上每个门离开的流体量，同时减去每个门进入的流体量。

    $$
    \iint_S \overbrace{\mathbf{F} \cdot \hat{\mathbf{n}}}^{\begin{array}{c}
    \text{流体的} \\
    \text{流入/流出量?}
    \end{array}} \underbrace{d \Sigma}_{\text{微小的面积元}}
    $$



5.  Local view of outward flow: Divergence
    外流的局部视图：散度

--- pic\3D divergence theorem.pdf_04.png ---

1. Divergence, in any dimensions, measures the tendency for fluid to flow away from each point in space. More specifically, if you take some point in space, $\left(x_0, y_0, z_0\right)$, and some tiny volume around that point $V_{\text {tiny }}$, the rate at which fluid flowing along the vector field $\mathbf{F}$ leaves this tiny region will be roughly equal to the following expression:
   在任何维度中，散度都衡量了流体从空间中的每一点流出的趋势。更具体地说，如果你取空间中的某一点$\left(x_0, y_0, z_0\right)$，和这一点周围的一些微小体积$V_{\text {tiny }}$，沿着矢量场$\mathbf{F}$流动的流体离开这个微小区域的速率将大致等于以下表达式：

    $$
    \underbrace{\left(\nabla \cdot \mathbf{F}\left(x_0, y_0, z_0\right) \right)}_{\text {散度 }} \overbrace{\left|V_{\text {tiny }}\right|}^   {\text {体积 } V_{\text {tiny }}}
    $$

2. In other words, divergence gives the outward flow rate per unit volume near a point. The reason it must be multiplied by volume before estimating an actual outward flow rate is that the divergence at a point is a number which doesn't care about the size of the volume you happen to be thinking about around that point. But the outward flow rates for smaller volumes will be smaller simply by virtue of the fact that there is less fluid in them to do the flowing.
   换句话说，散度给出了靠近点的单位体积的外流速率。在估计实际的外流速率之前必须乘以体积的原因是，点处的散度是一个不关心你恰好在考虑该点周围的体积大小的数。但是，对于较小的体积，外流速率将会更小，仅仅是因为它们中的流体较少。

3. Add up local view to get a global view
   将局部视图加起来得到全局视图

4. Next, to bring triple integrals into the game, think of the following process:
   接下来，为了引入三重积分，可以考虑以下过程：

5. Break up a three-dimensional volume $V$ into many tiny pieces (little three-dimensional crumbs).
   将三维体积 $V$ 分解成许多小块（小三维面包屑）。

6. Compute the divergence of $\mathbf{F}$ inside each piece.
   计算每一块内部的 $\mathbf{F}$ 的散度。

7. Multiply that value by the volume of the piece.
   将该值乘以该块的体积。

8. Add up what you get.
   加起你得到的结果。

9. This will give a sense of the "total outward flow" due to $\mathbf{F}$ throughout the entire volume $V$. But as I mentioned above, this quantity is also measured by the flux of $\mathbf{F}$ through the surface $S$ of $V$.
   这将给出由于 $\mathbf{F}$ 在整个体积 $V$ 中的 "总外向流" 的感觉。但是如我上面提到的，这个量也是通过 $V$ 的表面 $S$ 上的 $\mathbf{F}$ 的通量来测量的。

10. The process outlined above also describes the intuition for a triple integral:
   上述过程也描述了对三重积分的直觉：

   $$
   \iiint_V \overbrace{\nabla \cdot \mathbf{F}}^{\text {散度}} \underbrace{d V}_{\begin{array}{c}
   \text {微小的} \\
   \text {体积元}
   \end{array}}
   $$


11. Setting this equal to the flux of $\mathbf{F}$ through the surface of $V$, we get the divergence theorem.
   将这个设置为通过$V$的表面的$\mathbf{F}$的通量，我们得到散度定理。

$$
\underbrace{\iiint_V \operatorname{div} \mathbf{F} d V}_{\begin{array}{c}
\text { 在 } V \text { 中加起小块的 } \\
\text { 外向流 }
\end{array}} = \overbrace{\underbrace{\iint_S \mathbf{F} \cdot \hat{\mathbf{n}} d \Sigma}_{\begin{array}{c}
\text { 测量通过 } V \text{'s 边界的总外向流 } \\
\end{array}}}^{\text { 流量积分 }}
$$

--- pic\3D divergence theorem.pdf_05.png ---

1. Usefulness
   有用性

2.  Both surface integrals and triple integrals can be very nasty to compute. But the divergence theorem gives a tool for translating back and forth between them, and oftentimes it can help turn a particularly difficult surface integral into an easier volume integral. This is especially effective if the volume $V$ is some familiar shape, like a sphere, and if the divergence turns out to be a simple function.
    表面积分和三重积分都可能非常难以计算。但是散度定理提供了一个在它们之间来回转换的工具，而且往往可以帮助将特别困难的表面积分转化为更容易的体积积分。如果体积$V$是一些熟悉的形状，比如球，而且如果散度变成一个简单的函数，这将特别有效。

3.  You can practice with examples of using this theorem in the next article.
    你可以在下一篇文章中通过例子来练习使用这个定理。

4.  It is also a powerful theoretical tool, especially for physics. In electrodynamics, for example, it lets you express various fundamental rules like Gauss's law either in terms of divergence, or in terms of a surface integral. This can be very helpful conceptually. Sometimes a situation is easier to think about locally, e.g. what individual charges at individual points in space are generating an electric field. But other times you want a more global view, perhaps asking how an electric field passes through an entire surface.
    它也是一个强大的理论工具，特别是对于物理学。例如，在电动力学中，它让你可以用散度或者表面积分的形式来表达各种基本规则，比如高斯定律。这在概念上可以非常有帮助。有时候，局部的情况更容易思考，例如，空间中的各个点的单个电荷是如何产生电场的。但是其他时候，你可能想要一个更全局的视角，也许是询问电场如何穿过整个表面。

5.  Summary
 总结

1. The divergence theorem says that when you add up all the little bits of outward flow in a volume using a triple integral of divergence, it gives the total outward flow from that volume, as measured by the flux through its surface.
   散度定理表明，当你使用散度的三重积分将体积中所有的微小出流量相加时，它给出的是通过其表面的总出流量。

$$
\underbrace{\iiint_V \operatorname{div} \mathbf{F} d V}_{\begin{array}{c}
\text { 在 } V \text { 中加起小块的 } \\
\text { 外向流 }
\end{array}} = \overbrace{\underbrace{\iint_S \mathbf{F} \cdot \hat{\mathbf{n}} d \Sigma}_{\begin{array}{c}
\text { 测量通过 } V \text{'s 边界的总外向流 } \\
\end{array}}}^{\text { 流量积分 }}
$$




