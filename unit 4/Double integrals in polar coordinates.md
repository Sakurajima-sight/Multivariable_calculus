

--- pic\Double integrals in polar coordinates.pdf_00.png ---

1. Double integrals in polar coordinates.
   极坐标下的二重积分。

2. If you have a two-variable function described using polar coordinates, how do you compute its double integral?
   如果你有一个用极坐标描述的两变量函数，你如何计算它的双重积分？

1. Background
背景

2. Polar coordinates (video)
极坐标（视频）

3. Double integrals beyond volume
超越体积的双重积分

3. What we're building to.
   我们正在建立的内容。

4. When you are performing a double integral, $\iint f dA$.
   当你正在执行一个双重积分，$\iint f dA$。

5. If you wish to express the function $f$ and the bounds for the region $R$ in polar coordinates $(r, \theta)$, the way to expand the tiny area $dA$ is $dA = r d\theta dr$.
   如果你希望用极坐标 $(r, \theta)$ 表示函数 $f$ 和区域 $R$ 的边界，扩大微小面积 $dA$ 的方法是 $dA = r d\theta dr$。

6. Pay attention to the fact that the variable $r$ is part of this expression.
   注意到变量 $r$ 是这个表达式的一部分。

7. Beyond that one rule, these double integrals are mostly about being careful to make sure the bounds of your integrals appropriately encode the region $R$.
   除了这个规则，这些双重积分主要是要小心，确保你的积分的边界适当地编码了区域 $R$。

8. Integrating using polar coordinates is handy whenever your function or your region have some kind of rotational symmetry.
   每当你的函数或你的区域有某种旋转对称性时，使用极坐标进行积分都是方便的。

9. For example, polar coordinates are well-suited for integration in a disk, or for functions including the expression $x^2+y^2$.
   例如，极坐标非常适合在磁盘中进行积分，或对包含表达式 $x^2+y^2$ 的函数进行积分。

10. Example 1: Tiny areas in polar coordinates.
    例 1：极坐标中的微小区域。

11. Suppose we have a multivariable function defined using the polar coordinates $r$ and $\theta$, $f(r,\theta) = r^2$.
    假设我们有一个用极坐标 $r$ 和 $\theta$ 定义的多变量函数，$f(r,\theta) = r^2$。

--- pic\Double integrals in polar coordinates.pdf_01.png ---

1. And let's say you want to find the double integral of this function in the region where $r\leq2$.
   假设你想找到这个函数在区域 $r\leq2$ 中的双重积分。

2. This is a disc of radius 2 centered at the origin.
   这是一个半径为2，中心在原点的圆盘。

3. Written abstractly, here's what this double integral might look like: 
   抽象地写出来，这个双重积分可能看起来像这样：

4. You could interpret this as the volume underneath a paraboloid (the three-dimensional analog of a parabola), as pictured below:
   你可以将其解释为抛物面（抛物线的三维类比）下方的体积，如下图所示：

--- pic\Double integrals in polar coordinates.pdf_02.png ---

1. The question is, what do we do with that $dA$ term?
   问题是，我们应该如何处理这个 $dA$ 项？

2. Warning! You might be tempted to replace $dA$ with $d\theta dr$, since in cartesian coordinates we replace it with $dx dy$.
   警告！你可能会试图将 $dA$ 替换为 $d\theta dr$，因为在笛卡尔坐标系中，我们将其替换为 $dx dy$。

3. But this is not correct!
   但这是不正确的！

4. Remember what a double integral is doing: It chops up the region that we are integrating over into tiny pieces, and $dA$ represents the area of each one of those pieces.
   记住双重积分在做什么：它将我们积分的区域切成微小的片段，而 $dA$ 表示每一个片段的面积。

4. For example, chopping up our disc of radius 2 might look like this: 
   例如，将我们的半径为2的圆盘切成如下的样子：

5. Why did I choose to chop it in this spiderweb pattern, as opposed to using vertical and horizontal lines?
   为什么我选择用这种蜘蛛网图案来切割，而不是使用垂直和水平线条呢？

1. Since we are in polar coordinates, it will be easiest to think about the tiny pieces if their edges represent either a constant $r$ value or a constant $\theta$ value.
由于我们处于极坐标系，如果它们的边缘表示常数 $r$ 值或常数 $\theta$ 值，那么考虑这些微小部分将是最容易的。

--- pic\Double integrals in polar coordinates.pdf_03.png ---

1. Let's focus on just one of these little chunks: 
   我们只关注这些小块中的一个：

2. Even though this little piece has a curve shape, if we make finer and finer cuts, we can basically treat it as a rectangle.
   尽管这小块呈曲线状，但如果我们进行越来越细的切割，我们基本上可以将其视为一个矩形。

3. The length of one side of this "rectangle" can be thought of as $dr$, a tiny change in the $r$-coordinate.
   这个"矩形"的一边的长度可以被看作是 $dr$，即 $r$-坐标的一个微小变化。

4. Using a differential $dr$ to describe this length emphasizes the fact that we are not really considering a specific piece, but instead we care about what happens as its size approaches 0.
   使用微分 $dr$ 来描述这个长度强调了一个事实，那就是我们并没有真正考虑一个特定的部分，而是关心的是当其大小趋近于0时会发生什么。

--- pic\Double integrals in polar coordinates.pdf_04.png ---

1. But how long is the other side?
   但是另一边有多长呢？

2. It's not $d\theta$, a tiny change in the angle, because radians are not a unit of length.
   它不是$d\theta$，也就是角度的微小变化，因为弧度不是长度单位。

2. To turn radians into a bit of arc length, we must multiply by $r$.
   要将弧度转换为一点弧长，我们必须乘以$r$。

3. Therefore, if we treat this tiny chunk as a rectangle, and as $dr$ and $d\theta$ each approach 0 it basically is a rectangle, its area is $dA = (r d\theta)(dr)$.
   因此，如果我们把这个微小的块当作一个矩形，当$dr$和$d\theta$都接近0时，它基本上就是一个矩形，它的面积是$dA = (r d\theta)(dr)$。

4. Plugging this into our original integral, we get 
   将这个插入我们原来的积分，我们得到 

5. Putting bounds on this region is relatively straight-forward in this example, because circles are naturally suited for polar coordinates.
   在这个例子中，对这个区域设定界限相对直接，因为圆形自然适合极坐标。

6. Since we wrote $d\theta$ in front of $dr$, the inner integral is written with respect to $\theta$.
   由于我们在$dr$前面写了$d\theta$，所以内积分是关于$\theta$的。

7. The bounds of this inner integral will reflect the full range of $\theta$ as it sweeps once around the circle, going from 0 to $2\pi$.
   这个内积分的边界将反映$\theta$在环绕圆形一周时的全范围，从0到$2\pi$。

8. The outer integral is with respect to $r$, which ranges from 0 to 2.
   外积分是关于$r$的，它的范围从0到2。

9. Concept check: Evaluate this double integral
概念检查：计算这个双重积分

--- pic\Double integrals in polar coordinates.pdf_05.png ---

1. $r^3$ can be factored out of the inner integral with respect to $\theta$.
   $r^3$ 可以从关于 $\theta$ 的内积分中提取出来。

2. Example 2: Integrating over a flower.
   示例 2：在花朵上进行积分。

3. Define a two-variable function $f$ in polar coordinates as $f(r, \theta) = r\sin(\theta)$.
   在极坐标中定义一个两变量函数 $f$，使 $f(r, \theta) = r\sin(\theta)$。

--- pic\Double integrals in polar coordinates.pdf_06.png ---

1. Let $R$ be flower-shaped region, defined by $r \leq \cos(2\theta)$.
   定义 $R$ 为花形区域，由 $r \leq \cos(2\theta)$ 确定。

2. Solve the double integral $\iint_R f dA$.
   求解双重积分 $\iint_R f dA$。

3. Step 1: Which of the following represents the right way to replace $f dA$ in the abstractly written double integral? 
   步骤1：以下哪个选项正确地代表了在抽象表述的双重积分中替换 $f dA$ 的正确方式？

1. Choose 1 answer: 
选择一个答案：

1. The second choice is correct: 
   第二个选择是正确的：

1. The function $f$ is defined as $r \sin(\theta)$, and the term $dA$ is expanded as $r d\theta dr$ (don't forget to add the $r$ term here).
函数 $f$ 定义为 $r \sin(\theta)$，并且 $dA$ 项扩展为 $r d\theta dr$（这里不要忘记添加 $r$ 项）。


2. Step 2: Now we must encode the fact that $R$ is defined as the region where $r \leq \cos(2\theta)$.
   步骤2：现在我们必须编码 $R$ 定义为满足 $r \leq \cos(2\theta)$ 的区域这一事实。


2. Which of the following is the right way to put bounds on the double integral?
以下哪种是在双重积分上设置边界的正确方式？

--- pic\Double integrals in polar coordinates.pdf_07.png ---

1. Choose 1 answer: 
   选择一个答案：

2. The first answer choice is correct $\int_{0}^{2\pi} \int_{0}^{\cos(2\theta)} r^{2} \sin(\theta) dr d\theta$.
   第一个答案选项是正确的 $\int_{0}^{2\pi} \int_{0}^{\cos(2\theta)} r^{2} \sin(\theta) dr d\theta$。

1. The inner integral reflects $r$ bounds, since $dr$ is written before $d\theta$.
内积分反映了 $r$ 的界限，因为 $dr$ 写在 $d\theta$ 之前。

2. Our region is explicitly defined such that $r \leq \cos(2\theta)$, and since these are polar coordinates, $r$ can only ever be positive.
我们的区域明确定义为 $r \leq \cos(2\theta)$，并且由于这些是极坐标，$r$ 只能永远是正的。

3. Therefore, $r$ ranges from $0$ to $\cos(2\theta)$.
因此，$r$ 的范围从 $0$ 到 $\cos(2\theta)$。

4. For the outer integral, $\theta$ ranges over its full range from $0$ to $2\pi$, since no constraints are given on $\theta$ in the definition of $R$.
   对于外积分，$\theta$ 的范围从 $0$ 到 $2\pi$，因为在定义 $R$ 时没有给出 $\theta$ 的约束。

5. Step 3: Solve this integral.
   步骤3：解这个积分。

--- pic\Double integrals in polar coordinates.pdf_08.png ---

1. In practice, I would use a calculator or Wolfram Alpha to solve one of these integrals.
   实际操作中，我会使用计算器或 Wolfram Alpha 来解决这其中的一个积分。

2. The hard part, which typically requires more human intelligence, is getting the double integral to the point where all the terms are in place.
   难点，通常需要更多的人类智慧，是将双重积分推进到所有项都到位的地方。

3. If you want to solve it by hand, here's how it might go.
   如果你想手动解决它，这可能是怎么做的。

1. Factor out sin ( θ ) from r -integral
从 $r$-积分中提取出 $\sin(\theta)$。

4. From here, we can save a lot of computational trouble with an observation: The inside of the integral is an odd function, meaning that when you replace $\theta$ by $-\theta$, the value of the expression as a whole becomes negative.
   从这里，我们可以通过一个观察省去很多计算麻烦：积分内部是一个奇函数，意味着当你用 $-\theta$ 替换 $\theta$ 时，整个表达式的值变为负数。

5. Also, since these trigonometric functions are periodic, integrating between 0 and $2\pi$ is the same as integrating between $-\pi$ and $\pi$.
   同样，由于这些三角函数是周期函数，所以在 0 和 $2\pi$ 之间积分与在 $-\pi$ 和 $\pi$ 之间积分是一样的。

6. The integral on the negative half cancels out with the integral on the positive portion, so in total it is 0.
   负半部分的积分与正半部分的积分抵消，所以总共是0。

--- pic\Double integrals in polar coordinates.pdf_09.png ---

1. Example 3: The bell curve.
   示例3：钟形曲线。

1. Are you ready for one of my favorite results in math?
你准备好看我最喜欢的数学结果之一了吗？

2. This is really quite clever.
这真的非常巧妙。

3. Question: What is the integral $\int_{-\infty}^{\infty} e^{-x^2} \, dx$? 
   问题：积分 $\int_{-\infty}^{\infty} e^{-x^2} \, dx$ 的结果是什么？

4. This single integral is hard-to-impossible to compute directly.
这个单独的积分直接计算几乎是不可能的。

5. Just try to find the antiderivative!
试试看找到反导数吧！

5. This integral is asking about the area under a bell curve, which turns out to be super important for probability and statistics!
   这个积分是在询问钟形曲线下的面积，这对概率和统计学来说非常重要！

--- pic\Double integrals in polar coordinates.pdf_10.png ---

1. What does this have to do with double integrals in polar coordinates?
这与极坐标下的双重积分有什么关系呢？

1. I hear you, my inquisitive friend, it does seem unrelated, doesn't it?
我听到你了，我的好奇朋友，这似乎没有关系，不是吗？

2. Well, this is where someone got super clever.
嗯，这就是有人变得超级聪明的地方。

2. Surprisingly, it is easier to solve this multi-dimensional analog of this problem.
   令人惊讶的是，解决这个问题的多维模拟更容易。

3. Namely, find the volume under a three-dimensional bell curve over the entire $xy$-plane.
   也就是说，在整个 $xy$ 平面上找到一个三维钟形曲线下的体积。

4. If we keep everything in cartesian coordinates, this is as hard to solve as the original single integral. 
   如果我们将一切保持在笛卡尔坐标中，解决这个问题就像解决原始单个积分一样困难。

5. However, something magical happens when we convert to polar coordinates.
   然而，当我们转换为极坐标时，会发生一些神奇的事情。

6. Concept check: Express this double integral using polar coordinates.
   概念检查：使用极坐标表示这个双重积分。

--- pic\Double integrals in polar coordinates.pdf_11.png ---

1. Choose 1 answer: 
   选择1个答案：

2. The second answer choice is correct.
   第二个答案选择是正确的。

1. First, make the following two conversions $x^2 + y^2 \rightarrow r$ and $dy dx \rightarrow r d\theta dr$
首先，进行以下两个转换：$x^2 + y^2 \rightarrow r$ 和 $dy dx \rightarrow r d\theta dr$

2. Polar form of $dA$
$dA$的极坐标形式

3. So our integral looks like this: 
   所以我们的积分看起来是这样的：

4. To put bounds on the integral, we cover the entire plane by letting $\theta$ range from 0 to $2\pi$, and $r$ range from 0 to $\infty$. 
   为了对积分进行界定，我们让 $\theta$ 从0到 $2\pi$，$r$ 从0到 $\infty$ 来覆盖整个平面。

5. Since the inner integral is with respect to $\theta$, we can factor out everything with an $r$ in it, which in this case is the entire function:
   由于内积分是关于 $\theta$，我们可以将所有包含 $r$ 的项提出来，在这种情况下，这是整个函数。

--- pic\Double integrals in polar coordinates.pdf_12.png ---

1. This evaluates to $2 \pi$.
   这个结果为 $2 \pi$。


2. Concept check: Find the antiderivative of $e^{-r^2}r$, using either $u$-substitution or the inverse chain rule.
   概念检查：找出 $e^{-r^2}r$ 的原函数，可以使用 $u$-代换法或反链式法则。

3. Using $u$-substitution: 
   使用 $u$-代换法：

2. Define $u$ as $u = -r^2$ which means $du = -2r dr$
定义 $u$ 为 $u = -r^2$，这意味着 $du = -2r dr$。

1. Our indefinite integral now becomes
   我们的不定积分现在变为 

2. Substituting back to $u = -r^2$.
   把 $u = -r^2$ 代回进去。


3. Substituting back to $u = -r$, this means our final antiderivative is
将 $u$ 替换回 $-r$，这意味着我们的最终原函数是

--- pic\Double integrals in polar coordinates.pdf_13.png ---

1. Notice, the reason you can now find an antiderivative is because of that little $r$ term that showed up due to the fact that $dA = r d\theta dr$.
   注意，现在你可以找到一个反导数的原因是因为由于 $dA = r d\theta dr$，出现了一个小的 $r$ 项。

2. Concept check: Using this antiderivative, finish solving the integral which computes volume under a three-dimensional bell curve.
   概念检查：使用这个反导数，完成计算三维钟形曲线下体积的积分。

3. Isn't that a beautiful answer?
   这不是一个美丽的答案吗？

4. It gets better, you can use this multi-dimensional result to solve the original single integral.
   更好的是，你可以使用这个多维结果来解决原始的单一积分。

5. Can you see how?
   你能看出怎么做吗？

1. Let $C=\int_{-\infty}^{\infty} e^{-x^2} \, dx$ , and try to solve the double integral $\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} e^{-(x^2+y^2)} \, dx dy$ in terms of C
设定 $C=\int_{-\infty}^{\infty} e^{-x^2} \, dx$，并尝试将双重积分 $\int_{-\infty}^{\infty} \int_{-\infty}^{\infty} e^{-(x^2+y^2)} \, dx dy$ 表示为 $C$ 的函数。

--- pic\Double integrals in polar coordinates.pdf_14.png ---

1. Following the hint, start by saying $C=\int_{-\infty}^{\infty} e^{-x^2} \, dx$.
   遵循提示，开始时我们说 $C=\int_{-\infty}^{\infty} e^{-x^2} \, dx$。

2. Now, as we start chewing on the double integral in cartesian coordinates, even though it cannot be solved directly the way it was in polar form, we can start writing things in terms of $C$. 
   现在，当我们开始处理笛卡尔坐标中的双重积分时，尽管我们不能像极坐标形式那样直接解决它，我们可以开始用 $C$ 来表示一些事物。

3. This equals $C$.
   这等于 $C$。

4. This also equals $C$.
   这也等于 $C$。

5. In other words, even if we don't know what the area under a bell curve is, we know that when you square it, you get the volume under a three-dimensional bell curve. 
   换句话说，即使我们不知道钟形曲线下的面积是多少，我们知道当你平方它时，你会得到三维钟形曲线下的体积。

6. But we just solved the volume under three-dimensional bell curve using polar-coordinate integration!
但是我们刚刚使用极坐标积分解决了三维钟形曲线下的体积问题！

7. We found that the volume was $\pi$.
我们发现体积是 $\pi$。

8. Therefore, the original integral is $\sqrt{\pi}$.
因此，原积分是 $\sqrt{\pi}$。

9. Isn't that crazy?
这不是疯了吗？

8. This expression looks like it has nothing to do with $x$ and circles, yet somehow it does. 
   这个表达式看起来与 $x$ 和圆无关，然而某种程度上它确实有关。

9. This is just one more of the many places in nature where $x$ and $e$ are connected.
   这只是自然界中 $x$ 和 $e$ 连接的许多地方之一。

--- pic\Double integrals in polar coordinates.pdf_15.png ---

1. The only real thing to remember about double integral in polar coordinates is that $dA = r dr d\theta$.
   关于极坐标下的双重积分，唯一真正需要记住的是 $dA = r dr d\theta$。

2. Beyond that, the tricky part is wrestling with bounds, and the nastiness of actually solving the integrals that you get.
   除此之外，棘手的部分是处理界限，以及实际解决你得到的积分的困难。

3. But those are the same difficulties one runs into with cartesian double integrals.
   但是这些都是在处理笛卡尔双重积分时会遇到的同样的困难。

4. The reason this is worth learning is that sometimes double integrals become simpler when you phrase them with polar coordinates, as was the case in the bell curve example.
   学习这个的原因是，有时当你用极坐标表示它们时，双重积分会变得更简单，就像在钟形曲线的例子中一样。