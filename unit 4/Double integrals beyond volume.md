
--- pic\Double integrals beyond volume.pdf_00.png ---

1. Double integrals beyond volume.
   双重积分超越体积。

2. Double integrals do more than find volume under three-dimensional graphs.
   双重积分不仅仅是找出三维图形下的体积。

3. Here we cover other uses, a more general notation for double integrals, and explain the "feel" of double integration.
   这里我们介绍其它用途，双重积分的更通用记法，以及解释双重积分的“感觉”。

4. Background
   背景

5. Double integrals over non-rectangular regions
   非矩形区域的双重积分

6. What we're building to
   我们正在构建的内容

4. Double integrals are used anytime you get that feeling where you want to chop up a two-dimensional region into infinitely many infinitely small areas, multiply each one by some value, then add them up.
   任何时候，当你有种想要将二维区域切割成无限多个无限小的面积，然后将每个面积乘以某个值，再加起来的感觉，就可以使用双重积分。

5. The more general notation for a double integral is $\int \int_R f dA$, where $A$ is the region that you are integrating over.
   双重积分的更通用记法是 $\int \int_R f dA$，其中 $R$ 是你要积分的区域。

6. $dA$ signifies a "tiny chunk of area", which typically means $dx\ dy$ or $dy\ dx$, unless another coordinate system is being used.
   $dA$ 表示一个“微小的区域”，通常意味着 $dx\ dy$ 或 $dy\ dx$，除非正在使用另一个坐标系。

7. Example 1: Mass of a plate
   示例 1：板的质量

7. Imagine a metal plate 3 meters wide and 2 meters tall.
   想象一个宽 3 米，高 2 米的金属板。

8. Our goal will be to find its mass based on its density, but the catch is that the density is not constant over the plate.
   我们的目标将是根据其密度找出其质量，但问题是板上的密度并不是恒定的。

8. To be able to describe this variable density with a function, start by situating the plate on the $xy$-plane:
   为了能够用函数描述这个变化的密度，首先将板放置在 $xy$ 平面上：

--- pic\Double integrals beyond volume.pdf_01.png ---

1. Its lower left corner at the origin, and its long side resting on the $x$-axis.
   它的左下角位于原点，长边搭在 $x$ 轴上。

4. Let's say that the density of this plate, in $kg / m$ , is expressed with the following function.
   假设这个板的密度（单位：$kg/m$）可以用以下函数表示。

5. $\sigma$ is a typical variable name for two-dimensional density.
   $\sigma$ 是表示二维密度的典型变量名。

3. Density is mass per unit area, so it might seem strange to define it using a function which takes in individual points.
   密度是单位面积的质量，所以用一个接收单个点的函数来定义它可能会显得奇怪。

4. After all, what does it mean for a single point like $(1, 2)$ to have density $\sigma(1, 2)$?
   毕竟，像 $(1, 2)$ 这样的单个点具有密度 $\sigma(1, 2)$ 是什么意思呢？

5. If you prefer, you can interpret this function as giving the density within a tiny region around each point.
   如果你愿意，你可以将这个函数解释为给出每个点周围微小区域内的密度。

6. To find the mass of the plate, you can imagine chopping it up into many tiny pieces, each one a rectangle, then adding up their masses.
   为了找到板的质量，你可以想象把它切成许多小片，每一片都是一个矩形，然后加起它们的质量。

--- pic\Double integrals beyond volume.pdf_02.png ---

7. Think of each of these rectangles as having a tiny width, $dx$, and a tiny height, $dy$.
   想象每个矩形都有一个微小的宽度 $dx$ 和一个微小的高度 $dy$。

8. Think about a specific rectangle, perhaps the one containing the point $(1, 2)$.
   考虑一个特定的矩形，也许是包含点 $(1, 2)$ 的那个。

9. Since this rectangle is really small, the density within it will pretty much equal the constant $\sigma(1, 2)$.
   由于这个矩形真的很小，所以它内部的密度几乎等于常数 $\sigma(1, 2)$。

10. The more finely you cut things, and the smaller the rectangles, the closer it is to being true that the density of each rectangle is constant.
    你切割得越细，矩形越小，每个矩形的密度都是常数的说法就越接近真实。

11. This means we can find the mass of each such rectangle.
    这意味着我们可以找到每个这样的矩形的质量。

--- pic\Double integrals beyond volume.pdf_03.png ---

1. To get the total mass of the plate, we integrate all of these tiny masses together.
   为了得到板的总质量，我们将所有这些微小的质量积分在一起。

2. Since we are integrating over a two-dimensional region, we use a double integral.
   由于我们正在对一个二维区域进行积分，所以我们使用双重积分。

3. Caution: the order of your integrals depends on whether you express the tiny area of each rectangle as $dx \, dy$ or $dy \, dx$.
   注意：你的积分顺序取决于你是将每个矩形的微小面积表示为 $dx \, dy$ 还是 $dy \, dx$。

4. Concept check: Which of the following double integrals represents the mass of our metal plate, which is 3 meters wide and 2 meters tall:
   概念检查：以下哪个双重积分代表我们的金属板的质量，该板宽3米，高2米：

5. The second choice is correct.
   第二个选项是正确的。

6. Since $dx$ is written first, the bounds and variable of integration within the inner integral must be in terms of $x$.
   由于 $dx$ 是首先写的，所以内部积分的边界和变量必须以 $x$ 的形式表示。

7. This integral is purely with respect to $x$.
   这个积分完全关于 $x$。

8. Concept check: Using the function $\sigma(x, y) = (\sin(\pi x) + 1)y$, evaluate this double integral.
   概念检查：使用函数 $\sigma(x, y) = (\sin(\pi x) + 1)y$，评估这个双重积分。

4. If you are unsure about how to do this, consider reviewing the article introducing double integrals.
   如果你对此不确定，可以考虑复习一下介绍双重积分的文章。

5. First do inner integral.
   首先进行内部积分。

--- pic\Double integrals beyond volume.pdf_04.png ---

1. So evidently our metal plate with the density function $\sigma ( x , y ) = ( \sin ( \pi x ) + 1 ) y$, has mass $\frac{4}{\pi}+ 6$.
很明显，我们的金属板的密度函数为 $\sigma ( x , y ) = ( \sin ( \pi x ) + 1 ) y$，其质量为 $\frac{4}{\pi}+ 6$。

3. Thinking about tiny areas.
   思考微小的面积。


--- pic\Double integrals beyond volume.pdf_05.png ---

1. When I first introduced double integrals, it was in the context of computing the volume under a graph.
   当我第一次介绍双重积分时，是在计算图形下方体积的上下文中。

2. The thought process went something like this: First cut the volume into infinitely many slices.
   思考过程大致如此：首先将体积切成无限多个切片。

3. Each slice represents a constant value for one of the variables, for example $x = 0.78$.
   每个切片代表变量之一的恒定值，例如 $x = 0.78$。

4. Find the area of each of those slices.
   找到每个切片的面积。

5. This is what the inner integral does.
   这就是内积分的作用。

6. Make each slice an infinitesimal volume by giving it a little depth.
   通过赋予每个切片一点深度，使每个切片成为一个无穷小的体积。

7. Mathematically, this means multiplying the area of each slice by either $dx$ or $dy$, whichever one represents a tiny step perpendicular to the slice.
   在数学上，这意味着将每个切片的面积乘以 $dx$ 或 $dy$，取决于哪一个代表了垂直于切片的微小步长。

8. Integrate those infinitesimal volumes together to get the volume of the solid as a whole.
   将那些无穷小的体积积分在一起，得到整个实体的体积。

9. This is what the outer integral does.
   这就是外积分的作用。

10. By contrast, the example from the previous section finding the mass of the plate has a different look and feel to it.
   相比之下，从前一节找出板块质量的例子有着不同的外观和感觉。

11. We start by thinking about tiny areas, then we multiply each one by a constant (the density) and try to add all of them together at once.
   我们首先考虑微小的区域，然后我们将每一个区域都乘以一个常数（密度）并试图一次性将它们全部加在一起。

12. Of course, both these perspectives are equivalent.
    当然，这两种观点是等效的。

13. And when it comes to the computation, nothing will look different.
    而当涉及到计算时，一切都不会有所不同。

14. You will always set up one integral inside another, compute the inner integral, then compute the outer integral.
    你总是会在一个积分内设立另一个积分，计算内积分，然后计算外积分。

15. Nevertheless, in terms of visualization and conceptual understanding, framing a double integral in terms of tiny areas is distinct from framing it as one linear integral inside another.
    然而，在可视化和概念理解方面，用微小区域来构建双重积分与将其视为一个线性积分内的另一个积分有着明显的区别。

16. For example, if you thought about computing the volume under a graph by initially breaking your region of the $xy$-plane down into tiny areas, you might imagine adding together the volume of thin columns above those tiny areas.
    例如，如果你考虑通过最初将 $xy$ 平面的区域分解为微小区域来计算图形下方的体积，你可能会想象将那些微小区域上方的薄柱体积加在一起。


--- pic\Double integrals beyond volume.pdf_06.png ---

1. Tiny columns of volume.
   体积的微小柱体。

2. General notation for double integrals.
   双重积分的一般符号。

3. When we think about a double integral with respect to tiny areas, it's common to write it abstractly like this: $\iint_R f\, dA$.
   当我们考虑关于微小面积的双重积分时，我们通常这样抽象地写它：$\iint_R f\, dA$。

4. $R$ represents the region that we are integrating over.
   $R$ 代表我们正在积分的区域。

5. The reason for writing it like this is that while you are setting things up, or reasoning about double integrals in general, you typically don't want to get bogged down with the specific (and potentially complicated) definition of your region while you scribble things down.
   之所以这样写，是因为在你设置东西，或者一般地推理双重积分的时候，你通常不想在草稿上被你的区域的特定（并可能复杂的）定义所困扰。

6. When it comes time to compute the integral, we replace this $\iint_R$ with an actual pair of single-integrals with bounds that can be computed.
当计算积分的时候，我们将这个 $\iint_R$ 替换为一个实际的单重积分对，其边界可以计算。

6. When $R$ is a rectangle, those bounds will be constants.
当 $R$ 是一个矩形时，这些边界将是常数。

1. More generally, when $R$ is defined in terms of some curves in the $xy$-plane, the bounds of the inner integral are expressed as functions of the outer variable.
更一般地，当 $R$ 是在 $xy$ 平面上的一些曲线的术语定义时，内部积分的边界被表示为外部变量的函数。

--- pic\Double integrals beyond volume.pdf_07.png ---

1. See the last article for practice with this idea.
请参阅上一篇文章以练习这个想法。

1. $dA$ represents a tiny area, in the same way that $dx$ represents a tiny length in an ordinary integral.
   $dA$ 表示一个微小的面积，就像在普通的积分中 $dx$ 表示一个微小的长度。

2. You will typically imagine chopping up the region $F$ into many tiny pieces, and this term represents the area of one of those pieces.
   你通常会想象将区域 $F$ 切成很多小块，这个项代表了那些小块中一个的面积。

3. Once you get down to computing the double integral, you will replace this with $dx\ dy$, or $dy\ dx$.
   一旦你开始计算双重积分，你将把它替换为 $dx\ dy$ 或 $dy\ dx$。

4. In other coordinate systems, there are different ways to break down $dA$, but I'll leave that for the next article.
   在其他坐标系中，分解 $dA$ 的方法有所不同，但我将留到下一篇文章中介绍。


1. $f(x, y)$ is some two-variable function.
$f(x, y)$ 是一个二元函数。

5. When you chop up your region into many tiny pieces, each piece typically represents some value that you are hoping to add up.
   当你把你的区域切成很多小块时，每一块通常代表一些你希望加起来的值。

6. Perhaps this value is a tiny bit of mass, or the tiny volume of a slim column under a graph.
   也许这个值是一点点的质量，或者图下面一根细柱的微小体积。

7. Hopefully, you are able to express this tiny amount as something times the area of your tiny piece.
   希望你能将这个微小的量表示为一些东西乘以你的微小片的面积。

8. For example, the mass of a piece is its density times its area; and the volume of a column above a piece is the height of the column times the area.
   例如，一块的质量是它的密度乘以它的面积；一个柱子上方的体积是柱子的高度乘以面积。

9. In these examples, $f(x, y)$ represents density, or height.
   在这些例子中，$f(x, y)$ 表示密度或高度。

10. In general, it is the thing that needs to be multiplied by the area $dA$ of a tiny piece, and it generally depends on the position of that tiny piece, expressed with $(x, y)$-coordinates.
    一般来说，这是需要与小片的面积 $dA$ 相乘的东西，它通常取决于用 $(x, y)$ 坐标表示的那个小片的位置。

11. What if I cannot express the tiny value that I want to add up as something times $dA$?
    如果我无法将我想要累加的微小值表示为某物乘以 $dA$ 呢？

12. Well, in that case my friend, double integrals are not the tool for you.
    嗯，那种情况下，我的朋友，双重积分并不适合你。

13. Although I cannot think of any examples where that comes up.
    尽管我想不出任何出现这种情况的例子。


2. There are two benefits to this abstract notation:
这种抽象表示法有两个好处：

--- pic\Double integrals beyond volume.pdf_08.png ---

1. Simplicity: When you're starting to set something up, or if you want to quickly reference the idea of a certain double integral without getting into the implementation details, it's nice to be able to write something quickly.
   简洁：当你开始设置某件事，或者你想快速参照某个双重积分的概念而不需要深入到实现细节时，能够快速写出东西是非常好的。

2. Also, many of the theorems and tools coming up in multivariable calculus are expressed abstractly in this notation.
   同时，多变量微积分中出现的许多定理和工具都用这种表示法抽象地表达出来。

3. Generality: Writing your integral as $\int \int_R f \, dA$ gives you options as you sit down to compute it.
   概括：将你的积分写为 $\int \int_R f \, dA$ 在你计算时提供了选项。

4. For example, in the next article, we will cover double integrals in polar coordinates, in which case the way you expand $dA$ and the way you put bounds on the two integrals are different than they are for cartesian coordinates.
   例如，在下一篇文章中，我们将涵盖极坐标中的双重积分，其中你扩展 $dA$ 的方式和你为两个积分设定边界的方式与笛卡尔坐标系的方式是不同的。

1. Example 2: Center of mass
示例2：质心

2. What is the center of mass of a half-disk?
半圆盘的质心是什么？

6. For simplicity, let's say the radius of the disk is 1, and let's orient it such that the diameter rests on the $y$-axis.
   为了简单起见，让我们假设盘的半径是1，并且让我们将其定向使得直径位于 $y$ 轴上。

7. Also, assume the disk has uniform density everywhere.
   同时，假设整个盘的密度都是均匀的。

8. This is a pretty interesting problem, don't you think? 
   这是一个相当有趣的问题，你不觉得吗？

1. You can guess that the answer is something slightly to the left of $(0.5, 0)$, but it's not obvious what the specific answer should be, is it?
你可以猜测答案应该稍微在 $(0.5, 0)$ 的左边，但具体的答案应该是什么并不明显，对吗？

9.  By the vertical symmetry of this half-disk, you can know that the center of mass will lie on the $x$-axis.
    通过这个半盘的垂直对称性，你可以知道质心将位于 $x$ 轴上。

10. In a sense, what we're looking for is the "average $x$-value" of points in the disk.
    从某种意义上说，我们正在寻找的是盘内点的"平均 $x$ 值"。


--- pic\Double integrals beyond volume.pdf_09.png ---

1. Concept check: If we let $H$ represent this half-disk, with $|H|$ representing its area, which of the following abstractly written integrals represents the $x$-value for the center of mass of $H$? 
   概念检查：如果我们让 $H$ 表示这个半圆盘，用 $|H|$ 表示它的面积，那么下面哪个抽象写出的积分代表 $H$ 的质心的 $x$ 值？

2. The first choice is correct.
   第一个选择是正确的。

3. Since we are assuming uniform density, we can think of $dA$ as representing a tiny piece of mass just as well as it represents a tiny area.
   由于我们假设密度均匀，我们可以认为 $dA$ 既可以代表一小块质量，也可以代表一小块面积。

4. Think of the density as being 1.
   把密度想象成1。

5. You can interpret this integral saying "Chop the disk into many many tiny pieces, multiply the mass (or area) of each one of those pieces by its $x$-value, then add up what you get."
   你可以这样理解这个积分：“把圆盘切成许多许多小片，把每一片的质量（或面积）与它的 $x$ 值相乘，然后加起来。”

1. *** Dividing this by the total mass of the disk, we get the "average $x$-value" of points on the disk, which is the $x$-coordinate of the center of mass.
将其除以圆盘的总质量，我们得到圆盘上点的“平均 $x$ 值”，这是质心的 $x$ 坐标。

7. Concept check: What is the area of the half-disk $H$?
   概念检查：半圆盘 $H$ 的面积是多少？

8. Since the disk has radius 1, the area of the entire full disk would be $\pi R^2$.
   由于圆盘的半径是1，所以整个圆盘的面积将是 $\pi R^2$。

1. Chopping that in half, we get $\frac{\pi}{2}$.
将其一分为二，我们得到 $\frac{\pi}{2}$。

--- pic\Double integrals beyond volume.pdf_10.png ---

1. Concept check: Which of the following represents the right way to expand the integral $\int \int_H x dA$ into a computable form? 
   概念检查：下列哪一项代表了将积分 $\int \int_H x dA$ 扩展为可计算形式的正确方式？

2. Choose all answers that apply:
   选择所有适用的答案：


3. This is kind of a trick question, both answers are correct.
   这是一个有点儿狡猾的问题，两个答案都是正确的。

4. The first one shows what it looks like if you think about dividing $H$ into horizontal stripes:
   第一个答案展示了如果你考虑将 $H$ 划分为水平条纹，它会是什么样子：

5. The right bound of this stripe, as a function of $y$, is found using the Pythagorean theorem.
   这个条纹的右边界，作为 $y$ 的函数，是用毕达哥拉斯定理找到的。

6. The integral over $H$ now starts by integrating along this stripe with respect to $x$ (the inner integral), then integrating the result between $-1$ and $1$ with respect to $y$, (the outer integral).
   现在对 $H$ 的积分开始沿着这个条纹对 $x$ 进行积分（内部积分），然后对结果在 $-1$ 和 $1$ 之间对 $y$ 进行积分（外部积分）。

7. The second integral shows what happens when you think of dividing $H$ into vertical stripes.
   第二个积分展示了当你想把 $H$ 划分为垂直条纹时会发生什么。

--- pic\Double integrals beyond volume.pdf_11.png ---

1. The bounds are again found using the Pythagorean theorem, but this time they must be expressed as functions of $x$.
   积分的界限再次使用勾股定理找到，但是这次它们必须表示为 $x$ 的函数。

2. Now the inner integral is with respect to $y$, and the outer integral is with respect to $x$, going from 0 to 1.
   现在，内部积分是关于 $y$ 的，外部积分是关于 $x$ 的，从 0 到 1。

3. Bring it on home: Solve this integral, and use it to find the center of mass of $H$.
   解决这个积分，并用它来找到 $H$ 的质心。

1. $x$ -coordinate of center of mass:
质心的 $x$ 坐标：

4. You can choose either one of the integrals shown in the previous question, but I think the one corresponding to horizontal stripes looks a bit easier.
   你可以选择上一个问题中显示的任何一个积分，但我认为对应于水平条纹的那个看起来稍微简单一些。

1. Start by evaluating the inner integral.
开始计算内部积分。

--- pic\Double integrals beyond volume.pdf_12.png ---

1. We are not done!
   我们还没有完成！

1. To find the center of mass we need to divide this by the total area of the disk, which is $\frac{\pi}{2}$.
为了找到质心，我们需要将其除以圆盘的总面积，即 $\frac{\pi}{2}$。

1. Therefore, the $x$-coordinate of the center of mass of the half-disk $A$ is $\frac{4}{3\pi}$.
   因此，半盘 $A$ 的质心的 $x$ 坐标是 $\frac{4}{3\pi}$。

2. It makes sense that this should be a little bit less than 0.5, since more of the mass is on the left portion of the half-disk.
这个结果小于0.5是有道理的，因为更多的质量在半圆盘的左侧部分。

1. Summary
总结

1. Double integrals are used anytime you get that feeling where you want to chop up a two-dimensional region into infinitely many infinitely small areas, multiply each one by some value, then add them up.
   任何时候，当你想把一个二维区域切成无穷多个无穷小的区域，然后把每一个区域乘以某个值，再加起来的时候，都会用到双重积分。

2. The more general notation for a double integral is $\int\int_R f \, dA$.
   双重积分的更通用符号是 $\int\int_R f \, dA$。

3. $R$ is the region that you are integrating over.
   $R$ 是你正在进行积分的区域。

4. $dA$ signifies a "tiny chunk of area", which typically means $dx \, dy$ or $dy \, dx$, unless another coordinate system is being used.
   $dA$ 表示一个"微小的区域"，通常意味着 $dx \, dy$ 或 $dy \, dx$，除非使用其他坐标系统。

5. $f(x, y)$ is a two-variable function.
$f(x, y)$ 是一个双变量函数。

1. From this point forward, double integrals will be inextricably tied to most of the new topics in multivariable calculus.
从这一点开始，双重积分将与多元微积分的大部分新主题密切相关。

1. And in almost all cases, it helps to think about what's happening inside each "tiny area" of a given region, rather than thinking about integrating something along a line then integrating again in the perpendicular direction.
在几乎所有的情况下，思考在给定区域的每一个"微小区域"内发生的事情比沿着一条线进行积分然后在垂直方向再次进行积分要有帮助。


补充***：
这句话的意思是，如果我们将盘的总质量分配给盘上的各个点，然后求得这些点的x坐标值的平均数，那么这个平均数就是盘的质心（或称为质量中心）的x坐标。

用中文解释这句话的话，就是：“通过将这个盘的总质量除以盘上各点的质量，我们可以得到盘上各点x坐标的平均值，这个平均值就是质心的x坐标。” 这种计算方法实际上就是求质心的过程。

在物理和数学中，质心就是一个物体质量分布的平均位置。如果你想找到一个二维物体（如盘）的质心，你需要分别找到x和y坐标的平均值。这个过程就是通过将每个点的x（或y）坐标乘以其质量，然后加起来，最后除以总质量，从而得到质心的x（或y）坐标。