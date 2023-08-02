
--- pic\Green's theorem examples.pdf_01.png ---
1. Green's theorem examples
   格林定理示例

2. Green's theorem is beautiful and all, but here you can learn about how it is actually used.
   格林定理很美，但在这里你可以学习它实际上如何被使用。

3. Background - Green's theorem
   背景 - 格林定理

4. Remembering the formula 
   记住公式

1. Green's theorem is most commonly presented like this:
   格林定理通常被这样展示：

$$
\oint_C P dx+Q dy=\iint_R\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d A
$$

1. This is also most similar to how practice problems and test questions tend to look.
   这也最接近练习题和测试题的常见形式。

2. But personally, I can never quite remember it just in this $P$ and $Q$ form.
   但是对我个人而言，我始终无法记住这种只有$P$和$Q$的形式。

3. "Was it $\frac{\partial Q}{\partial x}$ or $\frac{\partial Q}{\partial y} ?$
   “是$\frac{\partial Q}{\partial x}$还是$\frac{\partial Q}{\partial y} ?$

4. "Which term is subtracted again?"
   “再次减去的是哪一项？”

5. I always start by thinking about this form:
   我总是首先考虑这种形式：

$$
\oint_C \mathbf{F} \cdot d \mathbf{r}=\iint_R 2 \mathrm{~d}-\operatorname{curl} \mathbf{F} d A
$$

10. I find this easier to remember because it actually has a physical meaning (see the last article for more details):
    我觉得这更容易记住，因为它实际上具有物理含义（详见上一篇文章）：

11. The line integral of a vector field $\mathbf{F}(x, y)$ around a closed curve $C$ measures the fluid rotation around that boundary $C$.
    向量场$\mathbf{F}(x, y)$在闭曲线$C$周围的线积分测量了该边界$C$周围的流体旋转。

12. The double integral of the curl of $\mathbf{F}$ adds up all the tiny little bits of fluid rotation within the region $R$ enclosed by $C$.
    $\mathbf{F}$的旋度的双重积分累加了由$C$围住的区域$R$内所有微小的流体旋转。

13. Intuitively, it makes sense that these should be related. And in fact, they are equal.
    直观地说，这些应该是相关的是有意义的。实际上，他们是相等的。

14. To get to the $P Q$ version of the theorem, write the components of $\mathbf{F}$ as $P(x, y)$ and $Q(x, y)$:
    要得到定理的$PQ$版本，将$\mathbf{F}$的分量写为$P(x, y)$和$Q(x, y)$：


--- pic\Green's theorem examples.pdf_01.png ---

1. (To remember that $P$ is the $x$-component and $Q$ is the $y$-component, think about the fact that $P$ comes before $Q$ in the alphabet).
   $$
   \mathbf{F}(x, y)=\left[\begin{array}{l}
   P(x, y) \\
   Q(x, y)
   \end{array}\right]
   $$
   （为了记住$P$是$x$-分量，$Q$是$y$-分量，可以想到在字母表中$P$在$Q$前面）。

2. And from here, expand each bit of the line integral, curl, etc.
   从这里开始，展开线积分，旋度等的每一部分。

3. After doing this a couple times, it's natural enough to do in your head.
   做了几次之后，这就足够自然地在你的脑海中进行了。

4. 
   $$
   \begin{aligned}
   & \oint_C \mathbf{F} \cdot d \mathbf{r}=\iint_R 2 \mathrm{~d}-\operatorname{curl} \mathbf{F} d A \\
   & \oint_C\left[\begin{array}{l}
   P(x, y) \\
   Q(x, y)
   \end{array}\right] \cdot\left[\begin{array}{c}
   d x \\
   d y
   \end{array}\right]=\iint_R 2 \mathrm{~d}-\operatorname{curl}\left(\left[\begin{array}{c}
   P(x, y) \\
   Q(x, y)
   \end{array}\right]\right) d A \\
   & \oint_C P d x+Q d y=\iint_R\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d x d y \\
   &
   \end{aligned}
   $$
   $\Downarrow$

5. Of course, this requires remembering how to compute two-dimensional curl, but this is something which ought to be remembered outside the context of Green's theorem anyway.
   当然，这需要记住如何计算二维旋度，但这是在格林定理之外应该被记住的东西。

6. Warning: Green's theorem only applies to curves that are oriented counterclockwise.
   警告：格林定理只适用于逆时针方向的曲线。

7. If you are integrating clockwise around a curve and wish to apply Green's theorem, you must flip the sign of your result at some point.
   如果你在一条曲线周围顺时针积分，并希望应用格林定理，那么你必须在某一点反转你的结果符号。

8. How do you know when to use Green's theorem?
   你怎么知道何时使用格林定理？

9. "Mathematics is not a spectator sport" - George Polya
   "数学不是观赏运动" - 乔治·波利亚

10. The best way to get a feel for its usefulness is to simply jump into some examples to get a feel for it.
    了解它的用处最好的方式就是简单地通过一些例子来感受它。

11. I'll debrief after each example to help extract the intuition for each one.
    我会在每个例子后进行简要说明，以帮助提取出每一个例子的直觉。


--- pic\Green's theorem examples.pdf_02.png ---

1. Example 1: Line integral $\rightarrow$ Area
   示例1：线积分 $\rightarrow$ 面积

2. Problem: Let $C$ represent a circle with radius 2 centered at $(3,-2)$ :
   问题：设$C$代表一个以$(3,-2)$为中心、半径为2的圆：

3. If you orient $C$ counterclockwise, compute the following line integral:
   如果你逆时针定向$C$，计算下列线积分：

$$
\oint_C 3 y d x+4 x d y
$$

4. Solution
   解答

5. Step 1: Is the curve in question oriented clockwise or counterclockwise?
   第1步：问题中的曲线是顺时针还是逆时针定向的？

6. Choose 1 answer:
   选择一个答案：

7. (B) Counterclockwise
   (B) 逆时针

8.  I know that might feel silly to ask, given that it was just stated explicitly in the problem.
    我知道，这个问题可能看起来很傻，因为它在问题中已经明确给出。

9.  But it's important to remember that you must always ask this when using Green's theorem.
    但是，要记住，当使用格林定理时，你必须总是问这个问题。

--- pic\Green's theorem examples.pdf_03.png ---
1. Step 2: As we apply Green's theorem to this integral $\oint_C 3 y dx+4 x dy$, what should we substitute for $P(x, y)$ and $Q(x, y)$?
   第2步：当我们将格林定理应用到这个积分$\oint_C 3 y dx+4 x dy$时，我们应该用什么来替代$P(x, y)$和$Q(x, y)$？


2. The line integral in Green's theorem looks like this: 
   格林定理中的线积分看起来像这样：

$$
\oint_C P dx+Q dy
$$

6. And here's the integral we need to compute:
   这是我们需要计算的积分：

$$
\oint_C 3 y dx+4 x dy
$$

7. Just matching terms, we should apply
   只需匹配项，我们应该应用

$$
P(x, y)=3 y
$$
   
8. and
   和

$$
Q(x, y)=4 x
$$

9. Step 3: Now compute the appropriate partial derivatives of $P(x, y)$ and $Q(x, y)$.
   第3步：现在计算$P(x, y)$和$Q(x, y)$的适当偏导数。


1. --- pic\Green's theorem examples.pdf_04.png ---

$$
\begin{aligned}
& \frac{\partial Q}{\partial x}=\frac{\partial}{\partial x}(4 x)=4 \\
& \frac{\partial P}{\partial y}=\frac{\partial}{\partial y}(3 y)=3
\end{aligned}
$$

2. Step 4: Finally, compute the double integral from Green's theorem. In this case, $R$ represents the region enclosed by the circle with radius 2 centered at $(3,-2)$. (Hint, don't work too hard on this one).
   步骤4：最后，根据格林定理计算双重积分。在这个例子中，$R$表示以$(3,-2)$为中心，半径为2的圆所围成的区域。（提示，这个不需要做得太复杂）。


3. Start by plugging in the expressions for $\frac{\partial Q}{\partial x}$ and $\frac{\partial P}{\partial y}$ that you found in the previous problem.
   从前面问题中找到的$\frac{\partial Q}{\partial x}$和$\frac{\partial P}{\partial y}$的表达式开始插入。

$$
\begin{aligned}
\iint_R\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d A & =\iint_R(4-3) d A \\
& =\iint_R d A
\end{aligned}
$$

6. Now before you go crazy describing the region $R$ with the appropriate bounds for $x$ and $y$, notice what this integral represents.
   在你为$x$和$y$确定合适的界限来描述区域$R$之前，注意一下这个积分代表的是什么。

7. Since there is no function inside it is just adding up tiny bits of area of $R$, so it will equal the area of $R$ itself!
   由于内部没有函数，它只是将$R$的微小面积相加，所以它等于$R$自身的面积！

8. Since $R$ is a circle with radius 2 , that area is $\pi r^2=\pi(2)^2=4 \pi$.
   由于$R$是一个半径为2的圆，那么面积是$\pi r^2=\pi(2)^2=4 \pi$。

9. Therefore our line integral evaluates to $4 \pi$.
   因此，我们的线积分的结果是$4 \pi$。

10. Example 1 debrief
    示例1解答

11. Why did the line integral in the last example become simpler as a double integral when we applied Green's theorem? 
    为什么在我们应用格林定理时，最后一个例子中的线积分变得简单了？

12. It's because the curl of the relevant function was a constant:
    这是因为相关函数的旋度是一个常数：

$$
2 \mathrm{~d}-\operatorname{curl}\left(\left[\begin{array}{c}
P(x, y) \\
Q(x, y)
\end{array}\right]\right)=2 \mathrm{~d}-\operatorname{curl}\left(\left[\begin{array}{c}
3 y \\
4 x
\end{array}\right]\right)
$$

--- pic\Green's theorem examples.pdf_05.png ---

1. More generally, if it looks like the partial derivative of $Q$ with respect to $x$ is simple, and/or that the partial derivative of $P$ with respect to $y$ is simple, think Green's theorem.
   更一般地，如果看起来$Q$关于$x$的偏导数很简单，和/或者$P$关于$y$的偏导数很简单，那么就考虑格林定理。

$$
\oint_C \overbrace{P(x, y)}^{\text {Is } \frac{\partial}{\partial y} \text { simple? }} d x+\overbrace{Q(x, y)}^{\text {Is }} d y
$$

2. It was also important that we could easily compute the area of the region in question. If that were not true, the double integral might not have been simpler at all.
   我们能够容易计算出问题区域的面积也很重要。如果不能做到这一点，双重积分可能根本就没有简化。

3. Example 2: Two function graphs
   示例2：两个函数图

4. Problem
   问题

5. Consider the following two functions:
   考虑以下两个函数：

$$
\begin{aligned}
& f(x)=\left(x^2-4\right)\left(x^2-1\right) \\
& g(x)=4-x^2
\end{aligned}
$$

6. Now consider the region between the graphs of these functions.
   现在考虑这些函数图之间的区域。

--- pic\Green's theorem examples.pdf_06.png ---

1. Let $D$ be the clockwise-oriented boundary of this region ( $D$ for droopy).
   让$D$表示这个区域的顺时针方向的边界（$D$表示下垂）。

2. Compute the following line integral:
   计算以下的线积分：

$$
\oint_D x^2 y d x-y^2 d y
$$

3. Solution
   解答

4. Step 1: Is the curve in question oriented clockwise or counterclockwise?
   步骤1：所讨论的曲线是顺时针方向还是逆时针方向？

5. Choose 1 answer:
   选择一个答案：

6. (A) Clockwise
   (A) 顺时针方向

7. Since Green's theorem applies to counterclockwise curves, this means we will need to take the negative of our final answer.
   由于格林定理适用于逆时针的曲线，这意味着我们需要对最终的答案取负值。

8.  Step 2: What should we substitute for $P(x, y)$ and $Q(x, y)$ in the integral $\oint_D x^2 y d x-y^2 d y$ ?
    步骤2：在积分 $\oint_D x^2 y d x-y^2 d y$ 中，我们应该用什么来替代 $P(x, y)$ 和 $Q(x, y)$？

$$
P(x, y)=
$$

$$
Q(x, y)=
$$

--- pic\Green's theorem examples.pdf_07.png ---


1. The line integral in Green's theorem looks like this:
   格林定理中的线积分如下：

$$
\oint_D P dx+Q dy
$$

3. And here's the integral we need to compute:
   这是我们需要计算的积分：

$$
\oint_D x^2 y dx-y^2 dy
$$

4. Just matching terms, we should apply
   只需匹配项，我们应该应用

$$
P(x, y)=x^2 y
$$
   
1. and 
   和
$$
Q(x, y)=-y^2
$$

1. Step 3: Now compute the appropriate partial derivatives of $P(x, y)$ and $Q(x, y)$.
   步骤3：现在计算$P(x, y)$和$Q(x, y)$的适当偏导数。

$$
\begin{aligned}
& \frac{\partial Q}{\partial x}= \\
& \frac{\partial P}{\partial y}=
\end{aligned}
$$

1. 
$$
\begin{aligned}
& \frac{\partial Q}{\partial x}=\frac{\partial}{\partial x}\left(-y^2\right)=0 \\
& \frac{\partial P}{\partial y}=\frac{\partial}{\partial y}\left(x^2 y\right)=x^2
\end{aligned}
$$


--- pic\Green's theorem examples.pdf_08.png ---
1. Step 4: To apply Green's theorem, we will perform a double integral over the droopy region $D$, which was defined as the region above the graph $y=\left(x^2-4\right)\left(x^2-1\right)$ and below the graph $y=4-x^2$.
   第四步：要应用格林定理，我们将对下垂区域$D$进行双重积分，该区域被定义为位于图形$y=\left(x^2-4\right)\left(x^2-1\right)$之上和图形$y=4-x^2$之下的区域。

2. This double integral will be something of the following form:
   这个双重积分将是以下形式的一些内容：

$$
\int_{x_1}^{x_2} \int_{y_1(x)}^{y_2(x)} \ldots d y d x
$$

3. Fill in all of those bounds:
   填写所有的这些边界：

$$
x_1=
$$
$$
x_2=
$$
$$
y_1(x)=
$$
$$
y_2(x)=
$$


1. Let's start with the easier ones. The bounds for $y$ are explicitly given in the problem: The region is defined to be above the graph $y=\left(x^2-4\right)\left(x^2-1\right)$ and below the graph $y=4-x^2$.
   让我们从较容易的开始。$y$的边界在问题中已经明确给出：该区域被定义为位于图形$y=\left(x^2-4\right)\left(x^2-1\right)$之上和图形$y=4-x^2$之下的区域。

2. This means the inner integral will look like this:
   这意味着内部积分将如下所示：

$$
\int_{\left(x^2-4\right)\left(x^2-1\right)}^{4-x^2}<\text { yadda yadda yadda }>d y
$$

7. The trickier part is knowing the bounds of $x$. The definition of our region doesn't even mention $x$. Let's take a look at the graphs of the $y$ bounds:
   更棘手的部分是知道$x$的边界。我们区域的定义甚至没有提到$x$。让我们看一下$y$边界的图形：




--- pic\Green's theorem examples.pdf_09.png ---
1. The bounds on the $x$-values are determined by where these two graphs intersect on the left and right.
   $x$值的界限是由这两个图在左右两侧交叉的位置决定的。

2. Just looking at the graph, you can probably guess that they intersect at $x=-2$ and $x=2$.
   只要看图，你可能会猜测他们在$x=-2$和$x=2$处相交。

3. You can also check this more precisely by plugging in 2 and -2 to each equation.
   你也可以通过将2和-2插入每个方程来更精确地检查这一点。

4. If you did not have the graph to look at to guess-and-check, you would solve the equation $\left(x^2-4\right)\left(x^2-1\right)=4-x^2$.
   如果你没有图表可以看来进行猜测和检查，你会解方程$\left(x^2-4\right)\left(x^2-1\right)=4-x^2$。

5. This means the double integral as a whole will have the following setup:
   这意味着整个双重积分将有以下设置：

1. $$\int_{-2}^2 \int_{\left(x^2-4\right)\left(x^2-1\right)}^{4-x^2} \overbrace{<\text { yadda yadda yadda }>}^{\text {We'll put something here in just a sec }} d y d x
$$
$$
\int_{-2}^2 \int_{\left(x^2-4\right)\left(x^2-1\right)}^{4-x^2} \overbrace{<\text { yadda yadda yadda }>}^{\text {我们马上会在这里放点东西 }} d y d x
$$

6. Step 5: Finally, to apply Green's theorem, we plug in the appropriate value to this integral.
   步骤5：最后，为了应用格林定理，我们将适当的值插入这个积分。

7. If our original line integral was oriented counterclockwise, we would plug in
   如果我们的原始线积分是逆时针方向，我们会插入

$$
\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}
$$

8. However, since the curve is oriented clockwise, we make this negative:
   但是，由于曲线是顺时针方向的，我们将其取负：

$$
-\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)=\frac{\partial P}{\partial y}-\frac{\partial Q}{\partial x}
$$




--- pic\Green's theorem examples.pdf_10.png ---

1. Using the answers to the previous two questions, plugging in this value to the double integral you set up, find the answer to the original line integral problem:
   利用前两个问题的答案，将这个值代入你设立的双重积分中，找出原始线积分问题的答案：

$$
\oint_D x^2 y d x-y^2 d y=
$$

2. Check [Hide explanation].
   检查 [隐藏解释]。

3. Then the integral is computed as follows:

1. 
$$
\begin{aligned}
& \int_{-2}^2(\int_{\left(x^2-4\right)\left(x^2-1\right)}^{4-x^2} \underbrace{\left(\frac{\partial P}{\partial y}-\frac{\partial Q}{\partial x}\right)}_{\text {Replace with values from step } 3} d y) d x \\
& \int_{-2}^2(\int_{\left(x^2-4\right)\left(x^2-1\right)}^{4-x^2} \underbrace{\left(x^2-0\right)}_{\text {Factor out from } y \text { integral }} d y) d x \\
& \int_{-2}^2(x^2 \underbrace{\int_{\left(x^2-4\right)\left(x^2-1\right)}^{4-x^2} d y}_{\text {Simply the difference of bounds }}) d x \\
& \int_{-2}^2 x^2(\underbrace{\left(4-x^2\right)-\left(x^2-4\right)\left(x^2-1\right)}_{\text {Factor out } x^2-4}) d x \\
& \int_{-2}^2 x^2\left(x^2-4\right) \underbrace{\left(-1-\left(x^2-1\right)\right)}_{-x^2} d x \\
& \int_{-2}^2-x^4\left(x^2-4\right) d x \\
& \int_{-2}^2-\left(x^6-4 x^4\right) d x \\
& \int_{-2}^2 4 x^4-x^6 d x \\
& {\left[4 \frac{x^5}{5}-\frac{x^7}{7}\right]_{x=-2}^{x=2}} \\
& \left(4 \frac{2^5}{5}-\frac{2^7}{7}\right)-\left(4 \frac{(-2)^5}{5}-\frac{(-2)^7}{7}\right) \\
\end{aligned}
$$
1. 
$$
\begin{aligned}
& \int_{-2}^2(\int_{\left(x^2-4\right)\left(x^2-1\right)}^{4-x^2} \underbrace{\left(\frac{\partial P}{\partial y}-\frac{\partial Q}{\partial x}\right)}_{\text {用步骤3的值替换}} d y) d x \\
& \int_{-2}^2(\int_{\left(x^2-4\right)\left(x^2-1\right)}^{4-x^2} \underbrace{\left(x^2-0\right)}_{\text {从 } y \text { 积分中提取出来}} d y) d x \\
& \int_{-2}^2(x^2 \underbrace{\int_{\left(x^2-4\right)\left(x^2-1\right)}^{4-x^2} d y}_{\text {只是边界的差值 }}) d x \\
& \int_{-2}^2 x^2(\underbrace{\left(4-x^2\right)-\left(x^2-4\right)\left(x^2-1\right)}_{\text {提取出 } x^2-4}) d x \\
& \int_{-2}^2 x^2\left(x^2-4\right) \underbrace{\left(-1-\left(x^2-1\right)\right)}_{-x^2} d x \\
& \int_{-2}^2-x^4\left(x^2-4\right) d x \\
& \int_{-2}^2-\left(x^6-4 x^4\right) d x \\
& \int_{-2}^2 4 x^4-x^6 d x \\
& {\left[4 \frac{x^5}{5}-\frac{x^7}{7}\right]_{x=-2}^{x=2}} \\
& \left(4 \frac{2^5}{5}-\frac{2^7}{7}\right)-\left(4 \frac{(-2)^5}{5}-\frac{(-2)^7}{7}\right) \\
\end{aligned}
$$




--- pic\Green's theorem examples.pdf_11.png ---

1.
$$
\left(4 \frac{32}{5}-\frac{128}{7}\right) \underbrace{-\left(4 \frac{-32}{5}-\frac{-128}{7}\right)}_{\text {This is just adding the same amount again }}
$$
$$
\left(4 \frac{32}{5}-\frac{128}{7}\right) \underbrace{-\left(4 \frac{-32}{5}-\frac{-128}{7}\right)}_{\text {这只是再次添加相同的数量}}
$$

1. Example 2 debrief
   示例2详解

1. As in Example 1, part of the reason this line integral became simpler is that the terms simplified once we looked at the appropriate partial derivatives.
   就像在示例1中，这个线积分变得更简单的部分原因是，一旦我们查看了适当的偏导数，这些项就简化了。

3. 
$$
\oint_C \overbrace{x^2 y}^{\begin{array}{c}
\text { Is } \frac{\partial}{\partial y} \text { simple? } \\
\text { A little bit, yes. }
\end{array}} d x+\overbrace{\left(-y^2\right)}^{\begin{array}{c}
\text { Is } \\
\text { Very } \frac{\partial}{\partial x} \text { simple } ?
\end{array}} d y
$$
$$\oint_C \overbrace{x^2 y}^{\begin{array}{c}
\text { 对于 } \frac{\partial}{\partial y} \text { 来说简单吗？ } \\
\text { 有点，是的。 }
\end{array}} d x+\overbrace{\left(-y^2\right)}^{\begin{array}{c}
\text { 对于 } \\
\text { 非常 } \frac{\partial}{\partial x} \text { 简单的 } ?
\end{array}} d y
$$


1. Also, the region in question was defined by two separate curves.
   另外，所讨论的区域由两个独立的曲线定义。

2. Computing the line integral directly requires setting up two separate line integrals for each curve.
   直接计算线积分需要为每个曲线设置两个独立的线积分。

3. But the double integral very naturally went over the full region in one fell swoop.
   但是，双重积分在一次过程中很自然地覆盖了整个区域。

4. Another thing to note is that the ultimate double integral wasn't exactly simple.
   另一点需要注意的是，最终的双重积分并不完全简单。

1. You still had to mark up a lot of paper during the computation.
   在计算过程中，你仍然需要标记很多纸张。


6. But this is okay. We can still feel confident that Green's theorem simplified things, since each individual term became simpler, since we avoided needing to parameterize our curves, and since what would have been two separate line integrals was just one double integral.
   但这没关系。我们仍然可以确信，格林定理简化了事情，因为每个单独的项都变得更简单，因为我们避免了需要参数化我们的曲线，而且原本需要进行的两个单独的线积分只是一个双重积分。





--- pic\Green's theorem examples.pdf_12.png ---

1. Sneaky area calculations.
   狡猾的面积计算。

2. In the previous two examples, we used Green's theorem to turn a line integral into a double integral.
   在前两个例子中，我们使用格林定理将线积分转化为双重积分。

3. Here, let's do things the other way around.
   这里，我们换一种方式来做。

4. Take a look at the double integral from Green's theorem:
   看看格林定理中的双重积分：

$$
\iint_R\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d A
$$

6. Remember how in Example 1, we were lucky enough to have the following property:
   还记得在第一个例子中，我们很幸运地具有以下属性：

$$
\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)=1
$$

7. This means our integral was just computing the area of $R$ :
   这意味着我们的积分只是在计算$R$的面积：

$$
\iint_R\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d A \rightarrow \iint_R d A=\text { Area of } R
$$

8. Now imagine that we didn't already know the area of $R$, but we wished to compute it.
   现在想象一下，我们还不知道$R$的面积，但我们希望计算它。

9. One thing you could do is find some pair of functions $P(x, y)$ and $Q(x, y)$ satisfying this curl-equals-one property:
   你可以做的一件事是找到一对满足旋度等于一的性质的函数$P(x, y)$和$Q(x, y)$：

$$
\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=1
$$

10. According to Green's theorem, any pair of functions like this let's you compute the area of a region using a line integral:
    根据格林定理，任何像这样的函数对都可以让你使用线积分来计算一个区域的面积：

$$
\begin{aligned}
\oint_C P d x+Q d y & =\iint_R\left(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right) d A \\
& =\iint_R(1) d A \\
& =\text { Area of } R
\end{aligned}
$$

11. Doesn't that feel strange, computing the area of a region using a line integral around its boundary?
    使用围绕其边界的线积分计算区域的面积，感觉不觉得很奇怪吗？

12. Let' see what it looks like in action.
    让我们看看在实际中是什么样子。




--- pic\Green's theorem examples.pdf_13.png ---
1. Example 3: Area of a seashell
   示例3：海贝的面积

2. Problem
   问题

3. Consider the spiral defined by the following parametric equations in the range $0 \leq t \leq 2 \pi$.
   考虑在范围$0 \leq t \leq 2 \pi$内由以下参数方程定义的螺旋线。

$$
\begin{aligned}
& x(t)=t \cos (t) \\
& y(t)=t \sin (t)
\end{aligned}
$$

4. Now add the line from $(0,0)$ to $(2 \pi, 0)$ to this spiral, and consider the seashellshaped region it encloses.
   现在，把从$(0,0)$到$(2 \pi, 0)$的线段加到这个螺旋线上，考虑它所包围的形如海贝的区域。



--- pic\Green's theorem examples.pdf_14.png ---
1. What is the area of that region?
   那个区域的面积是多少？

2. Solution
   解答

3. Step 1: How is the boundary of this seashell oriented?
   第一步：这个贝壳的边界是如何定向的？

4. Choose 1 answer: (B) Counterclockwise
   选择一个答案：（B）逆时针

5. Step 2: Choose the appropriate $P(x, y)$ and $Q(x, y)$.
   第二步：选择适当的 $P(x, y)$ 和 $Q(x, y)$。

6. To apply the Green's theorem trick, we first need to find a pair of functions $P(x, y)$ and $Q(x, y)$ which satisfy the following property:
   要应用格林定理的技巧，我们首先需要找到一对函数 $P(x, y)$ 和 $Q(x, y)$，它们满足以下性质：

$$
\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=1
$$

8. Actually, quite a few pairs of functions satisfy this.
   实际上，有相当多的函数对满足这一条件。

9. Concept check: Which of the following function pairs satisfies this property?
   概念检查：以下哪对函数满足这个性质？

10. Choose all answers that apply:
    选择所有适用的答案：




--- pic\Green's theorem examples.pdf_15.png ---


1. B
$$
\begin{aligned}
& P(x, y)=-y \\
& Q(x, y)=0
\end{aligned}
$$

1. C
$$
\begin{aligned}
& P(x, y)=0 \\
& Q(x, y)=x
\end{aligned}
$$

1. D
$$
\begin{aligned}
& P(x, y)=-\frac{y}{2} \\
& Q(x, y)=\frac{x}{2}
\end{aligned}
$$


1. All but the first choice are correct.
   除了第一项选择以外，所有的选择都是正确的。

2. When you take the definitions of $P$ and $Q$ in the first choice, both partial derivatives are 0.
   当你采用第一项选择中$P$和$Q$的定义时，两个偏导数都为0。

3. You might think the second or third choices above make things simplest.
   你可能会认为上面的第二或第三个选择使事情变得最简单。

4. Interestingly, though, it's often the last choice that makes the line integral computation work out best.
   然而，有趣的是，最后一个选择通常使线积分计算得到最好的结果。

5. This means solving the following integral:
   这意味着解决以下积分：

$$
\oint_C \underbrace{-\frac{1}{2} y dx}_{P dx}+\underbrace{\frac{1}{2} x dy}_{Q dy}
$$

10. Or, written more cleanly,
    或者，更干净地写出来，

$$
\oint_C \frac{1}{2}(x dy-y dx)
$$

11. Why is this simpler? You will see in just a moment how things nicely cancel out, and it has to do with symmetrically including both $x$ and $y$ into the expression.
    为什么这更简单？你会立刻看到事情如何很好地抵消，并且它与将$x$和$y$对称地包含在表达式中有关。

12. Honestly, I'm not sure how you could have seen this ahead of time; it's just really clever.
    说实话，我不确定你怎么可能提前看到这一点；这真的很聪明。

13. Step 3: Compute the line integral.
    步骤3：计算线积分。


--- pic\Green's theorem examples.pdf_16.png ---
1. The boundary of our region is defined with two curves.
   我们的区域边界由两条曲线定义。

2. One is the spiral, defined by these two equations in the range $0 \leq t \leq 2 \pi$ :
   其中一条是螺旋线，在范围$0 \leq t \leq 2 \pi$内由这两个方程定义：

$$
\begin{aligned}
& x(t)=t \cos (t) \\
& y(t)=t \sin (t)
\end{aligned}
$$

3. The other is the line between $(0,0)$ and $(2 \pi, 0)$.
   另一条是从$(0,0)$到$(2 \pi, 0)$的线。

4. Notice, this line is purely on the $x$-axis.
   请注意，这条线完全在$x$轴上。

5. Therefore $y$ is always 0 , and $d y$ is also 0 , since there's no change in $y$.
   因此，$y$始终为0，由于$y$没有变化，所以$dy$也为0。

6. So consider the value of the line integral on this segment:
   所以，我们考虑一下这一段线积分的值：

$$
\int \frac{1}{2}(x \underbrace{d y}_0-\underbrace{y}_0 d x)
$$

7. Each part of the integrant is 0 , so we can ignore it!
   积分中的每一部分都是0，所以我们可以忽略它！

8. Therefore, we can just take this line integral over our spiral and get the answer.
   因此，我们只需对螺旋线进行这个线积分就可以得到答案。

9. Concept check: Given that $x(t)=t \cos (t)$ and $y(t)=t \sin (t)$, what should we plug in for $x d y-y d x$ in the line integral?
   概念检查：已知$x(t)=t \cos (t)$和$y(t)=t \sin (t)$，我们应该在线积分中代入什么作为$x dy - y dx$？

10. Try to work it out on paper and simplify.
    尝试在纸上计算并简化。


1. 
$$
\begin{aligned}
&\underbrace{x \, dy-y \, dx}_{\text{in functions } x(t), y(t)}\\
&\underbrace{x(t)\left(\frac{dy}{dt} \, dt\right)-y(t)\left(\frac{dx}{dt} \, dt\right)}_{\text{Factor out } dt}\\
&\underbrace{\left(x(t) \frac{dy}{dt}-y(t) \frac{dx}{dt}\right)}_{\text{Plug in definitions of } x(t) \text{ and } y(t)} dt\\
&(t \cos (t) \underbrace{\frac{d}{dt}(t \sin (t))}_{\text{Product rule }}-t \sin (t) \underbrace{\frac{d}{dt}(t \cos (t))}_{\text{Product rule }}) dt
\end{aligned}
$$

$$
\begin{aligned}
&\underbrace{x d y-y d x}_{\text {在函数 } x(t), y(t) \text { 中}}\\
&\underbrace{x(t)\left(\frac{d y}{d t} d t\right)-y(t)\left(\frac{d x}{d t} d t\right)}_{\text {提取出 } d t}\\
&\underbrace{\left(x(t) \frac{d y}{d t}-y(t) \frac{d x}{d t}\right)}_{\text {代入 } x(t) \text { 和 } y(t) \text { 的定义}} d t\\
&(t \cos (t) \underbrace{\frac{d}{d t}(t \sin (t))}_{\text {乘积法则 }}-t \sin (t) \underbrace{\frac{d}{d t}(t \cos (t))}_{\text {乘积法则 }}) d t
\end{aligned}
$$



--- pic\Green's theorem examples.pdf_17.png ---
1. 


2. Bring it on home: Use the last answer to compute the following line integral on the spiral, which will give the area of the seashell region as desired:
   将其带回家：使用最后的答案计算螺旋上的以下线积分，这将给出所需的贝壳区域的面积：

$$
\int_{\text {Spiral }} \frac{1}{2}(x d y-y d x)=
$$

3. Start by plugging in the value for $x d y-y d x$ that you found in the last problem, and put in the bounds $t=0$ and $t=2 \pi$ :
   首先，插入你在最后一个问题中找到的$x d y-y d x$的值，并设置边界$t=0$ 和 $t=2 \pi$：

$$
\begin{aligned}
\int_{\text {Spiral }} \frac{1}{2} \underbrace{(x d y-y d x)}_{t^2 d t} & =\int_0^{2 \pi} \frac{1}{2} t^2 d t \\
& =\left[\frac{1}{6} t^3\right]_{t=0}^{t=2 \pi} \\
& =\frac{(2 \pi)^3}{6}-\frac{0^3}{6} \\
& =\frac{8 \pi^3}{6}
\end{aligned}
$$

1. Summary
   总结

2. Green's theorem can turn tricky line integrals into more straight-forward double integrals.
   格林定理可以将复杂的线积分转化为更直接的双重积分。

3. To know if Green's theorem will actually make a line integral simpler, ask the following two questions:
   要知道格林定理是否真的会简化线积分，可以提出以下两个问题：



--- pic\Green's theorem examples.pdf_18.png ---

1. Also, consider if the region encompassed by the curve $C$ will be easy to describe with a double integral, or if it has a known area.
   此外，还要考虑由曲线$C$包围的区域是否易于用双重积分来描述，或者它是否有已知的面积。

2. You can compute the area of a region with the following line integral around its counterclockwise-oriented boundary:
   你可以使用以下围绕其逆时针方向边界的线积分来计算一个区域的面积：

$$
\oint_C \frac{1}{2}(x d y-y d x)
$$



