
--- pic\Maxima, minima, and saddle points.pdf_00.png ---

1. Maxima, minima, and saddle points
   极大值，极小值，和鞍点

2. Learn what local maxima/minima look like for multivariable function.
   学习多元函数的局部极大值/极小值看起来是什么样的。

3. Background: Graphs, The gradient
   背景：图形，梯度

4. Intuitively, when you're thinking in terms of graphs, local maxima of multivariable functions are peaks, just as they are with single variable functions.
   从直观上来说，当你从图形的角度考虑时，多元函数的局部极大值是峰值，就像单变量函数一样。

5. The gradient of a multivariable function at a maximum point will be the zero vector, which corresponds to the graph having a flat tangent plane.
   在最大点，多元函数的梯度将是零向量，这对应于图形有一个平坦的切平面。

6. Formally speaking, a local maximum point is a point in the input space such that all other inputs in a small region near that point produce smaller values when pumped through the multivariable function $f$.
   正式来说，局部最大点是输入空间中的一个点，该点附近的小区域中的所有其他输入在通过多元函数 $f$ 处理时都会产生更小的值。

7. In general, the graph of a function with n variables exists in an $(n + 1)$-dimensional space, and its tangent is an n-dimensional space.
   一般来说，具有 n 个变量的函数的图形存在于 $(n + 1)$ 维空间中，其切线是 n 维空间。

8. For example, the graph of a single variable function is two-dimensional and its tangent is a one-dimensional line; the graph of a two-variable function is three-dimensional and its tangent is a two-dimensional plane.
   例如，单变量函数的图形是二维的，其切线是一维线；两变量函数的图形是三维的，其切线是二维平面。

9. For functions with three variables or more, the tangent won't be a plane anymore, since a plane is necessarily two-dimensional.
   对于具有三个或更多变量的函数，切线将不再是平面，因为平面必须是二维的。

10. The formal term for a subspace that has one dimension less than its ambient space is hyperplane. 
    小于其环境空间一个维度的子空间的正式术语是超平面。

1. So, formally, the gradient of a multivariable function corresponds to a tangent hyperplane.
因此，正式地说，多元函数的梯度对应于一个切超平面。

11. In this article, we will keep calling the tangent a plane, because all of our examples use two-variable functions.
    在这篇文章中，我们将继续称切线为平面，因为我们所有的例子都使用两变量函数。

12. Nevertheless, it's important to remember that formally, we are talking about hyperplanes.
    然而，重要的是要记住，正式地说，我们在讨论超平面。

--- pic\Maxima, minima, and saddle points.pdf_01.png ---

1. Optimizing in higher dimensions
    在更高维度优化

14. One of the most important applications of calculus is its ability to sniff out the maximum or the minimum of a function.
    微积分最重要的应用之一是它能够找出函数的最大值或最小值。

15. Perhaps you find yourself running a company, and you've come up with some function to model how much money you can expect to make based on a number of parameters, such as employee salaries, cost of raw materials, etc.
    也许你发现自己正在经营一家公司，你想出了一种函数模型，根据一些参数（如员工薪水、原材料成本等）预测你可以赚多少钱。

16. Maybe you are designing a car, hoping to make it more aerodynamic, and you've come up with a function modelling the total wind resistance as a function of many parameters that define the shape of your car, and you want to find the shape that will minimize the total resistance.
    也许你正在设计一辆车，希望让它更具空气动力性，你想出了一个函数模型，它以定义汽车形状的许多参数为函数，模拟总风阻，你想找到可以使总阻力最小化的形状。

17. In machine learning and artificial intelligence, the way a computer "learns' how to do something is commonly to minimize some "cost function" that the programmer has specified.
    在机器学习和人工智能中，计算机“学习”如何做某事的常见方法是最小化程序员指定的某种“成本函数”。

1. Local maxima and minima, visually
局部最大值和最小值，直观地看

18. Let's start by thinking about those multivariable functions which we can graph: Those with a two-dimensional input, and a scalar output, like this:
    让我们开始考虑那些我们可以绘制图形的多元函数：具有二维输入和标量输出的函数，就像这样：

19. $f(x,y) = cos(x) cos(y)e^*$
    $f(x,y) = cos(x) cos(y)e^*$ 1. x

20. I chose this function because it has lots of nice little bumps and peaks. 
    我选择了这个函数，因为它有很多好看的小凸起和峰值。

1. We call one of these peaks a local maximum, and the plural is local maxima.
我们把其中的一个峰值叫做局部最大值，复数形式是局部最大值。

--- pic\Maxima, minima, and saddle points.pdf_02.png ---

1. These are all local maxima
    这些都是局部最大值

22. The point $(x_0, y_0)$ underneath a peak in the input space (which in this case means the xy-plane) is called a local maximum point. 
    在输入空间（在这种情况下，意味着xy平面）下的峰顶处的点 $(x_0, y_0)$ 被称为局部最大点。

23. The output of a function at a local maximum point, which you can visualize as the height of the graph above that point, is the local maximum itself.
    在局部最大点处函数的输出，你可以将其视为图上该点的高度，就是局部最大值本身。

24. The word "local" is used to distinguish these from the global maximum of the function, which ts the single greatest value that the function can achieve.
    "局部"这个词是用来区分这些和函数的全局最大值，全局最大值是函数可以达到的单个最大值。

25. If you are on the peak of a mountain, it's a local maximum, but unless that mountain is Mt. Everest, it is not a global peak.
    如果你在山峰上，那是一个局部最大值，但除非那座山是珠穆朗玛峰，否则它不是全局峰值。

1. I'll give you the formal definition of a local maximum point at the end of this article.
我将在本文的最后给出局部最大点的正式定义。

2. Intuitively, it is a special point in the input space where taking a small step in any direction can only decrease the value of the function.
直观地说，它是输入空间中的一个特殊点，从这个点沿任何方向小步移动只会降低函数的值。

3.  Similarly, if the graph has an inverted peak at a point, we say the function has a local minimum point at the value $(x, y)$ above/below this point on the $xy$-plane, and the value of the function at this point is a local minimum.
    类似地，如果图在一点有一个倒置的峰值，我们说函数在$xy$平面上这一点上方/下方的值 $(x, y)$ 处有一个局部最小点，而这一点上函数的值就是局部最小值。

4.  Intuitively, these are points where stepping in any direction can only increase the value of the function.
    从直观上看，这些点在任何方向上的步行都只会增加函数的值。

--- pic\Maxima, minima, and saddle points.pdf_03.png ---
1. These are all local minima
这些都是局部最小值

1. Stable points in one variable (review)
单变量中的稳定点（回顾）

1. You may remember the idea of local maxima/minima from single-variable calculus, where you see many problems like this:
你可能记得单变量微积分中的局部最大/最小值的概念，在那里你会看到许多这样的问题：

--- pic\Maxima, minima, and saddle points.pdf_04.png ---

1.  Concept check: For what value $x$ is the function $f(x) = -(x - 2)^2 + 5$ the greatest? What is the maximum value?
    概念检查：对于什么值 $x$，函数 $f(x) = -(x - 2)^2 + 5$ 是最大的？最大值是多少？

2.  The tangent line at any local maximum will have slope 0, so we look for points where $f'(x) = 0$:
    任何局部最大值处的切线斜率都将为0，所以我们寻找使 $f'(x) = 0$ 的点：

3.  $f'(x) = -2(x - 2) = 0$
    $f'(x) = -2(x - 2) = 0$

4.  In this case, the only solution is $x = 2$, at which point $f$ has the value $f(2) = -(2-2)^2+5=5$.
    在这种情况下，唯一的解是 $x = 2$，在这一点，$f$ 的值为 $f(2) = -(2-2)^2+5=5$。

5.  To check that this is really a maximum, and not a minimum or an inflection point, you could take the second derivative and confirm that it is negative at the point $x = 2$.
    为了确认这真的是一个最大值，而不是最小值或拐点，你可以取二阶导数，并确认在点 $x = 2$ 处它是负的。

1. In general, local maxima and minima of a function f are studied by looking for input values a where $f'(a) = 0$.
一般来说，函数f的局部最大值和最小值是通过寻找满足$f'(a) = 0$的输入值a来研究的。

2. This is because as long as the function is continuous and differentiable, the tangent line at peaks and valleys will flatten out, in that it will have a slope of 0.
这是因为只要函数是连续且可微的，峰值和谷值处的切线会变平，即它的斜率为0。

3. Such a point a has various names: Stable point, Critical point, Stationary point.
这样的点a有各种名称：稳定点、临界点、静止点。

1.  All of these mean the same thing: $f'(a) = 0$
所有这些都意味着同一件事：$f'(a) = 0$

4. The requirement that f be continuous and differentiable is important, for if it was not continuous, a lone point of discontinuity could be a local maximum.
要求f是连续且可微的是很重要的，因为如果它不连续，一个孤立的不连续点可能是一个局部最大值。

--- pic\Maxima, minima, and saddle points.pdf_05.png ---

1. And if f is continuous but not differentiable, a local maximum could look like this:
如果函数$f$是连续的但不可微的，局部最大值可能看起来像这样：

1.  In either case, talking about tangent lines at these maximum points doesn't really make sense, does it?
    在任何情况下，谈论这些最大点处的切线真的有意义吗？

2. However, even when f is continuous and differentiable, it is not enough for the derivative to be 0, since this also happens at inflection points:
然而，即使函数$f$是连续的并且可微的，导数为0也不够，因为在拐点处也会发生这种情况：

--- pic\Maxima, minima, and saddle points.pdf_06.png ---

1. This means finding stable points is a good way to start the search for a maximum, but it is not necessarily the end.
    这意味着寻找稳定点是开始寻找最大值的好方法，但这并不一定是结束。

38. The story is very similar for multivariable functions.
    对于多变量函数，情况非常相似。

1. Stable points in two variables
两个变量的稳定点

39. When the function is continuous and differentiable, all the partial derivatives will be 0 at a local maximum or minimum point.
    当函数是连续且可微的，所有的偏导数在局部最大或最小点处都会为0。

40. $f_x (x_0, y_0,...) = 0$
    $f_x (x_0, y_0,...) = 0$

41. Partial with respect to x
    关于x的偏导数

42. $f_y (x_0, y_0,...) = 0$
    $f_y (x_0, y_0,...) = 0$

43. Partial with respect to y
    关于y的偏导数

44. With respect to the graph of a function, this means its tangent plane will be flat at a local maximum or minimum.
    对于函数的图，这意味着它的切平面在局部最大或最小处将是平的。

1.  For instance, here is a graph with many local extrema and flat tangent planes on each one:
例如，这是一个图，其中有许多局部极值，每个极值上都有一个平的切平面：

--- pic\Maxima, minima, and saddle points.pdf_07.png ---

1. Saying that all the partial derivatives are zero at a point is the same as saying the gradient at that point is the zero vector.
    在一个点上所有偏导数为零，就等于说那个点的梯度是零向量。

46. People often write this more compactly like this: $∇f(x_0) = 0$
    人们经常用更紧凑的方式来写这个: $∇f(x_0) = 0$

47. The convention ts that bold variable are vectors. 
    约定粗体变量是向量。

1. So x 0 is a vector of the input values $(x_0, y_0, \ldots)$ and 0 is the vector with all zeros.
所以，$x_0$ 是输入值 $(x_0, y_0, \ldots)$ 的向量，而 0 是所有元素都为零的向量。

1. Such an input $x_0$ goes by the same various names as in the single-variable case:
这样的输入$x_0$在单变量情况下有相同的各种名称：

2. Stable point
稳定点

3. Stationary point
静止点

4. Critical point
临界点

--- pic\Maxima, minima, and saddle points.pdf_08.png ---

1. The thinking behind the words "stable" and "stationary" is that when you move around slightly near this input, the value of the function doesn't change significantly.
    "稳定"和"静止"这两个词背后的思想是，当你在这个输入附近稍微移动时，函数的值不会显著改变。

50. The word "critical" always seemed a bit over dramatic to me, as if the function Is about to die near those points.
    "临界"这个词对我来说总是显得有点夸张，就好像函数在那些点附近即将死亡。

51. As with single variable functions, it is not enough for the gradient to be zero to ensure that a point is a local maximum or minimum.
    就像单变量函数一样，只有梯度为零是不足以确保一个点是局部最大值或最小值的。

52. For one thing, you can still have something similar to an inflection point.
    对于一件事，你仍然可以有类似于拐点的东西。

53. But there Is also an entirely new possibility, unique to multivariable functions. 
    但也有一种完全新的可能性，这是多变量函数的独特性。

1. Saddle points
马鞍点。

54. Consider the function $f(x, y) = x^2-y^2$. 
    考虑函数$f(x, y) = x^2-y^2$。

1. Let's make a few observations about what goes on around the origin $(0, 0)$
让我们对原点$(0, 0)$周围发生的情况做一些观察。

55. Both partial derivatives are 0 at this point: $∂f/∂x = 0$ and $∂f/∂y = 0$.
    在这一点上，两个偏导数都为0: $∂f/∂x = 0$ 和 $∂f/∂y = 0$.

--- pic\Maxima, minima, and saddle points.pdf_09.png ---

1. Therefore $(0,0)$ is a stable point.
    因此，$(0,0)$ 是一个稳定点。

57. When you just move in the $x$ direction around this point, the function looks like $f(x, 0) = x^2-0= x^2$.
    当你仅在此点附近的 $x$ 方向移动时，函数看起来像 $f(x, 0) = x^2-0= x^2$。

58. The single-variable function $f(x) = x^2$ has a local minimum at $x = 0$.
    单变量函数 $f(x) = x^2$ 在 $x = 0$ 处有一个局部最小值。

59. When you just move in the $y$ direction around this point, meaning the function looks like $f(0, y) = 0-y^2= -y^2$.
    当你仅在此点附近的 $y$ 方向移动时，函数看起来像 $f(0, y) = 0-y^2= -y^2$。

60. The single-variable function $f(y) = -y^2$ has a local maximum at $y = 0$.
    单变量函数 $f(y) = -y^2$ 在 $y = 0$ 处有一个局部最大值。

61. In other words, the $x$ and $y$ directions disagree over whether this input should be a maximum or a minimum point.
    换句话说，$x$ 和 $y$ 方向对于这个输入应该是最大值点还是最小值点意见不一致。

62. So even though $(0, 0)$ is a stable point, and is not an inflection point, it cannot be a local maximum or local minimum!
    所以即使 $(0, 0)$ 是一个稳定点，并且不是拐点，它也不能是局部最大值或局部最小值！

63. Doesn't the region around $(0, 0,0)$ kind of have the shape of a horse's saddle?
    周围 $(0, 0,0)$ 的区域不是有点像马鞍的形状吗？

--- pic\Maxima, minima, and saddle points.pdf_10.png ---

1. Well, mathematicians thought so, and they had one of those rare moments of deciding on a good name for something: Saddle points.
    好吧，数学家们就是这么认为的，他们有一种罕见的决定给某物起一个好名字的时刻：马鞍点。

65. By definition, these are stable points where the function has a local maximum in one direction, but a local minimum in another direction.
    根据定义，这些稳定点在一个方向上函数有一个局部最大值，但在另一个方向上有一个局部最小值。

1. Testing maximality/minimality
测试最大性/最小性

66. "Alright," I hear you saying, "so it's not enough for the gradient to be 0 since you might have an inflection point or a saddle point.
    "好的，"我听到你说，"所以只有梯度为0是不够的，因为你可能会有一个拐点或一个马鞍点。

1. But how can you tell if a stable point is a local maximum or minimum?
但是你怎么知道一个稳定点是局部最大值还是局部最小值呢？

67. This is the topic of the next article on the second partial derivative test.
    这是下一篇关于二阶偏导数检验的文章的主题。

68. For now, let's finish things off with a formal definition of a local maximum.
    现在，让我们用局部最大值的正式定义来结束。

1. Formal definition
正式定义

69. I've said this before, but the reason to learn formal definitions, even when you already have an intuition, is to expose yourself to how intuitive mathematical ideas are captured precisely.
    我之前说过，学习正式定义的原因，即使你已经有了直觉，也是为了让自己暴露在如何精确捕获直觉数学概念的方式中。

70. It's good practice for thinking clearly, and it can also help to understand those times when intuition differs from reality.
    这是明确思考的好习惯，也可以帮助理解直觉与现实不符的时候。

71. In defining a local maximum, let's use vector notation for our input, writing it as $x$.
    在定义局部最大值时，让我们使用向量记法表示我们的输入，记作 $x$。

--- pic\Maxima, minima, and saddle points.pdf_11.png ---

1. Formal definition of a local maximum: A scalar-valued function $f$ has a local maximum at $x_0$ If there exists some positive number $r > 0$, thought of as a radius, such that the following statement is true: $f(x) \leq f(x_0)$ for all $x$ such that $||x — x_0|| <r$
    局部最大值的正式定义：如果存在某个正数$r > 0$，被视为半径，使得以下语句成立：对于所有满足$||x — x_0|| <r$的$x$，有$f(x) \leq f(x_0)$，则标量值函数$f$在$x_0$处有一个局部最大值。

73. Saying "$||x — x_0|| < r$" means the variable $x$ is within a distance $r$ of the maximum point $x_0$.
    说 "$||x — x_0|| < r$" 意味着变量 $x$ 在最大点 $x_0$ 的 $r$ 距离内。

74. When $x$ is two-dimensional this is the same as saying $x$ lies inside a circle of radius $r$ centered at the point $x_0$.
    当 $x$ 是二维的，这相当于说 $x$ 位于以点 $x_0$ 为中心、半径为 $r$ 的圆内。

75. More generally, if $x$ is n-dimensional, the set of all $x$ such that $||x — x_0|| <r$ forms an n-dimensional ball with radius $r$ centered at $x_0$.
    更一般地，如果 $x$ 是 n 维的，所有满足 $||x — x_0|| <r$ 的 $x$ 组成了一个以 $x_0$ 为中心、半径为 $r$ 的 n 维球。

--- pic\Maxima, minima, and saddle points.pdf_12.png ---

1. We can then translate this definition from math-speak to something more closely resembling English as follows: 
    然后我们可以将这个定义从数学语言翻译成更接近英语的形式：

1. $x_0$ is a maximum point of $f$ if there is some small (ball-shaped) region in the input space around the point $x_0$ such that the highest possible value you can get for $f$ evaluated on points in that region is achieved at the point $x_0$.
如果在点 $x_0$ 周围的输入空间中有一个小的（球形的）区域，使得你在该区域内的点上评估 $f$ 可以得到的最高可能值在点 $x_0$ 处获得，那么 $x_0$ 就是 $f$ 的最大点。

77. Test your understanding: Write the formal definition for a local minimum, and think about what each component means as you write it down.
    测试你的理解：写出局部最小值的正式定义，并在写下它的过程中思考每个组成部分的含义。

78. Resist the temptation to just copy down the words in the definition above.
    抵制仅仅抄写上面定义中的词语的诱惑。

1. A scalar-valued function f has a local minimum at $x_0$ if there exists some positive number $r > 0$ such that $f ( x ) ≥ f ( x_0 )$ for all $x$ such that $|| x − x_0 || < r$.
如果存在某个正数$r > 0$，使得对于所有满足$|| x − x_0 || < r$的$x$，都有$f ( x ) ≥ f ( x_0 )$，那么标量值函数$f$在$x_0$处有一个局部最小值。

1. Summary
总结

2. Intuitively, when you're thinking in terms of graphs, local maxima of multivariable functions are peaks, just as they are with single variable functions.
直观地说，当你在图形的角度思考时，多变量函数的局部最大值就像单变量函数一样，是峰值。

--- pic\Maxima, minima, and saddle points.pdf_13.png ---

1.  The gradient of a multivariable function at a maximum point will be the zero vector, which corresponds to the graph having a flat tangent plane.
    在最大值点处，多变量函数的梯度将是零向量，这对应于图形具有平坦的切平面。

2.  Formally speaking, a local maximum point is a point in the input space such that all other inputs in a small region near that point produce smaller values when pumped through the multivariable function $f$.
    从形式上讲，局部最大值点是输入空间中的一个点，使得在该点附近的小区域内的所有其他输入在通过多变量函数 $f$ 时产生较小的值。