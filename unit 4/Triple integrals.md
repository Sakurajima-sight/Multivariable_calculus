
--- pic\Triple integrals.pdf_00.png ---

1. Triple integrals.
   三重积分。

2. Triple integrals are the analog of double integrals for three dimensions.
   三重积分是三维情况下的双重积分。

3. They are a tool for adding up infinitely many infinitesimal quantities associated with points in a three-dimensional region.
   它们是一种工具，用于累加与三维区域内的点相关的无穷多个无穷小量。

4. Background:
   背景

1. Double integrals beyond volume.
超越体积的双重积分。

5. Make sure you have a solid grasp of double integrals before reading through this.
   在阅读这个之前，确保你对双重积分有深刻的理解。

6. The main difficulty in understanding multiple integrals is going from the concept of single integration, to that of double integration.
   理解多重积分的主要难度在于从单一积分的概念转变到双重积分的概念。

7. After that, as in the case of triple integrals, most of the mental effort goes towards applying the same principles to situations which are a bit trickier to visualize.
   之后，就像在三重积分的情况下，大部分的思考努力都会用于将相同的原理应用于稍微难以想象的情况。

8. What we're building to
   我们正在构建的

1.  An example three-dimensional region.
一个三维区域的例子。

9. At the risk of sounding obvious, triple integrals are just like double integrals, but in three dimensions.
   尽管这听起来很显然，但三重积分就像双重积分，只不过是在三个维度上。


--- pic\Triple integrals.pdf_01.png ---

1. $R$ is some region in three-dimensional space.
   $R$ 是三维空间中的某个区域。

1. $f(x, y, z)$ is some scalar-valued function which takes points in three-dimensional space as its input.
$f(x, y, z)$ 是一个标量值函数，它将三维空间中的点作为其输入。

2. $dV$ is a tiny unit of volume.
   $dV$ 是一个微小的体积单位。

3. In cartesian coordinates, this is expanded as $dV = dx\,dy\,dz$.
   在笛卡尔坐标中，这被扩展为 $dV = dx\,dy\,dz$。

4. Concretely, these are computed as three embedded integrals.
   具体地说，这些被计算为三个嵌入式积分。

2. This is a function purely of $y$ and $z$.
这是一个纯粹以 $y$ 和 $z$ 为变量的函数。

3. This is a function purely of $z$.
这是一个纯粹以 $z$ 为变量的函数。

5. As with double integrals, the bounds of inner integrals might be functions of the outer variables.
   就像双重积分一样，内积分的边界可能是外部变量的函数。

6. These bound functions are what encodes the shape of $R$.
   这些边界函数是编码 $R$ 的形状的内容。

7. Use a three-dimensional integral anytime you get that sensation of wanting to chop up a three-dimensional region into infinitely many pieces, associate each piece with a value, then add them all up.
   任何时候，当你有将三维区域切割成无穷多个片段，将每个片段与一个值关联，然后全部相加的感觉时，都可以使用三维积分。

8. One place where this is surprisingly useful is just finding the volume of three-dimensional regions by adding up all the tiny volumes $dV$.
   这种方法出奇地有用的一个地方就是通过累加所有的微小体积 $dV$ 来找到三维区域的体积。

9.  As with double integrals, the hard part is finding the right bounds which encode your region.
    和双重积分一样，难的部分是找到正确的边界来编码你的区域。

10. This just takes some practice, and a willingness to roll up your sleeves and dive into the muck of a problem.
    这只需要一些实践，以及愿意挽起袖子，深入到问题的混乱中去。

11. Example 1: Rectangular prism with variable density.
    示例1：具有变密度的长方体。

12. Suppose you have a block of metal in the shape of a rectangular prism with dimensions 3 x 2 x 5.
    假设你有一个金属块，形状为长方体，尺寸为3 x 2 x 5。

13. However, suppose its density is non-uniform.
    但是，假设其密度是不均匀的。

14. To be able to describe its density with a three-variable function, let's start by imagining this block in three-dimensional cartesian space.
    为了能够用三变量函数描述其密度，让我们首先想象这个块在三维笛卡尔空间中的样子。

抱歉，我之前没有正确地将变量转换为 LaTeX 格式。以下是经过更正后的文本：

--- pic\Triple integrals.pdf_02.png ---

1. Specifically, the block is positioned such that
   具体来说，这个方块的位置是这样的：

2. One corner is sitting at the origin.
   一个角位于原点。

3. One of its edges of length 3 rests on the positive $x$-axis.
   它的一个长度为3的边沿正$x$轴。

4. One of its edges of length 2 rests on the positive $y$-axis.
   它的一个长度为2的边沿正$y$轴。

5. One of its edges of length 5 rests on the positive $z$-axis.
   它的一个长度为5的边沿正$z$轴。

6. Let's say its density at each point is given using the function $\rho(x, y, z)$.
   假设其在每个点的密度由函数 $\rho(x, y, z)$ 给出。

7. (The Greek symbol $\rho$, pronounced "rho", is the typical variable used to represent three-dimensional density.)
   (希腊字母 $\rho$, 发音为 "rho"，是用来表示三维密度的典型变量。)

8. Key question: What is the mass of the entire block?
   关键问题：整个方块的质量是多少？

9. As with other integration problems, we start by imagining chopping up this region into many small pieces.
   就像其他的积分问题一样，我们开始时会想象把这个区域切成很多小块。

10. Unlike ordinary integrals, where you chop up a line to get tiny pieces of length $dx$, or double integrals, where you chop up a two-dimensional area to get tiny pieces of area $dA$, this time each tiny piece has some volume $dV$.
    不同于普通的积分，那里你将一条线切割成长度为 $dx$ 的小块，或者双重积分，那里你将一个二维区域切割成面积为 $dA$ 的小块，这次每个小块都有一些体积 $dV$。

11. Ultimately, this tiny volume will be broken down as the product of three tiny lengths, but as you set up the problem, it is helpful to just think about it as a little volume.
    最终，这个微小的体积将被分解为三个微小长度的乘积，但在你设定问题时，把它看作一个小体积是有帮助的。

12. Concretely, the way you might imagine chopping up this block into tiny pieces is by slicing it in three directions:
具体来说，你可能会想象通过三个方向切割这个方块来分割成小块：

13. Slice it with planes representing constant values of $x$.
用代表常数值的 $x$ 的平面来切割它。

14. Slice it with planes representing constant values of $y$.
用代表常数值的 $y$ 的平面来切割它。

15. Slice it with planes representing constant values of $z$.
用代表常数值的 $z$ 的平面来切割它。

--- pic\Triple integrals.pdf_03.png ---

1. Chop up 3x2x5 block.
   切割3x2x5的块。

2. Since $\rho(x, y, z)$ is a continuous function, when these tiny pieces are small enough, the density inside any one of them is pretty much constant.
   由于 $\rho(x, y, z)$ 是一个连续函数，当这些微小的部分足够小时，其中任何一个部分的密度基本上都是恒定的。

3. For example, as a particular piece shrinks around the point $(2, 1, 3)$, its overall density approaches $\rho(2, 1,3) = (2^2)(1)(\cos(\pi 3) + 2) = (4)(1)(1) = 4$.
   例如，当一个特定的部分在点 $(2, 1, 3)$ 周围收缩时，其总体密度接近 $\rho(2, 1,3) = (2^2)(1)(\cos(\pi 3) + 2) = (4)(1)(1) = 4$。

4. Therefore, the mass of one of these tiny pieces can be written as $\rho(x,y,z) \, dV$.
因此，这些微小部分中的一个的质量可以写成 $\rho(x,y,z) \, dV$。

5. Where $(x, y, z)$ is any point inside the piece, and $dV$ is the volume of the piece (the specifics of which are handled by the integral).
其中 $(x, y, z)$ 是部分内的任何点，而 $dV$ 是部分的体积（具体由积分处理）。

5. Each piece will be a tiny rectangular prism with side lengths $dz$, $dy$ and $dz$, the tiny linear changes in the $x$, $y$ and $z$-directions.
   每一部分都将是一个边长为 $dx$，$dy$ 和 $dz$ 的微小长方体，即 $x$，$y$ 和 $z$ 方向上的微小线性变化。

6. Therefore, the tiny volume is $dV = dx  dy  dz$.
   因此，微小体积是 $dV = dx  dy  dz$。

7. I think it's important to always think through why $dV$ can be expanded like this, thinking very concretely about the tiny rectangular prism and its edge lengths.
   我认为，总是要深思熟虑为何 $dV$ 可以像这样展开是非常重要的，要非常具体地想象这个微小的长方体及其边缘长度。

1. I say this because the way to expand it in other coordinate systems, such as cylindrical and spherical coordinate systems, is not so straightforward.
我之所以这么说，是因为在其他坐标系统中，如圆柱坐标系统和球坐标系统中，扩展它的方式并不那么直接。

2. Putting this together, the mass of one of our tiny pieces is 
将这些放在一起，我们微小部分的质量是

--- pic\Triple integrals.pdf_04.png ---

1. To add up all of these tiny masses, we set up three embedded integrals, each one integrating in the direction of a different coordinate axis. 
   为了加总所有这些微小的质量，我们设置了三个嵌套的积分，每一个都在不同的坐标轴方向进行积分。

2. Notice, the bounds on the inner integral reflect the $x$-values, since $dx$ Is written before $dy$ and $dz$.
   注意，内部积分的界限反映了 $x$ 的值，因为 $dx$ 写在 $dy$ 和 $dz$ 之前。

3. Similarly, the middle integral is bounded by $y$ values, since $dy$ is the second differential term listed, and the outer integral reflects the last term, $dz$.
   同样，中间的积分受 $y$ 值的限制，因为 $dy$ 是列出的第二个微分项，而外部积分反映了最后一个项，$dz$。

4. Concept check: Work through this triple integral.
概念检查：通过这个三重积分。

5. As a tip, you can keep things relatively tidy by factoring terms out of inner integrals as much as you can.
作为一个提示，你可以通过尽可能地将项从内部积分中提取出来，来保持事物相对整洁。


--- pic\Triple integrals.pdf_05.png ---

1. Home stretch! 
   冲刺阶段！

2. As you work through one of these computations, It's all-too easy to lose sight of what it represents.
   当你处理这些计算中的一个时，很容易忽视它代表的含义。

3. You can think of the innermost integral as adding up little bits of mass along lines parallel to the $x$-axis.
   你可以把最内层的积分想象成沿着与$x$轴平行的线段累积起来的一小部分质量。

4. It returns some expression of $y$ and $z$, which is a way of saying "Depending on the choice for the $y$ and $z$ coordinates of your line, which is parallel to the $x$-axis, this is what the sum of the infinitesimal masses along that line will be."
   它返回关于 $y$ 和 $z$ 的一些表达式，这其实是在说：“根据你的线（与$x$轴平行）的 $y$ 和 $z$ 坐标的选择，这就是沿着该线的无穷小质量之和”。

5. The next integral, with respect to $y$, adds up the infinitesimal masses of those lines in the $y$-direction, giving the infinitesimal mass of a sheet parallel to the $xy$-plane.
   下一个关于 $y$ 的积分，累加了那些在 $y$ 方向上的线段的无穷小质量，得到了一个与 $xy$ 平面平行的薄片的无穷小质量。

6. It will return an expression purely in terms of $z$, which says "Depending on the height of your sheet above the $xy$-plane, this is what its infinitesimal mass will be".
   它将返回一个纯粹关于 $z$ 的表达式，即“根据你的薄片在 $xy$ 平面之上的高度，这就是它的无穷小质量”。

7. Finally, the outermost integral adds up the masses of these sheets as $z$ ranges from 0 to 5.
   最后，最外层的积分将这些薄片的质量累加起来，当 $z$ 的取值范围从 0 到 5。

8. It returns a constant, which is the (no-longer-infinitesimal) mass of the block of metal as a whole.
   它返回一个常数，这就是整个金属块的（不再是无穷小的）质量。

--- pic\Triple integrals.pdf_06.png ---

1. Example 2: Using a triple integral to compute volume.
示例 2：使用三重积分计算体积。

2. You have seen how double integrals can compute the volume under the graph of a two-variable function.
你已经看到了双重积分如何计算两变量函数图下的体积。

2. Indeed, for most of the regions you might be able to think up, if you are clever enough you can probably figure a way to compute the volume using some kind of double integral.
   的确，对于你可能想到的大多数区域，如果你足够聪明，你可能会想出某种方式使用双重积分计算体积。

3. Remember, the reason double integrals could compute volume is because they took tiny pieces on the xy-plane, with area $dA$, and multiplied each one by the height of the function above that point, $f(x, y)$, which gave the infinitesimal volume of a column above the piece with area $dA$ and below the graph.
   请记住，双重积分能够计算体积的原因是它们在 $xy$-平面上取得微小的片段，面积为 $dA$，并将每一个都乘以该点上方的函数的高度 $f(x, y)$，这给出了面积为 $dA$ 的片段上方和图形下方的柱体的无穷小体积。

4. Tiny columns of volume.
   体积的微小柱体。

5. With triple integrals, we have a stronger tool which can scan through an entire region and add up tiny units of volume as it goes. 
   使用三重积分，我们有了一个更强大的工具，可以扫描整个区域并在过程中累加微小的体积单位。

6. If for no other reason, doing this can be very good practice for putting bounds on a triple integral without getting bogged down by the function inside.
   如果没有其他原因，这将是一个很好的实践，可以在不被内部函数困扰的情况下对三重积分设置边界。

7. For example, consider the region $R$ bounded by the following two surfaces:
例如，考虑由以下两个表面围成的区域 $R$：

8. The paraboloid $z = x^2+y^2$.
抛物面 $z = x^2+y^2$。

9. The plane $z = 2(x + y+ 1)$.
平面 $z = 2(x + y+ 1)$。

8. Here's what those two surfaces look like:
   这就是这两个表面的样子：

--- pic\Triple integrals.pdf_07.png ---

1. Surfaces $z=x^2+y^2$ and $z=2(x+y+1)$
   表面 $z=x^2+y^2$ 和 $z=2(x+y+1)$

1. And here's what the three-dimensional region $R$ bound between them looks like:
这就是它们之间的三维区域$R$的样子：

2. Region between $x^2+y^2$ and $2(x+y+1)$
区域在 $x^2+y^2$ 和 $2(x+y+1)$ 之间。

3. To find its volume, we start by setting up a deceptively simple looking integral which will add up the volume of all the little pieces you might cut this region into.
   为了找到它的体积，我们首先设置一个看似简单的积分，这个积分将累计所有你可能将这个区域切割成的小块的体积。

4. All of the difficulty lies in setting up the right bounds of these three integrals to accurately encode the region $R$.
所有的难度都在于设置这三个积分的正确界限，以准确地编码区域$R$。

5. From the definition of $R$, we get the bounds of $z$ for free:
从$R$的定义中，我们得到了$z$的界限。


--- pic\Triple integrals.pdf_08.png ---

1. Since the bounds of $z$ are given as functions of $x$ and $y$, this suggests that the inner-most integral of our triple integral should be with respect to $z$.
   由于$z$的界限是$x$和$y$的函数，这暗示我们的三重积分的最内部积分应该是关于$z$的。

1. We might start writing the triple integral as follows.
   我们可能会开始像下面这样写三重积分。

2. Inner integral is with respect to $Z$.
   最内部的积分是关于$Z$的。

3. But what do we put for the bounds of the outer two integrals?
   但是我们在外面两个积分的边界上放什么呢？

4. How far out can $x$ and $y$ go?
   $x$和$y$可以到多远？

5. For this, we must analyze where the two surfaces defining $R$ intersect.
   为了这个，我们必须分析定义$R$的两个表面在哪里相交。

6. This intersection is a closed loop in three-dimensional space, pictured as a red line below.
   这个交点是三维空间中的一个闭环，如下图的红线所示。

7. Now imagine projecting the entire region $R$ onto the $x$-$y$ plane, which is a way of just focusing on which values of $x$ and $y$ matter.
   现在想象将整个区域$R$投影到$x$-$y$平面，这只是关注哪些$x$和$y$的值有意义的一种方式。

--- pic\Triple integrals.pdf_09.png ---

1. Projection of region onto $xy$ plane.
   将区域投影到$xy$平面。

2. The red loop marking the intersection between $z = 2x^{2} + y^{2}$ and $z = 2(x + y +1)$ becomes the boundary of the region in the $x$-$y$-plane that we care about.
   红线标记的是$z = 2x^{2} + y^{2}$和$z = 2(x + y +1)$之间的交点，这成为了我们在$x$-$y$平面上关心的区域的边界。

3. This is all visual, but to find the analytic description of this curve, set the equations defining each of our two surfaces equal to each other: 
   这一切都是可视的，但要找到这条曲线的分析描述，就需要将定义我们两个表面的等式设定为相等：

4. By completing the square for both $x$ and $y$, we can get an expression which is easier to geometrically interpret. 
   通过对$x$和$y$都完成平方，我们可以得到一个更容易从几何角度解释的表达式。

5. Perfect square.
   完全平方。

6. Equation for a circle.
   这是一个圆的等式。

1. Concept check: What shape does this equation describe?
   概念检查：这个等式描述的是什么形状？

2. Choose 1 answer:
   选择1个答案：

--- pic\Triple integrals.pdf_10.png ---

1. The equation $(x - 1)^2 + (y - 1)^2 = 4$ represents a circle centered at $(1, 1)$ with radius $\sqrt{4} = 2$.
   方程式 $(x - 1)^2 + (y - 1)^2 = 4$ 代表一个以$(1, 1)$为中心，半径为$\sqrt{4} = 2$的圆。

2. To describe how $x$ and $y$ range over this region, you can either break it up into vertical stripes or horizontal stripes.
   要描述$x$和$y$如何在这个区域内变化，你可以将其划分为竖直条纹或水平条纹。

3. For no particular reason, I'll choose horizontal stripes.
   没有特别的原因，我选择水平条纹。

--- pic\Triple integrals.pdf_11.png ---

2. We encode the fact that the vertical position of the stripes. ranges from − 1 to 3 by making these the bounds of y.
我们通过将 $y$ 的界限设定为从 $-1$ 到 $3$，来表示条纹的垂直位置的范围。

2. The bounds for $x$, which describe the left and right ends of each horizontal stripe in our circle, are the two solutions for $x$ in the equation defining the circle.
   描述我们圆内每个水平条纹的左右端点的$x$的界限是定义圆的方程中的两个$x$的解。

3. This means our final integral looks like this:
   这意味着我们的最终积分看起来像这样：

4. Isn't that absurd?
   这不荒谬吗？

5. Welcome to the world of triple integrals.
   欢迎来到三重积分的世界。


--- pic\Triple integrals.pdf_12.png ---

1. As a reminder, it's super important to write the differential terms in the right order, in this case, the order is $dz$ $dx$ $dy$. 
   提醒一下，按正确的顺序编写微分项非常重要，在这种情况下，顺序是 $dz$ $dx$ $dy$。

2. The bounds of inner integral describe $z$ -values, so $dz$ Is listed first, the next integral runs over $x$-values, so $dx$ Is listed second, etc.
   内部积分的界限描述 $z$ 值，所以首先列出 $dz$，下一个积分运行在 $x$ 值上，所以 $dx$ 列在第二，等等。

3. The main skill to practice here is setting up the integral, as we have now done.
   在这里需要练习的主要技能是设置积分，就像我们现在所做的那样。

4. From there, a computer can handle it.
   从那里开始，电脑可以处理它。

5. But if you want to practice computing one of these triple integrals, by all means, go for it.
   但是，如果你想练习计算这些三重积分中的一个，那就尽管去做。

6. This particular integral gets out of hand rather quickly.
   这个特定的积分很快就会失控。

7. Example 3: Volume of a conical region.
   示例3：圆锥形区域的体积。

1. Problem: Setup a triple integral which will find the volume of a region $R$ defined by the following properties.
   问题：设置一个三重积分，它将找到由以下属性定义的区域 $R$ 的体积。

2. Here's what this region looks like.
   这个区域看起来像这样。


--- pic\Triple integrals.pdf_13.png ---

1. Region between $y=0$ and $y=2-\sqrt{x^2+z^2}$.
   区域在$y=0$和$y=2-\sqrt{x^2+z^2}$之间。

2. “But wait, I hear you say, "I already know how to compute the volume of a cone!
   “等等，我听到你说，“我已经知道如何计算锥体的体积了！

3. That's fine, but seeing how to find that volume with a triple integral will be a good way to stretch our triple integral muscles.
   这很好，但是看看如何用三重积分找到那个体积将是锻炼我们三重积分能力的好方法。

1. Concept check: The region $R$ is defined using bounds for $y$, so which of the following is a valid way to start setting up the integral?
概念检查：区域$R$是用$y$的界限定义的，那么以下哪种方法是开始设置积分的有效方法呢？ 

2. Choose 1 answer:
选择1个答案：


--- pic\Triple integrals.pdf_14.png ---

1. The third choice is correct: 
   第三个选择是正确的：

2. Since the upper bound of $y$ is given as a function of $x$ and $z$, the integral handling $y$ must be inside the integrals handling $x$ and $z$.
   由于$y$的上界是作为$x$和$z$的函数给出的，处理$y$的积分必须在处理$x$和$z$的积分内部。

3. This way, the variables $x$ and $z$ can be integrated out as we work through the middle and outer integrals.
   这样，当我们处理中间和外部积分时，变量$x$和$z$可以被积分出来。

4. Concept check: Given the two constraints defining our region, $y \geq 0$ and $y \leq 2-\sqrt{x^2+z^2}$, how can you find the values of $x$ and $z$ within $R$? 
概念检查：给定定义我们区域的两个约束条件，$y \geq 0$ 和 $y \leq 2-\sqrt{x^2+z^2}$，你如何找到 $R$ 中的 $x$ 和 $z$ 的值？

2. Let $R_{xz}$ be the set of all points $(x, z)$ such that $(x, y, z)$ is a point in $R$ for some value of $y$.
让 $R_{xz}$ 是所有点 $(x, z)$ 的集合，使得 $(x, y, z)$ 是 $R$ 中的某个 $y$ 值的点。

1. $R_{xz}$ is bounded by the curve described by the equation $0=2-\sqrt{x^2+z^2}$.
$R_{xz}$ 被方程 $0=2-\sqrt{x^2+z^2}$ 描述的曲线所限定。

1. The second choice is correct.
第二个选择是正确的。

2. The hard part of this question is just parsing what is being said (as happens so often in math).
这个问题的难点就是解析所说的内容（这在数学中经常发生）。

2.  To be clear about what the question is asking, imagine projecting the region $R$ onto the $xz$-plane.
    为了清楚地理解这个问题的要求，想象一下将区域$R$投影到$xz$平面上。


--- pic\Triple integrals.pdf_15.png ---

1. This will give you all of the values $(x, z)$ such that there was a point $(x,y, z)$ inside $R$ for some value of $y$.
这将给出所有的值 $(x, z)$，以致于在一些 $y$ 的值下，点 $(x, y, z)$ 在 $R$ 内。

1. For example, the value $(x, z) = (0, 1)$ is inside this projection, because the point $(0, 0.75, 1)$, to take one of many examples, is inside $R$.
例如，值 $(x, z) = (0, 1)$ 在这个投影内，因为点 $(0, 0.75, 1)$，举其中一个例子，是在 $R$ 内的。

1. However, the value $(3, 4)$ is not inside this projection, because there is no value of $y$ such that $(3, y, 4)$ is inside $R$.
然而，值 $(3, 4)$ 不在这个投影内，因为没有 $y$ 的值使得点 $(3, y, 4)$ 在 $R$ 内。

1. The boundary of this two-dimensional region on the $xz$-plane is determined by where the condition $y = 0$ meets with the condition $y =2-\sqrt{x^2+z^2}$.
这个二维区域在 $xz$ 平面上的边界是由 $y = 0$ 的条件与 $y =2-\sqrt{x^2+z^2}$ 的条件相交的地方确定的。

1. In other words, the boundary is given by the equation $0=2-\sqrt{x^2+z^2}$.
换句话说，边界由方程 $0=2-\sqrt{x^2+z^2}$ 给出。

1. Concept check: Based on the answer to the previous question, which of the following describes the region on the $xz$-plane that captures all values of $z$ and $x$ that our triple integral needs to cover.
概念检查：基于对前一个问题的回答，下列哪个选项描述了 $xz$ 平面上的区域，捕获了我们的三重积分需要覆盖的所有 $z$ 和 $x$ 的值。

1. The region inside a circle of radius  2.
   在半径为 2 的圆内的区域。

--- pic\Triple integrals.pdf_16.png ---

1. The third answer choice is correct: The region inside a circle of radius 1.
   第三个答案选项是正确的：半径为1的圆内的区域。

2. As I described in the answer to the last question, the relevant region of the $xz$ plane has a boundary described by the equation $0=2-\sqrt{x^2+z^2}$.
   正如我在上一题的答案中描述的，$xz$ 平面的相关区域的边界由方程 $0=2-\sqrt{x^2+z^2}$ 描述。

3. This describes a circle of radius 2.
这描述了一个半径为2的圆。

4. But remember, this is just the boundary of the region in the $xz$-plane that we care about; most of the points $(x, z)$ that our triple integrals needs to cover lie within this region.
但是记住，这只是我们关心的$xz$平面区域的边界；我们的三重积分需要涵盖的大多数点$(x, z)$都位于这个区域内。

4. Concept check: Which of the following shows the right way to set up our volume integral? 
   概念检查：以下哪一项展示了设置我们体积积分的正确方式？

--- pic\Triple integrals.pdf_17.png ---

1. The first choice is correct. 
   第一个选择是正确的。

2. This corresponds to breaking up the circle in the $xz$-plane into horizontal stripes.
   这对应于将$xz$平面上的圆分成水平条纹。

3. Within each stripe, $x$ ranges from $-\sqrt{4-z^2}$ to $\sqrt{4-z^2}$, and the height of the stripes themselves ranges from $z=-2$ to $z=2$.
   在每个条纹内，$x$的范围从$-\sqrt{4-z^2}$到$\sqrt{4-z^2}$，条纹本身的高度范围从$z=-2$到$z=2$。

4. Therefore, the bounds on the outer integrals look like this:  
   因此，外层积分的界限如下：

以下是我对你提供的段落的处理：

--- pic\Triple integrals.pdf_18.png ---

1. Summary:
   摘要：

2. Triple integrals are written abstractly as $\iiint_R f dV$
三重积分抽象地写作 $\iiint_R f dV$

1. $R$ is some region in three-dimensional space.
   $R$ 是三维空间中的某个区域。

2. $f(x, y, z)$ is some scalar-valued function which takes points in three-dimensional space as its input.
$f(x, y, z)$ 是一个标量值函数，它将三维空间中的点作为其输入。

1. $dV$ is a tiny unit of volume.
   $dV$ 是一个微小的体积单位。

2. In cartesian coordinates, this is expanded as $dV = dx\,dy\,dz$.
   在笛卡尔坐标中，这被扩展为 $dV = dx\,dy\,dz$。

3. Concretely, these are computed as three embedded integrals.
   具体地说，这些被计算为三个嵌入式积分。

4. This is a function purely of $y$ and $z$.
这是一个纯粹以 $y$ 和 $z$ 为变量的函数。

1. This is a function purely of $z$.
这是一个纯粹以 $z$ 为变量的函数。

1. As with double integrals, the bounds of inner integrals might be functions of the outer variables.
   就像双重积分一样，内积分的边界可能是外部变量的函数。


2. Use a three-dimensional integral anytime you get that sensation of wanting to chop up a three-dimensional region into infinitely many pieces, associate each piece with a value, then add them all up.
   任何时候，当你有将三维区域切割成无穷多个片段，将每个片段与一个值关联，然后全部相加的感觉时，都可以使用三维积分。

3. One place where this is surprisingly useful is just finding the volume of three-dimensional regions by adding up all the tiny volumes $dV$.
   这种方法出奇地有用的一个地方就是通过累加所有的微小体积 $dV$ 来找到三维区域的体积。

4.  As with double integrals, the hard part is finding the right bounds which encode your region.
    和双重积分一样，难的部分是找到正确的边界来编码你的区域。

5.  This just takes some practice, and a willingness to roll up your sleeves and dive into the muck of a problem.
    这只需要一些实践，以及愿意挽起袖子，深入到问题的混乱中去。