

--- pic\Flux in three dimensions.pdf_00.png ---

1. Flux in three dimensions
   三维的通量

2. Also known as a surface integral in a vector field, three-dimensional flux measures of how much a fluid flows through a given surface.
   也被称为向量场中的表面积分，三维通量测量了多少流体通过给定的表面流动。

3. Background
   背景

4. Vector fields
   向量场

5. Surface integrals
   表面积分

6. Unit normal vector of a surface
   表面的单位法向量

7. Not strictly required, but useful for analogy: Two-dimensional flux
   不是严格要求，但对于类比有用：二维通量

8. What we are building to
   我们要构建的是

9. When you have a fluid flowing in three-dimensional space, and a surface sitting in that space, the flux through that surface is a measure of the rate at which fluid is flowing through it.
   当你有一个流体在三维空间中流动，并且有一个表面位于那个空间中，通过那个表面的通量是流体通过它的速率的一种度量。

10. Flux can be computed with the following surface integral: 
    通量可以用以下的表面积分来计算：

11. Where $S$ denotes the surface through which we are measuring flux.
    其中$S$表示我们正在通过它测量通量的表面。

12. $F(x, y, z)$ is a three-dimensional vector field, thought of as describing a fluid flow.
    $F(x, y, z)$是一个三维向量场，被认为是描述流体流动的。

1. $n( x , y , z )$ is a function which gives a unit normal vector at each point on $S$.
   $n( x , y , z )$ 是一个函数，它在 $S$ 的每一点给出一个单位法向量。

2. $d \Sigma$ can be thought of as a tiny unit of area on the surface $S$.
   $d \Sigma$ 可以被认为是表面 $S$ 上的一个微小的面积单位。

--- pic\Flux in three dimensions.pdf_01.png ---

1. Vector field around a surface
   表面周围的向量场

2. Changing fluid mass in a blob
   改变一个斑点中的流体质量

3. Think of some three-dimensional vector field, represented by a vector-valued function $F(x, y, z)$.
   想象一下某个由向量值函数$F(x, y, z)$表示的三维向量场。

4. Three dimensional vector field
   三维向量场

5. As we like to do with vector fields, imagine this is describing some three-dimensional fluid flow.
   就像我们喜欢对向量场做的那样，想象这是在描述某种三维流体流动。

6. And for this topic, it helps to just imagine what that flow looks like over a quick instant.
   对于这个主题，有助于想象一下那个流在瞬间是什么样子。

7. Perhaps imagine fluid particles moving from the tail of each vector to its tip over a very short time $\Delta t$.
   也许可以想象在很短的时间$\Delta t$内，流体粒子从每个向量的尾部移动到它的顶部。

8.  Now think of some three-dimensional blob, with the fluid passing through its surface.
    现在想象一下某个三维的斑点，流体通过它的表面。


--- pic\Flux in three dimensions.pdf_02.png ---

1. Blob in a vector field.
   矢量场中的斑块。

2. Let's name the surface of that blob $S$.
   我们将那个斑块的表面命名为$S$。

3. Key question: How much fluid is leaving/entering this blob as the fluid flows along the vector field defined by $F(x, y, z)$?
   关键问题：当流体沿着由$F(x, y, z)$定义的向量场流动时，有多少流体正在离开/进入这个斑块？

4. To be precise, we could phrase this in terms of the mass leaving/entering the blob.
   确切地说，我们可以用离开/进入斑块的质量来表述这一点。

1. For the sake of simplicity (who doesn't like simplicity, right?), let's assume the fluid has density $1 \, \text{kg} / \text{m}^3$.
   为了简单起见（谁不喜欢简单呢？），我们假设流体的密度为 $1 \, \text{kg} / \text{m}^3$。

2. Here's a more quantifiable phrasing of our key question: 
   这是我们关键问题的更可量化的表述：

1. More rigorous phrasing: What is the rate of change of mass inside the blob, as a function of time?
更严谨的表述：作为时间函数，物体内部质量的变化率是多少？
6. Assume the velocity of each fluid particle is given by the vector $F(x, y, z)$, where $(x, y, z)$ are the coordinates of the particle.
   假设每个流体粒子的速度由向量$F(x, y, z)$给出，其中$(x, y, z)$是粒子的坐标。

3. Also assume that the fluid has a uniform density of $1 \, \text{kg} / \text{m}^3$ throughout the surface.
   同样假设流体在整个表面上的密度均匀，为 $1 \, \text{kg} / \text{m}^3$。



7.  Flow through each tiny piece of the surface.
   流经表面的每一小片。

4. Here's the essence of how to solve the problem: 
   这是解决问题的要点：

1. Step 1: Break up the surface $S$ into many, many tiny pieces.
步骤1：将表面 $S$ 分解成许多许多的小片。


5.  Step 2: See how much fluid leaves/enters each piece.
    步骤2：看看每个部分离开/进入的流体有多少。

6.  Step 3: Add up all of these amounts with a surface integral.
    步骤3：使用表面积分将所有这些量加起来。
5. Step 1: Break up the surface.
   步骤1：分解表面。

--- pic\Flux in three dimensions.pdf_03.png ---

1. In principle, you should think of each piece as being infinitesimally small.
   原则上，你应该把每一块都想象成无穷小的。

2. After all, this is what we like to do with integrals.
   毕竟，这是我们喜欢做的积分。

2. A common notation to use with surfaces is to denote the infinitesimal area of one of these pieces as "$d\sum$".
   一个常用的表示表面的符号是用"$d\sum$"表示这些片段中的一个的无穷小面积。

3. Also, since each piece is really small, and since we are thinking of the surface $S$ as being smooth, you can treat these pieces as if they are flat.
   此外，由于每一块都非常小，并且我们把表面$S$看作是平滑的，所以你可以把这些片段当作是平的。

4. Step 2: Measure fluid flow through each piece.
   步骤2：测量每块的流体流动。

5. Since each of these pieces is really tiny, all of the fluid flowing through it will basically be moving at the same speed and direction.
   由于每一块都非常小，流经它的所有流体基本上都会以相同的速度和方向移动。

6. Specifically, if you choose an arbitrary point $(x_0, y_0, z_0)$ on this piece, the fluid particles passing through it will have a velocity vector  $\approx$ $F(x_0, y_0, z_0)$.
   具体来说，如果你在这一块上选择一个任意点$(x_0, y_0, z_0)$，通过它的流体粒子将有一个速度矢量 $\approx$ $F(x_0, y_0, z_0)$。

7. This means the fluid passing through it over a short time $\Delta t$ will form some kind of slanted prism.
   这意味着在短时间$\Delta t$内通过它的流体会形成一种倾斜的棱柱。


--- pic\Flux in three dimensions.pdf_04.png ---

1. Flow through a single piece of area.
   单个面积片通过的流量。

2. The displacement vector for each one of these particles will be its velocity times the change in time: 
   这些粒子中每一个的位移矢量将是它的速度乘以时间变化：

3. Vector describing slanted edge of prism.
   描述棱镜斜边的矢量。

4. Now let $n$ denote the unit normal vector to our tiny piece of area:
   现在让$n$表示我们的小面积片的单位法向量：

5. Concept check: What is the volume of fluid which leaves the tiny piece over the time $\Delta t$? (The tiny piece has area $d\sum$). 
   概念检查：在时间$\Delta t$过程中离开这小块的流体体积是多少？（这小块有面积$d\sum$）。

--- pic\Flux in three dimensions.pdf_05.png ---

1. The second choice is correct: 
   第二个选择是正确的：

1. The slanted prism formed by the fluid leaving our tiny piece has a base with area $\Delta \sum$.
   由流体离开我们的微小部分形成的倾斜棱柱有一个面积为$\Delta \sum$的底面。

2. To get its volume, we must multiply this base area by the height of the prism.
   要得到其体积，我们必须将这个底面积乘以棱柱的高。

3. The displacement $F(x_0, y_0, z_0) \Delta t$ of a fluid particle does not quite give the height.
   流体粒子的位移$F(x_0, y_0, z_0) \Delta t$并不能完全给出高度。

4. What we want is the component of that vector which is perpendicular to the tiny piece, so we take the dot product between this vector and the unit normal vector:
   我们想要的是这个矢量的分量，它垂直于这个微小的部分，所以我们取这个矢量和单位法矢量之间的点积：

4. I chose to rearrange this into the equivalent expression $(F(x_0, y_0, z_0) \cdot n) \Delta t$ because the next thing to do involves dividing out that $\Delta t$. 
   我选择将此重排为等效表达式$(F(x_0, y_0, z_0) \cdot n) \Delta t$，因为接下来要做的事情涉及到将那个$\Delta t$分解出来。

5. Notice, since we are assuming the density of the fluid is 1, this expression also gives the mass of fluid leaving the tiny piece. 
   注意，因为我们假设流体的密度为1，这个表达式也给出了离开微小部分的流体的质量。

6. If you divide by the change in time $\Delta t$, you can get the rate at which mass is passing through that tiny piece of area: 
   如果你用时间的变化$\Delta t$来除，你可以得到质量通过那个微小的面积的速率：

7.  Note: Orientation matters
    注意：方向很重要

8.  Notice, if we had chosen the unit normal vector pointing in the opposite direction, the sign of this expression $(F(x_0, y_0, z_0) \cdot n) (\Delta \sum)$ would be flipped. 
    注意，如果我们选择了指向相反方向的单位法向量，这个表达式$(F(x_0, y_0, z_0) \cdot n)  (\Delta \sum)$的符号就会翻转。

9. With closed surfaces, the convention is to choose an outward-facing unit normal vector.
   对于闭合的表面，习惯选择一个向外的单位法向量。

10. This means our expression for flow rate will be positive when fluid is flowing out of the region through the tiny piece, and negative if fluid is flowing into that region.
    这意味着我们的流速表达式在流体通过微小的部分从区域内流出时为正，如果流体流入该区域则为负。

--- pic\Flux in three dimensions.pdf_06.png ---

1. Step 3: Add it all together with an integral
   第三步：将其全部加在一个积分中。

2. The goal is to measure the rate at which fluid flows through the entire surface as a whole: 
   目标是测量流体通过整个表面的速率：

1. Fluid exiting blob
流体从块中出来


1. (Note, in this animation all fluid is going out of the surface. In general, it might be going into the region at some points).
   （注意，在这个动画中，所有的流体都在从表面流出。一般来说，它可能在某些点进入区域）。

1. To get this more global flow rate, add up the rate at which mass flows through each tiny piece of $S$.
   要获得这种更全局的流量，需要将质量通过 $S$ 的每一小块的流速相加。

4. Since we are adding up quantities associated with tiny pieces of area on a surface, the appropriate tool is a surface integral.
   由于我们正在将与表面上的小面积片段相关的数量加起来，所以适当的工具是表面积分。

5. Take the result from the last section:
   从上一节取得的结果：

1. Flow rate through tiny piece.
通过小片的流速。

3. Now put it into a surface integral:
   现在将它放入表面积分中。

4. Notice, there are two functions inside this integral: 
   请注意，这个积分内有两个函数：

1. $F(x, y, z)$, which gives the velocity of a fluid particle at a point.
$F(x, y, z)$，它给出了一个点上流体粒子的速度。

1. $n ( x , y , z )$, which gives the outward facing unit normal vector at an arbitrary point on the surface.
   $n ( x , y , z )$，它给出了表面上任意一点向外的单位法向量。

--- pic\Flux in three dimensions.pdf_07.png ---

1. Both of these are vector-valued functions, and their dot product Is a scalar-valued function.
   这两者都是矢量值函数，它们的点积是一个标量值函数。

2. You might write this as the negative derivative of fluid mass in $R$; negative because the surface integral will be positive when fluid leaves the region.
   你可能会将其写为$R$中流体质量的负导数；之所以为负，是因为当流体离开区域时，表面积分将为正。

3. Rate at which fluid exits $R$.
   流体离开$R$的速率。

4. In the next article, you can walk through an example computing one of these integrals.
   在下一篇文章中，你可以通过一个例子来计算这些积分之一。

5. This involves finding an expression for the unit normal vector, reframing the integral in terms of a parameterization for $S$, etc. 
   这涉及到找到单位法向量的表达式，根据$S$的参数化重新构造积分等。

1. Flux
通量

6. This measure of how much fluid is flowing through a surface is called flux.
   测量流经表面的流体量的这个度量被称为通量。

7. In the example above, this was framed in the context of a closed surface that is the boundary of a region, in which case flux was also a measure of the changing mass in that region.
   在上面的例子中，这是在一个封闭表面的背景下构建的，该封闭表面是一个区域的边界，在这种情况下，通量也是衡量该区域中质量变化的一种方法。

8. In principle, though, flux is something you can compute for any surface, closed or not.
   但原则上，你可以为任何表面（无论是否封闭）计算通量。

9. Many things in physics can be thought of as a flow of some sort, not just fluid.
   在物理学中，许多事物都可以被视为某种类型的流动，而不仅仅是流体。

10. Heat, and even in some sense forces, also flow through space.
    热量，甚至在某种意义上，力也会通过空间流动。

11. And as such, it Is not uncommon to find yourself computing flux through a surface in a problem about heat or, say, electromagnetism.
    因此，你会发现自己在关于热量或者说电磁的问题中计算通过表面的通量并不少见。

--- pic\Flux in three dimensions.pdf_08.png ---

1. Given a three-dimensional fluid flow, the intuition for computing its flux through a surface goes as follows: 
   给定一个三维流体流动，计算其通过表面的通量的直觉如下：

2. Imagine cutting the surface up into many small pieces, small enough that each piece can be considered flat. 
   想象将表面切成许多小块，每一块都小到可以被视为平面。

1. Compute how much fluid flows through each piece as a function of the area $d\Sigma$ of that piece, the unit normal vector $n$ to that piece, and the fluid velocity $F$ in that region.
   计算通过每一块的流体量，作为该块的面积 $d\Sigma$，该块的单位法向量 $n$，以及该区域的流体速度 $F$ 的函数。

4. "Add up" all these flow rates with a surface Integral to get the flux as a whole. 
   用面积积分将所有这些流量"加起来"，得到整体的通量。

1. Flux through $S$. 
通过$S$的通量。

5. If you change the orientation of your surface by choosing unit normal vectors facing the opposite direction, the sign of this integral will be flipped. 
   如果你通过选择朝相反方向的单位法向量改变你的表面的方向，那么这个积分的符号将会翻转。  