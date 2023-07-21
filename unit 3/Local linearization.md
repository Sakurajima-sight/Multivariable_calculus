
--- pic\Local linearization.pdf_00.png ---

1. Local linearization
     本地线性化
2. Learn how to generalize the idea of a tangent plane into a linear approximation of scalar-valued multivariable functions.
     学习如何将切平面的概念推广到标量值多变量函数的线性近似。
3. Background
     背景
1. The gradient
梯度
4. What we're building to
     我们正在建设的
5. Local linearization generalizes the idea of tangent planes to any multivariable function.
     本地线性化将切平面的概念推广到任何多变量函数。
6. Here, I will just talk about the case of scalar-valued multivariable functions.
     在这里，我只会谈论标量值多变量函数的情况。
7. The idea is to approximate a function near one of its inputs with a simpler function that has the same value at that input, as well as the same partial derivative values.
     这个思想是用一个更简单的函数近似函数在其一个输入值附近的值，该简单函数在该输入值处具有相同的值，以及相同的偏导数值。
8. Written with vectors, here's what the approximation function looks like:
     用向量表示，近似函数看起来像这样：
9. x is the variable
     x是变量
10. $L_f(x) = f(x_0) + \nabla f(x_0) (x - x_0)$
   $L_f(x) = f(x_0) + \nabla f(x_0) (x - x_0)$
11. This is called the local linearization of f near $x_0$.
    这被称为f在$x_0$附近的局部线性化。
12. Tangent planes as approximations
    切平面作为近似
13. In the previous article, | talked about finding the tangent plane to a two-variable function's graph.
    在上一篇文章中，我谈到了找到一个二变量函数图的切平面。
14. As always in multivariable calculus, it is healthy to contemplate a new concept without relying on graphical intuition. 
   在多元微积分中，不依赖图形直觉来思考新概念总是有益的。
15. That's not to say you should not try to think visually.
   这并不是说你不应该试图进行视觉思考。
16. Maybe instead think purely about the input space, or think relevant transformation rather than the graph.
   也许你应该纯粹地思考输入空间，或者思考相关的变换，而不是图形。



--- pic\Local linearization.pdf_01.png ---
1. The formula for the tangent plane ended up looking like this. 
切平面的公式最后呈现如下形式。

1. $T(x, y) = f(x_0, y_0) + f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0)$
$T(x, y) = f(x_0, y_0) + f_x(x_0, y_0)(x - x_0) + f_y(x_0, y_0)(y - y_0)$

1. This function $T(x, y)$ often goes by a different name: The "local linearization" of f at the point $(x_0, y_0)$. 
这个函数 $T(x, y)$ 通常有一个不同的名称：在点 $(x_0, y_0)$ 处 f 的"局部线性化"。

1. You can think about this as the simplest function satisfying two properties:
你可以将其视为满足以下两个性质的最简单的函数：

1. It has the same value of f at the point $(x_0, y_0)$. 
在点 $(x_0, y_0)$ 处，它的 f 值与原函数相同。

1. It has the same partial derivatives as f at the point $(x_0, y_0)$. 
在点 $(x_0, y_0)$ 处，它的偏导数与原函数相同。

--- pic\Local linearization.pdf_02.png ---

1. Fundamentally, a local linearization approximates one function near a point based on the information you can get from its derivative(s) at that point. 
从根本上说，局部线性化是在一个点附近对一个函数进行近似，这种近似基于你能在该点处得到的导数信息。

1. In the case of functions with a two-variable input and a scalar (i.e. non-vector) output, this can be visualized as a tangent plane.
在具有两个变量输入和标量（即非向量）输出的函数的情况下，这可以被视为一个切平面。

2. However, with higher dimensions we don't have this visual luxury, so we are left to think about it just as an approximation.
然而，对于更高维度，我们没有这种视觉的奢侈，所以我们只能把它当作一个近似值来思考。

1. In real-world applications of multivariable calculus, you almost never care about an actual plane in space. 
在多变量微积分的实际应用中，你几乎不关心空间中的实际平面。

1. Instead, you might have some complicated function, like, oh, I don't know, air resistance on a parachute as a function of speed and orientation.
相反，你可能有一些复杂的函数，比如，我不知道，降落伞的空气阻力作为速度和方向的函数。

1. Dealing with the actual function may be tricky or computationally expensive, so it's helpful to approximate it with something simpler, like a linear function.
处理实际的函数可能会很棘手或者计算成本高，所以用一些更简单的东西，比如线性函数来近似它是有帮助的。

1. What do I mean by "Linear function"?
我说的"线性函数"是什么意思？

1. Consider a function with a multidimensional input.
考虑一个具有多维输入的函数。

1. This function is called linear if in its definition, all the coordinates are just multiplied by constants, with nothing else happening to them.
如果在其定义中，所有的坐标只是被常数乘以，而没有其他的操作，那么这个函数就被称为线性的。

1. For example, it might look like this:
例如，它可能看起来像这样：

1. The full story of linearity goes deeper (hence the existence of the field "Linear algebra"), but for now, this conception will do.
线性的全貌更深入（因此存在"线性代数"这个领域），但现在，这个概念就够了。

1. Typically, instead of writing out all the variable like this, you would treat the input as a vector:
通常，你不会像这样写出所有的变量，而是将输入视为一个向量：

9. And you would define the function using a dot product:
并且你会使用点积来定义函数：

--- pic\Local linearization.pdf_03.png ---
1. For the purposes of this article, and more generally when you talk about local linearization, you are allowed to add in a constant to this expression:
对于这篇文章，更一般的说，当你谈论局部线性化时，你可以在这个表达式中加入一个常数：

1. $f(x) = c + v \cdot x$
$f(x) = c + v \cdot x$

1. If you wanted to be pedantic, this is no longer a linear function.
如果你想吹毛求疵，这已经不再是一个线性函数了。

2. It's what's called an "affine" function.
这被称为"仿射"函数。

3. But most people would say "whatever, it's basically linear".
但大多数人会说"无所谓，基本上是线性的"。

1. Now, suppose your function $f(x)$ does not have the luxury of being linear. 
现在，假设你的函数 $f(x)$ 没有线性的优点。

4. (The bolded "x" still represents a multidimensional vector).
（加粗的"x"仍然代表一个多维向量）。

5. It might be defined by some crazy expression way more wild than a dot product.
它可能由比点积更疯狂的表达式定义。

1. The idea of a local linearization is to approximate this function near some particular input value, $x_0$, with a function that Is linear. 
局部线性化的想法是用一个线性函数来近似这个函数在某个特定输入值 $x_0$ 附近的值。

6. Notice, by plugging in $x = x_0$, you can see that both functions $f$ and $L_f$ will have the same value at the input $x_0$.
注意，通过插入$x = x_0$，你可以看到函数$f$和$L_f$在输入$x_0$处都有相同的值。

7. The vector dotted against the variable $x$ is the gradient of $f$ at the specified input, $\nabla f(x_0)$.
与变量$x$点乘的向量是在指定输入处$f$的梯度，$\nabla f(x_0)$。

8. This ensures that both functions $f$ and $L_f$ will have the same gradient at the specified input.
这确保了函数$f$和$L_f$在指定输入处具有相同的梯度。

9. In other words, all their partial derivative information will be the same.
换句话说，他们所有的偏导数信息都是相同的。

10. I think the best way to understand this formula is to basically derive it for yourself in the context of a specific function.
我认为理解这个公式的最好方法基本上是在特定函数的上下文中自己推导出来。

11. Example 1: Finding a local linearization.
示例1：寻找局部线性化。

12. Problem: Have yourself a function:
问题：有一个函数：

--- pic\Local linearization.pdf_04.png ---
1. Find a linear function $L_f(x, y, z)$ such that the value of L and all its partial derivatives match those of f at the following point:
找一个线性函数 $L_f (x, y, z)$，使得 L 的值及其所有的偏导数与 f 在下面这个点的值及偏导数相匹配：

1. Step 1: Evaluate f at the chosen point
步骤1：在选定的点处评估函数f

1. Step 2: Use this to start writing your function. Which of the following functions will be guaranteed to equal f at the input $(x, y, z) = (8, 4,3)$? Choose 1 answer:
步骤2：用这个开始编写你的函数。下列哪个函数能保证在输入 $(x, y, z) = (8, 4,3)$ 时等于 f 呢？选择一个答案：

1. For both of these, a, b and c are all arbitrary constants.
对于这两个公式，a、b 和 c 都是任意常数。


--- pic\Local linearization.pdf_05.png ---
1. You might start writing the desired function $L_f$ like this:
   你可能会这样开始写下你想要的函数$L_f$：
   
   $L_f(x,y,z) = 3 + \text{{<something equal to 0 when }} (x,y,z) = (8, 4, 3)$
   $L_f(x,y,z) = 3 + \text{{<当 }} (x,y,z) = (8, 4, 3)\text{{ 时等于0的某些东西>}}$
   
2. To make sure that the remainder of the equation is 0 at $(x,y, z) = (8,4, 3)$ while keeping things linear, we only add constant multiples of the terms $(x - 8)$, $(y - 4)$, and $(z - 3)$.
   为了确保等式在 $(x,y, z) = (8,4, 3)$ 时余数为0，同时保持线性，我们只添加 $(x - 8)$, $(y - 4)$, 和 $(z - 3)$ 这些项的常数倍。
   
3. Since these will all be 0 at the input.
   因为这些在输入时都会为0。

4. $L_f(x,y,z) =3+a(x - 8) + b(y - 4) + c(z - 3)$
   $L_f(x,y,z) =3+a(x - 8) + b(y - 4) + c(z - 3)$

5. The partial derivatives of $L_f$, as you have written it so far, are precisely these constants a, b and c.
   到目前为止，你所写的$L_f$的偏导数就是这些常数a、b和c。

6. So to force our function to have the same partial derivative information as $f$ at the point $(8, 4,3)$, we just need to set these constants equal to the corresponding partial derivatives of $f$ at this point.
   所以，为了使我们的函数在点$(8, 4,3)$处具有与$f$相同的偏导数信息，我们只需要将这些常数设为该点$f$的相应偏导数。

7. Step 3: Compute each partial derivative of $f(x,y,z) = ze^{x^2 - y^3}$
   第3步：计算$f(x,y,z) = ze^{x^2 - y^3}$的每个偏导数

8.  Now we evaluate each of these at $(8, 4, 3)$.
    现在我们在$(8, 4, 3)$处评估这些值。

--- pic\Local linearization.pdf_06.png ---
1. Luckily, our computations are made easier by the fact that .
   幸运的是，我们的计算变得更容易，因为。

2. Step 4: Replacing the constants $a$, $b$ and $c$ in the expression of $L_f$ with these partial derivative values, what do you get?
   第4步：用这些偏导数值替换$L_f$表达式中的常数$a$、$b$和$c$，你会得到什么？

3. Now notice what this looks like if you write it with vector notation.
   现在注意，如果你用矢量记号写出来，这看起来是什么样的。


--- pic\Local linearization.pdf_07.png ---
1. It is just a specific form of the general formula shown above.
   这只是上面所示的一般公式的特定形式。

   $L_f (x) = f (x_0) + \nabla f(x_0)\cdot (x - x_0)$
   $L_f (x) = f (x_0) + \nabla f(x_0)\cdot (x - x_0)$

2. Example 2: Using local linearization for estimation
   示例2：使用局部线性化进行估计

3. What follows is by no means a practical application, but working through it will help give a feel for what local linearization is doing.
   下面的内容绝不是实际应用，但是通过它的学习可以帮助理解局部线性化在做什么。

4. Problem: Suppose you are on a desert island without a calculator, and you need to estimate $\sqrt{2.01 + \sqrt{0.99 + \sqrt{9.01}}}$. How would you do it?
   问题：假设你在一个没有计算器的荒岛上，你需要估算$\sqrt{2.01 + \sqrt{0.99 + \sqrt{9.01}}}$。你会怎么做？

5. Solution: We can view this problem as evaluating a certain 1. Solution: We can view this problem as evaluating a certain three-variable function at the point $(2.01,0.99,9.01)$,namely $f(x,y,z)=\sqrt{x + \sqrt{y + \sqrt{z}}}$
解决方案：我们可以将这个问题视为在点$(2.01,0.99,9.01)$处评估某个三变量函数，即$f(x,y,z)=\sqrt{x + \sqrt{y + \sqrt{z}}}$

1. I don't know about you, but I'm not sure how to evaluate square roots by hand. 
   我不知道你怎么想，但我不确定如何手动求解平方根。

1. Then working it out by hand would only involve adding and multiplying numbers.
    然后，手动求解只会涉及到加法和乘法运算。

7. What we could do is find the local linearization at a nearby point where evaluating $f$ is easier. 
   我们可以做的是在一个求解$f$更容易的附近点找到局部线性化。

1. Then we can get close to the right answer by evaluating the linearization at the point $(2.01,0.99,9.01)$.
   然后我们可以通过在点$(2.01,0.99,9.01)$处评估线性化来接近正确答案。

2. The point we care about is very close to the much simpler point $(2, 1,9)$, so we find the local linearization of $f$ near that point.
   我们关心的点离$(2, 1,9)$这个更简单的点非常近，所以我们找到$f$在那个点附近的局部线性化。

1. As before, we must find $f(2,1,9)$
和以前一样，我们必须找到$f(2,1,9)$

2. All partial derivatives of f at $(2,1,9)$
在$(2,1,9)$处的f的所有偏导数

3. The first of these is $f(2,1,9)$
其中的第一个是$f(2,1,9)$

--- pic\Local linearization.pdf_08.png ---
1. Looks like someone chose a few convenient input values, eh?
   看起来有人选择了一些方便的输入值，是吧？

2. On to the partial derivatives (heavy sigh). 
   现在来到了偏导数(深深叹息)。

3. Since the square roots are abundant, let's write out for ourselves the derivative of $\sqrt{x}$.
   由于平方根很多，让我们为自己写出$\sqrt{x}$的导数。

1. Okay, here we go. The simplest partial derivative is $f_x$
好的，我们开始吧。最简单的偏导数是$f_x$

2. Since y is nestled in there, $f_y$ requires some chain rule action:
由于y被嵌套在其中，$f_y$需要一些链式法则的操作：

3. Nestled even deeper, that tricky z will require two iterations of the chain rule:
嵌套得更深，那个棘手的z将需要两次链式法则的迭代：

4. Next, evaluate each one of these at $(2, 1,9)$.
   接下来，在$(2, 1,9)$这个点上评估每一个。

4. This might seem like a lot, but they are all made up of the same three basic components:
这可能看起来很多，但它们都是由相同的三个基本组成部分组成的：

5. Plugging these values into our expressions for the partial derivatives, we have
将这些值插入我们的偏导数表达式，我们得到了

--- pic\Local linearization.pdf_09.png ---
1. Unraveling the formula for local linearization, we get
   展开局部线性化的公式，我们得到

1. Finally, after all this work, we can plug in $(x, y, z) = (2.01, 0.99, 9.01)$ to compute our approximation
最后，在所有这些工作之后，我们可以插入$(x, y, z) = (2.01, 0.99, 9.01)$来计算我们的近似值

3. Calculating this by hand still isn't easy, but at least it's doable.
   手动计算这个仍然不容易，但至少是可以做到的。

4. When you work it out, the final answer is $2.001979$.
   当你算出来时，最终答案是$2.001979$。

5. So our approximation is pretty good! 
   所以我们的近似是相当好的！

2. Had we just used a calculator, the answer is
如果我们只是使用计算器，答案是

6. Why do we care?
   我们为什么关心？

--- pic\Local linearization.pdf_10.png ---
1. Although it is not common to find yourself estimating square roots on a desert island (at least where I'm from), what is common in the contexts of math and engineering is wrangling with complicated but differentiable functions.
   尽管在一个荒岛上估计平方根并不常见（至少在我来自的地方不常见），但在数学和工程学的背景下，常见的是与复杂但可微的函数打交道。

2. The phrase "just linearize it" is tossed around so much that not knowing what it means could be awkward.
   “只是线性化它”这个词语使用得太多，如果不知道它的意思可能会很尴尬。

3. Remember, a local linearization approximates one function near a point based on the information you can get from its derivative(s) at that point.
   请记住，局部线性化是基于你可以从该点的导数(们)获取的信息，在一个点附近对一个函数进行近似。

4. Even though you can use a computer to evaluate functions, that's not always enough.
   尽管你可以使用计算机来评估函数，但这并不总是足够的。

5. You might need to evaluate it many thousands of times per second, and working it out in full takes too long.
   你可能需要每秒评估它几千次，全面计算出来需要太长时间。

6. Maybe you don't even have the function explicitly written out, and you just have a few measurements near a point which you wish to extrapolate.
   也许你甚至没有明确写出函数，你只是有一些在点附近的测量值，你希望将其推断出来。

7. Sometimes what you care about is the inverse function, which can be hard or even impossible to find for the function as a whole, whereas inverting linear functions Is relatively straight-forward.
   有时你关心的是反函数，对于整个函数来说，找到反函数可能很难，甚至不可能，而反转线性函数相对来说比较直接。

8. Summary: Local linearization generalizes the idea of tangent planes to any multivariable function.
   总结：局部线性化将切平面的概念推广到任何多变量函数。

9.  The idea is to approximate a function near one of its inputs with a simpler function that has the same value at that input, as well as the same partial derivative values.
    这个想法是在函数的一个输入附近，用一个更简单的函数去近似这个函数，这个简单的函数在那个输入的地方有相同的值，以及相同的偏导数值。

10. Written with vectors, here's what the approximation function looks like:
    用向量表示，这就是近似函数的样子：

    $Ls(x) = f(x_0) + \nabla f(x_0) \cdot (x - x_0)$
    $Ls(x) = f(x_0) + \nabla f(x_0) \cdot (x - x_0)$

    x is the variable
    x是变量

11. This is called the local linearization of f near $x_0$.
    这被称为在$x_0$附近的f的局部线性化。