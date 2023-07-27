
--- pic\Double integrals.pdf_00.png ---

1. Double integrals.
   双重积分。

1. Double integrals are a way to integrate over a two-dimensional area.
   双重积分是一种在二维区域上进行积分的方法。

2. Among other things, they let us compute the volume under a surface.
   除其他外，它们让我们能够计算出表面下的体积。

1. Background.
   背景。

2. Ordinary integrals.
   常规积分。

3. Graphs of multivariable functions.
   多变量函数的图。

4. What we're building to
   我们的目标

1. Given a two-variable function $f ( x , y )$, you can find the volume between this graph and a rectangular region of the $xy$-plane by taking an integral of an integral.
给定一个两变量函数 $f ( x , y )$，你可以通过计算一个积分的积分来找到这个图形和 $xy$ 平面的矩形区域之间的体积。


6. This is a function of $y$:
   这是一个关于 $y$ 的函数：

7. This is called a double integral.
   这被称为双重积分。

2. You can compute this same volume by changing the order of integration.
你可以通过改变积分的顺序来计算这相同的体积。

3. This is a function of $x$.
这是一个关于 $x$ 的函数。

--- pic\Double integrals.pdf_01.png ---

1. The computation will look and feel very different, but it still gives the same result.
   计算的过程可能会看起来和感觉起来非常不同，但它仍然会得到相同的结果。

2. Volume under a surface
   表面下的体积

3. Consider the function $f(x,y) = x + \sin(y) + 1$
   考虑函数 $f(x,y) = x + \sin(y) + 1$

4. Its graph looks like this:
   它的图像看起来像这样：

5. Graph of $f(x, y) = x + \sin(y) + 1$
   函数 $f(x, y) = x + \sin(y) + 1$ 的图像

6. Now consider the rectangle on the $xy$-plane defined by $0 < x < 2$ and $-π < y <= π$.
   现在考虑在$xy$平面上由 $0 < x < 2$ 和 $-π < y < π$ 定义的矩形。

7. What is the volume above this rectangle, and under the graph of $f(x, y)$?
   这个矩形上方和 $f(x, y)$ 图形下方的体积是多少？

--- pic\Double integrals.pdf_02.png ---

1. Quick refresh of area under curve
   快速刷新曲线下的区域

2. From single variable calculus, we know that integrals let us compute the area under a curve.
   从单变量微积分，我们知道积分让我们计算曲线下的面积。

3. For example, the area under the graph of $y = \frac{1}{4}x^2 + 1$ between the values $x = -3$ and $x = 3$ is
   例如，$y = \frac{1}{4}x^2 + 1$ 的图形在 $x = -3$ 和 $x = 3$ 之间的面积是


4. A nice way to think about this is to imagine adding the areas of infinitely many, infinitely thin rectangles which sweep under the curve in the specified region.
   想象一下这个的一个好方法是，想象添加无限多个、无限薄的矩形的面积，这些矩形在指定区域下的曲线下扫过。

1. You can think of the value of the function $g ( x ) = \frac{1}{4} x^2 + 1$ as being the height of each rectangle, $dx$ as being the infinitesimal width, and $\int$ as being a pumped-up summing machine that's able to handle the idea of infinitely many infinitely small things.
你可以将函数 $g ( x ) = \frac{1}{4} x^2 + 1$ 的值想象为每个矩形的高度，$dx$ 作为无穷小的宽度，而 $\int$ 则是一个强大的求和机器，能够处理无穷多的无穷小事物的概念。

理解了，按照您的需求，这是我拆分和翻译的结果：

--- pic\Double integrals.pdf_03.png ---

1. Written more abstractly, this looks like 
   更抽象地写，这看起来像 

2. Sweeping area under a volume
   扫过体积下的面积

3. For our volume problem, we can do something similar.
   对于我们的体积问题，我们可以做类似的事情。

4. Our strategy will be to subdivide the volume into slices with two-dimensional area.
   我们的策略将是将体积划分为具有二维面积的切片。

5. Compute the areas of these slices.
   计算这些切片的面积。

6. Combine them all together to get the volume as a whole.
   将它们全部结合起来得到整体的体积。

7. Think of two-dimensional slices of the volume under the graph of $f(x, y)$.
   考虑图形 $f(x, y)$ 下体积的二维切片。

1. Specifically, take all the slices representing a constant value of $y$:
具体来说，取所有代表 $y$ 常数值的切片：

1. Consider just one of those slices, such as the one representing $y = \frac{\pi}{2}$.
   考虑其中的一个切片，例如代表 $y = \frac{\pi}{2}$ 的那个。

2. The area of that slice is given by the integral:
   该切片的面积由积分给出：

3. Written more abstractly, for a given value of $y$, the area of that slice is:
更抽象地写，对于给定的 $y$ 值，该切片的面积是：

--- pic\Double integrals.pdf_04.png ---

1. Notice, this is an integral with respect to $x$, as indicated by the $dx$, so as far as the integral is concerned, the symbol "$y$" represents a constant.
   注意，这是一个关于 $x$ 的积分，如 $dx$ 所示，所以就积分而言，符号 "$y$" 表示一个常数。

2. When you perform this integral, it will be some expression of $y$.
   当你执行这个积分时，它将是 $y$ 的某个表达式。

3. Try it for yourself: Perform the integral to compute the area of these constant-$y$-value slices: 
   试试看：执行积分以计算这些恒定 $y$ 值切片的面积：

4. When you plug in some value of $y$ to this expression, such as $y = \frac{\pi}{2}$, you get the area of a slice of our volume representing that $y$-value.
   当你在这个表达式中代入 $y$ 的某个值，例如 $y = \frac{\pi}{2}$，你会得到表示那个 $y$ 值的我们体积的切片的面积。

5. Now If we multiply the area of each one of these slices by $dy$, a tiny change in the $y$-direction, we will get a tiny slice of volume.
   现在，如果我们将这些切片每一个的面积乘以 $dy$，$y$ 方向的微小变化，我们将得到一个微小的体积切片。

6. For example, $4 + 2 \sin(y)$ might represent the area of a slice, but $(4 + 2 \sin(y))dy$ represents the infinitesimal volume of that slice.
   例如，$4 + 2 \sin(y)$ 可能表示切片的面积，但是 $(4 + 2 \sin(y))dy$ 表示该切片的无穷小体积。

1. Using yet another integral, this time with respect to $y$, we can effectively sum up all those tiny volume slices to get the total volume under the surface:
通过再次使用积分，这次是关于 $y$ 的积分，我们可以有效地求和所有那些微小的体积切片，以得到表面下的总体积：

--- pic\Double integrals.pdf_05.png ---

1. Area of a slice.
   切片的面积。

2. Try it yourself! What do you get when you plug in the expression for $\int_{0}^{2} f(x, y) \, dx$ that you found above, and solve the second integral?
   自己试试看！当你将你之前找到的 $\int_{0}^{2} f(x, y) \, dx$ 表达式代入，并解决第二个积分，你会得到什么？

3. Start by plugging in the value for the inner integral that you found above
   首先，代入你之前找到的内部积分的值

4. Then compute the integral with respect to $y$:
   然后计算关于 $y$ 的积分：

5. So evidently the volume we were looking for is $8\pi$.
   所以显然我们要找的体积是 $8\pi$。

6. Two choices in direction.
   方向有两种选择。

7. You could also dissect the volume we are trying to find a different way.
   你也可以以不同的方式去解构我们试图寻找的体积。

8. Take slices which represent constant $x$ values, instead of constant $y$ values, and add up the volume slices.
   取代表常量 $x$ 值的切片，而不是常量 $y$ 值，并将体积切片加起来。

--- pic\Double integrals.pdf_06.png ---

1. Constant $x$ slices under graph $z = x+\sin(y)+1$.
   图形 $z = x+\sin(y)+1$ 下的常量 $x$ 切片。


2. Concept check: Which of the following integrals represents the area of a constant-$x$-value slice? 
   概念检查：下列哪个积分代表常数 $x$ 值切片的面积？

3. The second answer is correct: 
   第二个答案是正确的：

4. To get the area of a slice representing a constant $x$-value, you integrate with respect to $y$.
   为了得到代表常量 $x$ 值的切片的面积，你需要关于 $y$ 进行积分。

5. Some people call this "integrating the y-out", since you will be left with a function of $x$.
   有些人称之为"积分消去 $y$"，因为你最后将得到一个 $x$ 的函数。

1. Now imagine multiplying each of these areas by $dx$, a tiny step in the $x$-direction, which is perpendicular to the slice.
   现在想象每个面积都乘以 $dx$，这是 $x$ 方向上的一个微小步骤，它垂直于切片。

2. This will give some kind of infinitesimal volume.
   这将给出一种无穷小的体积。

6. By adding up all those infinitesimal volumes as $x$ ranges from 0 to 2, we will get the volume under the surface.
   通过将 $x$ 从 0 到 2 的范围内的所有这些无穷小体积加起来，我们将得到表面下的体积。

--- pic\Double integrals.pdf_07.png ---

1. Concept check: Which of the following double-integrals represents the volume under the graph of our function $f(x, y) = x + \sin(y) + 1$ in the region where $0 < x < 2$ and $-\pi \leq y \leq \pi$? Choose 1 answer:
   概念检查：以下哪个双重积分代表了我们的函数 $f(x, y) = x + \sin(y) + 1$ 在区域 $0 < x < 2$ 且 $-\pi \leq y \leq \pi$ 下的体积？

2. The second answer is correct:
   第二个答案是正确的：

1. It correctly matches the bounds of the inner $dy$ integral with the $y$-bounds of the region where we are integrating, and likewise it matches the bounds of the outer $dx$-integral with the $x$-bounds of our region.
   它正确地将内部 $dy$ 积分的界限与我们积分区域的 $y$-界限相匹配，同样，它将外部 $dx$ 积分的界限与我们区域的 $x$-界限相匹配。

2. Try it yourself! Perform the double integral to compute the volume under the surface.
   自己试试看！执行双重积分以计算表面下的体积。

3. Of course, you already found the volume in the previous section, but it is edifying to see how it can be computed a second way.
   当然，你在上一节已经找到了体积，但是看看它如何可以通过第二种方式计算是很有教育意义的。

--- pic\Double integrals.pdf_08.png ---

1. Integrate with respect to $y$ 
   对 $y$ 进行积分 

2. Consolidate terms.
   合并项。

1. Thankfully, this computation gives the same volume that we found in the previous section.
   幸运的是，这个计算得到的体积和我们在前一部分找到的体积是相同的。

2. Something would have to be wrong with our reasoning if it didn't.
   如果不是，我们的推理必定出了问题。

4. In short, the order of integration does not matter.
   简单来说，积分的顺序并不重要。

5. On the one hand, this might seem obvious, since either way you are computing the same volume.
   从一方面来说，这似乎很明显，因为无论如何你都是在计算同一体积。

6. However, these are two genuinely different computations, so the fact that they equal each other turns out to be a useful mathematical trick.
   然而，这两个计算确实是不同的，因此他们相等的事实被证明是一个有用的数学技巧。

7. For example, several proofs in probability theory involve showing that two quantities are equal by showing that both result from the same double integral, just computed in a different order.
   例如，在概率理论中有多个证明需要展示两个量是相等的，这是通过显示它们都来源于同一个双重积分来证明的，只是计算的顺序不同。

--- pic\Double integrals.pdf_09.png ---

1. Technically, I should mention that there exist some exotic double integrals where swapping the order of integration gives a different value.
   技术上讲，我应该提到存在一些特殊的双重积分，其中交换积分的顺序会得到不同的值。

2. The relevant piece of mathematics describing when you can and cannot swap integrals is "Fubini's Theorem".
   描述你何时可以和不能交换积分的相关数学是"富比尼定理"。

3. You may learn the full details of Fubini's Theorem in an analysis course, but as an introduction to double integrals, you really needn't worry about it.
   你可能会在分析课程中学习富比尼定理的全部细节，但作为双重积分的引入，你实际上不需要担心它。

4. For most, if not all, the function you deal with in practice, you can happily swap around the integrals to your heart's content!
   对于你在实践中处理的大多数，如果不是全部的函数，你可以愉快地随心所欲地交换积分！

5. Consider the function 
考虑函数 

1. What is the volume under the graph of this function in the region where $-1 \leq x \leq 1$ and $-\pi \leq y \leq \pi$?
在区域 $-1 \leq x \leq 1$ 和 $-\pi \leq y \leq \pi$ 下，这个函数图形下的体积是多少？

1. Here what this volume looks like:
这就是这个体积的样子：

--- pic\Double integrals.pdf_10.png ---

1. Concept check: Imagine cutting this volume under $f(x, y) = \cos(y)x + 1$ along the plane representing $y = 1$.
概念检查：想象一下，沿着表示 $y = 1$ 的平面切割在 $f(x, y) = \cos(y)x + 1$ 下的这个体积。

2. Which of the following integrals represents the area of that slice? Choose 1 answer:
   下列哪个积分代表了该切片的面积？选择1个答案:

2. Here is a picture of the slice in question (in red).
   这是被询问的切片的图片（红色部分）。

3. To find its area, you integrate from $-1$ to $1$ in the $x$-direction.
   要找到它的面积，你在 $x$ 方向上从 $-1$ 积分到 $1$。

4. Therefore, the first answer is correct.
   因此，第一个答案是正确的。

--- pic\Double integrals.pdf_11.png ---

1. Practice: What do you get when you compute this integral for a general value of $y$, not just $y = 1$? 
   练习：当你对一般的 $y$ 值计算这个积分时，你会得到什么，不仅仅是 $y = 1$？ 

1. More practice: The expression you just found represents the area of slices of our volume representing constant $y$-values.
   更多的练习：你刚刚找到的表达式代表了我们的体积中代表常数 $y$ 值的切片的面积。

2. Using this expression, set up an integral to find the volume under the surface, and solve the integral.
   使用这个表达式，建立一个积分来找出表面下的体积，并解出积分。

3. We just found that the area of a constant-$y$-value slice of our volume between the values $x = -1$ and $x = 1$ is 
   我们刚刚发现，我们的体积中，在 $x = -1$ 和 $x = 1$ 之间的一个常数 $y$ 值切片的面积是

4. You can imagine adding a tiny bit of depth to this area by multiplying It by $dy$, a tiny step in the $y$ direction.
   你可以想象通过将这个面积乘以 $dy$，在 $y$ 方向上的一个微小步骤，来给这个面积添加一点点深度。

5. You can think of this as an infinitesimal volume.
   你可以把这想象为一个无穷小的体积。

1. Since our volume is defined in the region where $- \pi \leq y \leq \pi$, we add up these infinitesimal volumes within that range:
由于我们的体积定义在区域 $- \pi \leq y \leq \pi$ 中，我们在该范围内累加这些无穷小的体积：

--- pic\Double integrals.pdf_12.png ---

1. Summary
   总结

2. Given a two-variable function $f(x, y)$, you can find the volume between its graph and a rectangular region of the $xy$-plane by taking an integral of an integral, this is called a double integral.
   给定一个二变量函数 $f(x, y)$，你可以通过取两次积分，找到它的图形和 $xy$ 平面的矩形区域之间的体积，这就叫做双重积分。

3. You can compute this same volume by changing the order of integration: 
   你可以通过改变积分的顺序计算同样的体积：

4. The computation will look and feel very different, but it still gives the same result.
   计算过程看起来和感觉起来会非常不同，但结果仍然是相同的。

