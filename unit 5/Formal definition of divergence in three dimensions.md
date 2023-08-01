
--- pic\Formal definition of divergence in three dimensions.pdf_00.png ---

1. Formal definition of divergence in three dimensions
   三维散度的正式定义

2. Learn how surface integrals and 3D flux are used to formalize the idea of divergence in 3D. 
   学习如何使用曲面积分和三维通量来形式化三维散度的概念。

3. Background 
   背景

4. Formal definition of divergence in two-dimensions
    二维散度的正式定义

5. Flux in three-dimensions
   三维的通量

1. It is a short step between these two prerequisites, and understanding the formal definition of divergence in three dimensions. 
   在这两个先决条件之间是一个短步骤，并理解三维散度的正式定义。

2. For that reason, I'm going to keep this article relatively short, assuming that you have the intuition behind both of those pieces of background knowledge. 
   因此，我将保持这篇文章相对较短，假设你对这两个背景知识的直觉有所理解。

3. What we're building to 
   我们正在构建的

1. The goal is to capture the intuition of outward fluid flow at a point in a mathematical formula.
目标是将流体在一个点的外流的直觉捕捉到一个数学公式中。

1. In three-dimensions, divergence is defined using the following limit: 
   在三维空间中，散度定义为使用以下极限：

1. Average outward flow from $R$ per unit volume
   单位体积的 $R$ 的平均外流量

2. Flux through the surface of $R$
   通过 $R$ 表面的通量

--- pic\Formal definition of divergence in three dimensions.pdf_01.png ---

1. $F(x, y, z)$ is a three-dimensional vector field, thought of as defining a three-dimensional fluid flow.
   $F(x, y, z)$是一个三维矢量场，被视为定义一个三维流体流动。

1. $(x, y, z)$ is some specific point in space.
   $(x, y, z)$ 是空间中的某个特定点。

1. $R_{( x , y , z )}$ is a three-dimensional region which contains the point $( x , y , z )$.
   $R_{( x , y , z )}$ 是一个包含点 $( x , y , z )$ 的三维区域。

2. $|R_{( x , y , z )}|$ is the volume of $R_{( x , y , z )}$.
   $|R_{( x , y , z )}|$ 是 $R_{( x , y , z )}$ 的体积。

3. $|R_{( x , y , z )}| \to 0$ indicates that we are considering the limit as the volume of the region goes to 0.
$|R_{( x , y , z )}| \to 0$ 表示我们正在考虑区域体积趋近于0的极限。

4. Since $R_{( x , y , z )}$ must contain $( x , y , z )$ by definition, you can think of the region as shrinking around the specific point.
由于 $R_{( x , y , z )}$ 必须包含 $( x , y , z )$，你可以认为该区域在特定点周围收缩。

4. $S$ is the boundary of $R_{( x , y , z )}$, which is a surface.
   $S$ 是 $R_{( x , y , z )}$ 的边界，它是一个表面。

5. $n ( x , y , z )$ is a vector-valued function which returns an outward facing unit normal vector at each point on $S$.
   $n ( x , y , z )$ 是一个向量值函数，它在 $S$ 上的每一点返回一个向外的单位法向量。

6. The surface integral $\iint_S F \cdot n  d \Sigma$ gives the flux of $F$ through the surface.
   表面积分 $\iint_S F \cdot n  d \Sigma$ 给出了通过表面的 $F$ 的通量。



3. There is quite a lot going on in this definition, but most of the complexity lies in that flux integral. 
   在这个定义中有很多内容，但是大部分复杂性在于那个通量积分。

4. If you understand that part, the rest comes from taking the limit with respect to a region shrinking around a point. 
   如果你理解了那一部分，剩下的部分来自于对收缩在一个点周围的区域取极限。

5. From a region to a point.
   从一个区域到一个点。

6. Let's say you have a three-dimensional vector field.  
   假设你有一个三维矢量场。

7. Three-dimensional vector field.
    三维矢量场。

8. As always, think of this vector field as representing a fluid flow. 
   一如既往，把这个向量场看作代表一个流体流动。

9.  The divergence $divF$ tries to measure the "outward flow" of this fluid at each point. 
    散度$divF$试图在每一点测量这个流体的“外流”。

10. However, it doesn't quite make sense to talk about what it means for fluid to flow out of a point. 
    然而，谈论流体从一个点流出意味着什么并没有太大的意义。

11. What does make sense is the idea of fluid flowing out of region. 
    有意义的是流体从区域流出的概念。

12. Specifically, picture some region $R$ in the vector field.
    具体来说，想象矢量场中的某个区域$R$。

--- pic\Formal definition of divergence in three dimensions.pdf_02.png ---

1. Blob in a vector field
   矢量场中的体积元


2. Let's name the surface of this region "$S$". 
   让我们将这个区域的表面命名为“$S$”。

3. In the article on flux in three dimensions, I showed how you can measure the rate at which fluid is leaving this region by taking the flux of $F$ over the surface $S$: 
   在关于三维流量的文章中，我展示了如何通过取表面$S$上的$F$的流量来测量流体离开这个区域的速率：

4. Rate at which fluid exits $R$ 
   流体离开$R$的速率，

1. Flux surface integral
   流量表面积分


5. Here, $n(x, y, z)$ is a vector-valued function which returns the outward facing unit normal vector at each point on $S$.
   这里，$n(x, y, z)$是一个向量值函数，它在$S$上的每一点返回面向外的单位法向量。

6. Divergence itself is concerned with the change in fluid density around each point, as opposed to mass.
   散度本身关注的是每一点周围的流体密度变化，而不是质量。

7. We can get the change in fluid density of $R$ by dividing the flux integral by the volume of $R$.
   我们可以通过将通量积分除以$R$的体积来得到$R$的流体密度变化。

8. To denote the volume of $R$, put bars around It: 
   要表示$R$的体积，可以在其周围加上竖线：

9. Volume of $R$
$R$的体积

1.  So here's what rate at which fluid density changes inside $R$ looks like:
   因此，流体密度在$R$内部变化的速率是这样的：

2.  The divergence of $F$ at a point $(x, y, z)$ is defined as the limit of this change-in-fluid-density expression as the region shrinks around the point $(x, y, z)$.
   点$(x, y, z)$处$F$的散度被定义为此流体密度变化表达式的极限，当区域在点$(x, y, z)$周围缩小时。

2. $R$ shrinks around $(x, y, z)$
   $R$ 在 $(x, y, z)$ 周围收缩

--- pic\Formal definition of divergence in three dimensions.pdf_03.png ---

1. In that equation, | wrote $R \rightarrow (x, y, z)$ to communicate the idea of $R$ shrinking around the point $(x, y, z)$.
   在那个等式中，我写了 $R \rightarrow (x, y, z)$ 来传达 $R$ 在点 $(x, y, z)$ 周围缩小的概念。

2. At the end of the day, all this notation is just a desperate attempt to communicate a heavily visual idea with symbols.
   说到底，所有这些符号都只是用符号来传达一个重视视觉的想法的一种绝望的尝试。

3. You will see different authors use different notation. 
   你会看到不同的作者使用不同的记号。

1. If you prefer, you could alternatively start by saying $R_{(x, y, z)}$ is a region which contains the point $(x, y, z)$, then write the following:
   如果你愿意，你也可以先说 $R_{(x, y, z)}$ 是一个包含点 $(x, y, z)$ 的区域，然后写下以下内容：

4. I have a slight preference for this last notation, just because it makes It a bit easier to see the connection between $(x, y, z)$ on the left hand side and the right hand side without relying so heavily on the context in which all the terms are defined.
   我稍微偏爱这最后一个记号，仅仅是因为它让人更容易看出左边的 $(x, y, z)$ 和右边的联系，而不是过分依赖于定义所有项的上下文。

5. Congratulations! 
   恭喜！

1. It also means you are in a strong position to understand the divergence theorem, which connects this idea to that of triple integrals.
   这也意味着你在理解散度定理方面处于有利的地位，散度定理将这个想法与三重积分联系起来。