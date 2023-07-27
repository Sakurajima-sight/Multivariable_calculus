
--- pic\Constructing a unit normal vector to curve.pdf_00.png ---

1. Constructing a unit normal vector to curve
   构造曲线的单位法向量

2. Given a curve in two dimensions, how do you find a function which returns unit normal vectors to this curve?
   给定二维空间中的一条曲线，如何找到一个函数，该函数返回这条曲线的单位法向量？

3. Background
   背景

4. Derivatives of vector-valued functions
   向量值函数的导数

5. What we're building to
   我们要构建什么

6. A unit normal vector to a two-dimensional curve is a vector with magnitude 1 that is perpendicular to the curve at some point.
   对二维曲线的单位法向量是一个大小为1的向量，在某点垂直于曲线。

7. Typically you look for a function that gives you all possible unit normal vectors of a given curve, not just one vector.
   通常，你会寻找一个函数，这个函数给出了给定曲线的所有可能的单位法向量，而不仅仅是一个向量。

8. To find the unit normal vector of a two-dimensional curve, take the following steps:
   要找到二维曲线的单位法向量，请执行以下步骤：

9. Find the tangent vector, which requires taking the derivative of the parametric function defining the curve.
   找到切向量，这需要对定义曲线的参数函数求导。

10. Rotate that tangent vector $90^\circ$, which involves swapping the coordinates and making one of them negative.
    将该切向量旋转$90^\circ$，这涉及到交换坐标并将其中一个坐标设为负。

11. Normalize the result, which requires dividing it by its own magnitude .
    规范化结果，这需要将其除以其自身的大小 。

--- pic\Constructing a unit normal vector to curve.pdf_01.png ---

1. Abstractly speaking, the result you get will look something like this:
   抽象地讲，你得到的结果可能看起来像这样：

2. For a given tiny step along the curve, think of $dx$ as the $x$-component of that step, $dy$ as the $y$-component of that step, and $ds$ as the length of that step.
   对于沿曲线的一个小步长，把$dx$想象成步长的$x$分量，$dy$作为步长的$y$分量，而$ds$是步长的长度。

3. Example: Normal vectors to a sine curve
   示例：正弦曲线的法向量

4. Consider the graph of the function $f(x) = \sin(x)$.
   考虑函数图像$f(x) = \sin(x)$。

5. Imagine you want a function that gives you unit normal vectors to this curve (perhaps because you wish to compute flux through it).
   假设你需要一个函数，能给出这个曲线的单位法向量（也许是因为你希望计算穿过它的通量）。

6. In other words, for any point on the curve, you want to be able to give the coordinates of a vector perpendicular to that curve with magnitude $1$.
   换句话说，对于曲线上的任何一点，你希望能给出一个垂直于该曲线且大小为$1$的向量的坐标。

7. This means you want an expression that can take any point on the curve, and return a vector with magnitude $1$ that is perpendicular to the curve at that point.
   这意味着你需要一个表达式，它能够取曲线上的任何一点，并返回在该点上垂直于曲线的大小为$1$的向量。


--- pic\Constructing a unit normal vector to curve.pdf_02.png ---

1. Step 0: Parameterize
   步骤0：参数化

2. Before anything, we need to make sure our curve is in parametric form.
   在开始之前，我们需要确保我们的曲线是以参数形式给出的。

3. Turning a function graph into a parametric function is simple enough. 
   将函数图转化为参数函数是相当简单的。

4. We let the parameter $t$ play the role of $x$:
   我们让参数 $t$ 扮演 $x$ 的角色：

5. I call this "Step 0" because often your curve is initially defined parametrically in the first place, so this would be given to you for free. 
   我称这为“步骤0”，因为通常你的曲线一开始就是以参数形式定义的，所以这会直接给你提供。

6. What this means for our unit normal vector is that we will find a second vector-valued function which also takes in $t$, but instead of outputting points on the sine curve itself, its outputs will be unit vectors normal to the curve at the point $v(t)$.
   这对我们的单位法向量来说意味着我们将找到第二个向量值函数，它也接受 $t$，但是它不输出正弦曲线上的点，而是输出在点 $v(t)$ 处的曲线的单位法向量。

1. Step 1: Find a tangent vector.
步骤1：找到切线向量。

2. When you take the derivative of the parametric function, it will give you a tangent vector to the curve:
当你对参数函数求导时，它会给你曲线的切线向量：

--- pic\Constructing a unit normal vector to curve.pdf_03.png ---

1. If this seems unfamiliar, consider reviewing the article on derivatives of vectorvalued functions.
   如果这看起来不熟悉，可以考虑复习一下关于向量值函数导数的文章。

2. For our example, here's what that looks like:
   对于我们的例子，看起来像这样：

3. For example, if you plug in $t = \pi$ to this function, you get the following vector
   例如，如果你将 $t = \pi$ 代入这个函数，你将得到以下向量


4. When you move this vector so that its tail sits at the point $v(\pi)$, which for our sine curve is $(\pi, 0)$, it will be tangent to the curve.
   当你移动这个向量，使其尾部位于点 $v(\pi)$，对于我们的正弦曲线来说是 $(\pi, 0)$，它将会切于曲线。

--- pic\Constructing a unit normal vector to curve.pdf_04.png ---

1. Step 2: Rotate this vector 90°
   步骤2：将此向量旋转90°。



2. To turn a tangent vector into a normal vector, rotate it by 90°.
   要将切向量转化为法向量，就要将其旋转90°。

3. How do you do this?
   如何做到这一点呢？

4. Swap the two components and make one of them negative:
   交换两个组成部分，然后使其中一个为负：

5. How do you choose which component to make negative?
   你如何选择哪个组分要变为负数？

6. If you are rotating counterclockwise, make the first component negative; if you are rotating clockwise, make the second component negative.
   如果你逆时针旋转，让第一个组分为负；如果你顺时针旋转，让第二个组分为负。

--- pic\Constructing a unit normal vector to curve.pdf_05.png ---

1. In our example, let's rotate the tangent vector counterclockwise so that it points up.
   在我们的例子中，让我们逆时针旋转切线向量，使其向上指：

2. Step 3: Scale it to magnitude 1.
   第三步：将其缩放到大小为1。

1. Great! We have a normal vector. 
   很好！我们有一个法向量。

2. But to make this a unit normal vector, we must divide it by its own magnitude.
   但是要使其成为单位法向量，我们必须除以其自身的大小。

4. In our example, the magnitude is as follows:
   在我们的例子中，大小如下：

5. Therefore, our unit normal vector function  $n(t)$ looks like this:
   因此，我们的单位法向量函数$n(t)$是这样的：

6. Summary: Let's generalize the steps of this example to see how they apply to any parametric curve.
   总结：让我们将这个例子的步骤进行概括，看看它们如何应用到任何参数曲线。

--- pic\Constructing a unit normal vector to curve.pdf_06.png ---

1. Step 0: Make sure the curve is given parametrically.
   步骤0：确保曲线是以参数形式给出的。

2. Step 1: Find a tangent vector to your curve by differentiating the parametric function.
   步骤1：通过对参数函数求导来找到曲线的切线向量。

1. Step 2: Rotate this vector 90° by swapping the coordinates and making one negative.
   步骤2：通过交换坐标并使其中一个坐标取负值，将此向量旋转90°。

2. Tangent vector 
   切线向量

1. Normal vector
法线向量

4. Step 3: To make this a unit normal vector, divide it by its magnitude.
   步骤3：要使此向量成为单位法向量，将其除以其大小。

5. If you prefer, you can think in terms of differentials, with a tiny step along the curve being represented by the vector $\begin{bmatrix} x \\ y \end{bmatrix}$.
   如果你愿意，你可以从微分的角度来思考，用向量 $\begin{bmatrix} x \\ y \end{bmatrix}$ 表示沿曲线的一个微小步长。

6. The magnitude of this step is $ds = \sqrt{dx^2+dy^2}$.
   这个步长的大小是$ds = \sqrt{dx^2+dy^2}$。

1. In this terminology, you might instead write down the unit normal vector like this:
在这种术语中，你可能会这样写下单位法向量：
