
--- pic\Surface integrals.pdf_00.png ---

1. Surface integrals
   表面积分

2. How do you add up infinitely many infinitely small quantities associated with points on a surface?
   如何累加与表面上的点相关的无穷多个无穷小的数量？

1. Background
   背景

2. Surface area
   表面积

3. Double integrals
   双重积分

4. Not strictly required, but useful for intuition and analogy: Line integrals.
   不是严格要求，但有助于直观理解和类比：线积分。

1. What we're building to:
   我们正在构建的是：

2. In principle, the idea of a surface integral is the same as that of a double integral, except that instead of "adding up" points in a flat two-dimensional region, you are adding up points on a surface in space, which is potentially curved.
   原则上，表面积分的概念与双重积分的概念相同，只不过不是在平面的二维区域中“加和”点，而是在空间中的表面上加和点，这可能是曲线。

1. The abstract notation for surface integrals looks very similar to that of a double integral:
   表面积分的抽象记号与双重积分的抽象记号看起来非常相似：

2. Tiny piece of area in $S$
   在$S$中的微小面积

3. $S$ represents a surface
   $S$代表一个表面。

4. Computing a surface integral is almost identical to computing surface area using a double integral, except that you stick a function inside the integral
   计算表面积分几乎与使用双重积分计算表面积相同，只是在积分中加入了函数

5. Tiny piece of area.
   微小面积。

6.  Here, $v(t, s)$ is a function parameterizing the surface $S$ from the region $T$ of the $ts$-plane.
    在这里，$v(t, s)$是一个函数，它将表面$S$从$ts$平面的区域$T$参数化。

7.  This is analogous to how computing line integrals is basically the same as computing arc length integrals, except that you throw a function inside the integral itself.
    这类似于计算线积分基本上与计算弧长积分相同，只不过在积分本身内部引入了一个函数。

8.  You can find an example of working through one of these integrals in the next article.
    在下一篇文章中，你可以找到一个通过这些积分的例子。

--- pic\Surface integrals.pdf_01.png ---

1. The idea of surface integrals
   表面积分的概念

2. lf you understand double integrals, and you understand how to compute the surface area of a parametric surface, you basically already understand surface integrals.
   如果你理解双重积分，并且你理解如何计算参数曲面的表面积，你基本上已经理解了表面积分。

3. It's just a matter of smooshing the two intuitions together.
   这只是将两种直觉结合在一起的问题。

4. I'll go over the computation of a surface integral with an example in just a bit, but first, I think it's important for you to have a good grasp on what exactly a surface integral does.
   我稍后会通过一个例子详述表面积分的计算，但首先，我认为你有必要很好地理解表面积分到底是做什么的。

5. Refresher of double integrals
   双重积分的回顾

1. Recall what a double integral does:
   回忆一下双重积分是做什么的：

2. Here, $R$ represents some region of the $xy$-plane, and $f(x, y)$ is a way to associate each point of $R$ with a number.
   这里，$R$表示$xy$-平面的某个区域，$f(x, y)$是一种将$R$的每个点与一个数字关联起来的方法。

1. Maybe $R$ represents a metal sheet, and $f(x,y)$ represents the density at each point.
   也许$R$代表一个金属片，$f(x,y)$表示每个点的密度。

2. Or perhaps $R$ represents a geographic region, and $f(x, y)$ represents the temperature at each point.
   或者，$R$表示一个地理区域，$f(x, y)$表示每个点的温度。

8. The double integral provides a way to "add up" the values of $f$ on this region.
   双重积分提供了一种在这个区域上“加总”$f$的值的方法。

1. However, the idea of "adding up" points in a continuous region is vague, so I like to imagine the following process:
   然而，“加总”连续区域中的点的概念是模糊的，所以我喜欢想象以下过程：

2. Chop up the region $R$ into many tiny pieces.
   将区域$R$切成许多小块。

10. Multiply the area of each piece, thought of as $dA$, by the value of $f$ at one of the points inside that piece.
    将每块的面积（看作$dA$）与该块内某点的$f$的值相乘。

--- pic\Surface integrals.pdf_02.png ---

1. Add up the resulting values.
   对结果值进行求和。

2. For example,
   例如，

2. If $R$ represents a metal sheet, and $f(x, y)$ is a density function, the double integral will give you the mass of the sheet. Why?
   如果$R$代表一片金属片，而$f(x, y)$是密度函数，那么双重积分将给出这片金属片的质量。为什么？

3. If $R$ represents a geographic region, and $f(x, y)$ give the temperature at each location, taking this double integral then dividing by the area of $R$ will give you the average temperature in that region. Why?
   如果$R$代表一个地理区域，$f(x, y)$给出每个位置的温度，那么进行这个双重积分然后除以$R$的面积将给你该区域的平均温度。为什么？

4. Double integrals over curved regions
   曲面上的双重积分

1. However, why stay so flat?
   然而，为什么要保持如此平坦？

2. This idea of adding up values over a continuous two-dimensional region can be useful for curved surfaces as well.
   在连续的二维区域上加和值的这个想法也适用于曲面。

6. What if you are considering the surface of a curved airplane wing with variable density, and you want to find its total mass?
   如果你正在考虑一个变密度的曲面飞机翼的表面，而你想找出它的总质量呢？

7. What if you have the temperature for every point on the curved surface of the earth, and you want to figure out the average temperature?
   如果你有地球曲面上每一点的温度，而你想计算出平均温度呢？

1. This time, the function $f$, which represents density, temperature, etc., must take in point of three dimensions since points on the surface live in three dimensions.
   这次，代表密度、温度等的函数 $f$，必须接收三维的点，因为表面上的点存在于三维空间中。

9. The abstract notation for integrating a three-variable function $f(x,y, z)$ over a surface is pretty much the same as the abstract notation for double integrals:
   对一个三变量函数$f(x,y, z)$在一个表面上进行积分的抽象表示法和双重积分的抽象表示法几乎相同：


--- pic\Surface integrals.pdf_03.png ---

1. Tiny piece of area on $S$.
   $S$上的小面积片段。

2. $S$ represents some surface 
   $S$代表某些表面

1. (Different authors might use different notation).
（不同的作者可能使用不同的符号）。

3. This is called a surface integral.
   这被称为表面积分。

4. The little $S$ under the double integral sign represents the surface itself, and the term $d\sum$ represents a tiny bit of area piece of this surface.
   双重积分符号下的小$S$代表表面本身，而项$d\sum$代表这个表面的一小块面积。

1. You can think about surface integrals the same way you think about double integrals:
   你可以像考虑双重积分一样考虑表面积分：

2. Chop up the surface $S$ into many small pieces.
   将表面$S$切割成许多小片。

6. Multiply the area of each tiny piece by the value of the function $f$ on one of the points in that piece.
   乘以每一小片的面积和函数$f$在该片中的一点的值。

7. Add up those values.
   加起这些值。

1. Why write $d\sum$ instead of $dA$?
   为什么写$d\sum$而不是$dA$？

2. There's no real difference; each one represents a tiny bit of area of the thing you are integrating over.
   其实没有真正的差别；每一个都代表你正在积分的东西的一小部分面积。

9.  However, when it comes time to compute things, the way to handle a tiny bit of area on a curved surface is fundamentally different from doing it on a flat surface, so it's worth emphasizing this difference by using a different variable.
    然而，当计算的时候，处理曲面上的一小块面积的方式从根本上来说与处理平面上的方式不同，所以使用不同的变量来强调这个差异是值得的。

10. How to compute a surface integral.
    如何计算表面积分。

11. Abstract notation and visions of chopping up airplane wings are all well and good, but how do you actually compute one of these surface integrals?
    抽象的符号和分解飞机翅膀的想法都很好，但你实际上如何计算这些表面积分呢？

12. The trick is to sneakily turn it into an ordinary, flat, double integral.
    技巧在于巧妙地将其转化为普通的、平面的、双重积分。

13. Specifically, the way you tend to represent a surface mathematically is with a parametric function.
    具体来说，你通常用参数函数来表示一个数学上的表面。

14. You'll have some vector-valued function $v(t, s)$, which takes in points on the two-dimensional $ts$-plane (lovely and flat), and outputs points in three-dimensional space.
    你会有一些向量值函数$v(t, s)$，它接收$ts$平面（可爱且平坦）上的点，并输出三维空间中的点。

15. You also need to specify the region $T$ of the $ts$-plane which maps onto the surface $S$.
    你还需要指定映射到表面$S$的$ts$平面的区域$T$。

16. The trick for surface integrals, then, is to find a way of integrating over the flat region $T$ that gives the same effect as integrating over the curved surface $S$.
    然后，计算表面积分的技巧就是找到一种在平面区域$T$上积分的方法，使得其效果与在曲面$S$上积分的效果相同。


--- pic\Surface integrals.pdf_04.png ---

1. This requires describing "tiny piece of area" of $S$ in terms of something inside the parameter.
   这需要用参数内的某个量来描述$S$的"微小面积"。

2. Almost all of the work for this was done in the article on surface area.
   这方面的大部分工作都在关于表面积的文章中完成。

3. There, we saw how a tiny rectangle inside $T$ with area $dt ds$ gets transformed into a parallelogram on $S$ with area $|\frac{\partial v}{\partial t} \times \frac{\partial v}{\partial s}| dt ds$.
   在那里，我们看到了如何将内部面积为$dt ds$的$T$中的一个小矩形转换为$S$上面积为$|\frac{\partial v}{\partial t} \times \frac{\partial v}{\partial s}| dt ds$的平行四边形。

1. In parameter space.
   在参数空间。

2. On the surface $S$.
   在表面$S$。

3. For our surface integral desires, this means you expand $d\sum$ as follows: 
   对于我们的表面积分需求，这意味着你需要按照以下方式展开$d\sum$：

4. Specifically, here's how to write a surface integral with respect to the parameter space: 
   具体来说，这是如何对参数空间编写表面积分的：

5. Let's break that down a bit:
   让我们稍微拆解一下：

7. Integral over surface.
   对表面进行积分。

6. Area of a tiny piece of $S$.
   $S$ 上一小块区域的面积。

8.  See where each point $(t, s)$ lands on $S$, then evaluate $f$.
   观察每个点 $(t, s)$ 在 $S$ 上的位置，然后计算 $f$。

9.  How much a tiny piece of $T$ is scaled after it is mapped onto $S$ by $v$.
   通过 $v$ 将 $T$ 的一小块映射到 $S$ 上后，这小块的缩放程度是多少。

10. Area of a tiny piece of $T$.
   $T$ 的一小块区域的面积。

--- pic\Surface integrals.pdf_05.png ---

1. The main thing to focus on here, and what makes computations particularly labor intensive, is the way to express $d\sum$.
   这里需要关注的主要事情，也是使计算特别劳动密集的，是表达$d\sum$的方式。

2. In the next article, you can go through a full example of one of these surface integrals.
   在下一篇文章中，你可以看到这些面积积分的一个完整示例。

3. Summary: Surface integrals are used anytime you get the sensation of wanting to add a bunch of values associated with points on a surface.
   概要：面积积分在你有感觉想要将一堆与表面点相关的值加起来的任何时候都会使用。

4. This is the two-dimensional analog of line integrals.
   这是线积分的二维对应物。

5. Alternatively, you can view it as a way of generalizing double integrals to curved surfaces.
   或者，你可以将其视为将双重积分推广到曲面的一种方式。

6. Tiny piece of area in $S$
   $S$中的微小面积

7. $S$ represents a surface.
   $S$表示一个表面。

8. Computing a surface integral is almost identical to computing surface area using a double integral, except that you stick a function inside the integral: 
   计算面积积分与使用双重积分计算面积几乎相同，只是你将一个函数放在积分内：

9. Like so many things in multivariable calculus, while the theory behind surface integrals is beautiful, actually computing one can be painfully labor intensive.
   像多元微积分中的许多其他事情一样，虽然面积积分背后的理论很美，但实际上计算一个面积积分可能非常费力。
