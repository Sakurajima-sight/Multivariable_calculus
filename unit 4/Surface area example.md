
--- pic\Surface area example.pdf_00.png ---

1. Surface area example
   表面积示例

2. Here you have the chance to practice computing surface area, using the example of a torus.
   在这里，你有机会使用一个环面（圆环形）的例子来练习计算表面积。

1. Who is this for?
   这是为谁准备的？

2. This article is meant for anyone who read the last article on computing the surface area of parametric surfaces using a certain double integral, and who wants to practice this concept.
   本文面向的是阅读了上一篇关于使用特定的二重积分计算参数曲面表面积的文章，并希望实践这个概念的人。

4. You will compute the surface area of a torus (a doughnut shape) using this method, which requires no small amount of computation.
   你将使用这种方法计算环面（甜甜圈形状）的表面积，这需要不少的计算。

1. If you neither want or need practice with this computation, and you feel comfortable with the general concept of how these surface area integrals work, feel free to skip ahead to the next article.
   如果你不需要或不想练习这个计算，而且你对这些表面积分的一般概念感到舒适，那么请随意跳到下一篇文章。

5. Quick recap of the surface area integral.
   快速回顾一下表面积积分。

6. Before diving into the example, leTs quickly remind ourselves of the method described for finding the area of a surface discussed in the last article.
   在深入研究例子之前，让我们快速回顾一下在上一篇文章中讨论的用于找到表面面积的方法。

1. Parameterize the surface.
   参数化表面。

2. In other words, find a vector-valued function $\mathbf{v}(t, s)$ which maps some region $T$ of the two-dimensional $ts$-plane onto your surface in three dimensions.
   换句话说，找到一个矢量值函数 $\mathbf{v}(t, s)$，它将二维 $ts$-平面上的某个区域 $T$ 映射到你的三维表面上。

1. Sometimes this parameterization will be given to you if that's how your surface is defined.
   有时候这种参数化会给你，如果这就是你的表面定义的方式。

2. Other times the surface is defined some other way, and you have to find it yourself.
   其他时候，表面以其他方式定义，你必须自己找出来。


--- pic\Surface area example.pdf_01.png ---

1. In the parameter space
   在参数空间

1. On the surface $S$
表面$S$

2. Imagine chopping up the parameter space with horizontal and vertical lines, thus dividing your region $T$ into little rectangles.
   想象一下用水平和垂直线切割参数空间，从而将你的区域$T$划分为小矩形。

3. Each of these rectangles gets mapped onto a little piece of your surface which Is well-approximated by a parallelogram.
   这些矩形中的每一个都映射到你的表面的一小部分，这部分可以被很好地近似为一个平行四边形。

4. If your little rectangle sits at the point $(t, s)$, and it has width $dt$ and height $ds$, you can approximate its area with the following expression: 
   如果你的小矩形位于点$(t, s)$，宽度为$dt$，高度为$ds$，那么你可以用以下表达式来近似其面积：

5. The smaller your initial rectangles, the more closely the corresponding piece of your surface resembles an actual flat parallelogram, and the closer this expression is to giving the true area of that piece.
   初始矩形越小，你的表面的相应部分越接近真正的平行四边形，这个表达式给出的面积就越接近那部分的真实面积。

6. Add up the areas of these pieces with a double integral:
   用双重积分将这些部分的面积加起来：

7. Surface area of a torus.
   圆环的表面积。

8. The goal of this article is to find the surface area of a torus.
   本文的目标是找到圆环的表面积。


--- pic\Surface area example.pdf_02.png ---

1. English makes it hard to describe the dimensions of this torus, but I'll give it a shot with the help of some doughnut terminology. 
   英语使得描述这个环形体的尺寸变得困难，但我会借助一些甜甜圈的术语尝试一下。

2. Imagine this torus as the glaze on a doughnut. 
   把这个环形体想象成甜甜圈上的糖衣。

1. Let's say the distance between the origin and the innermost part of this jelly filling is $3$.
   让我们假设原点和果冻填充的最内部之间的距离是$3$。

2. Call this the "outer radius".
   我们称这个为"外半径"。

4. Let's also say the distance between the innermost part of the jelly filling and the glaze itself is $1$.
   我们也可以说果冻填充的最内部和糖衣本身之间的距离是$1$。

1.  Call this the "inner radius" .
   我们称这个为"内半径"。

--- pic\Surface area example.pdf_03.png ---

1. With these dimensions, the torus (i.e. glaze) can be parameterized with the following function:
   有了这些维度，圆环体（即釉面）可以用以下函数进行参数化：

1. For this parameterization to cover the torus once and only once, apply it to the region of the $t$-$s$ plane where
   为了让这个参数化只覆盖一次圆环面，将其应用到$t$-$s$平面的区域。

2. For a description of where this parameterization comes from, check out the last example in this article.
   对于这个参数化从何处得来的描述，请查看本文中的最后一个例子。

3. Step 1: Compute each partial derivative
   步骤1：计算每个偏导数


--- pic\Surface area example.pdf_04.png ---

1. Remember, you should think of these vectors as representing the edges of little parallelograms, which piece together to make the torus as a whole.
   记住，你应该将这些向量视为代表小平行四边形的边，这些小平行四边形拼接在一起形成一个完整的圆环面。

2. More accurately, you must multiply the first one by $dt$ and the second one by $ds$ to scale them down to the infinitesimal size of one of these parallelograms.
   更准确地说，你必须将第一个乘以$dt$，将第二个乘以$ds$，将它们缩小到这些平行四边形之一的无穷小大小。

3. As it so happens, these vectors are perpendicular to each other (you can check by taking their dot product).
   正好，这些向量互相垂直（你可以通过取它们的点积来检查）。

4.  This implies all the little parallelograms making up the torus happen to be rectangles, at least when we use this particular parameterization.
    这意味着组成圆环面的所有小平行四边形恰好是矩形，至少在我们使用这种特定的参数化时是这样。

5.  You can see this in the picture of the torus above.
    你可以在上面的圆环面的图片中看到这一点。

6.  In the following steps, you will compute the area of one of these parallelograms by taking the cross product of the two vectors you just found, and computing its magnitude.
    在接下来的步骤中，你将通过取你刚刚找到的这两个向量的叉积，并计算其大小来计算这些平行四边形之一的面积。

7.  This is good practice for more general surface area computations.
    这对于更一般的表面积计算是一个很好的实践。

1. If you wanted to be clever, you could exploit the fact that these vectors happen to be perpendicular to each other.
   如果你想要聪明一点，你可以利用这些向量恰好彼此垂直的事实。

8.  Specifically, since the "parallelogram" they span will always be a rectangle, you can compute Its area by taking the magnitude of these two partial derivative vectors, and multiplying them together.
    具体来说，由于它们所跨越的"平行四边形"总是一个矩形，你可以通过取这两个偏导数向量的大小，并将它们相乘来计算其面积。

9.  Step 2: Compute the cross product.
    步骤2：计算叉积。

10. To find the area of a parallelogram spanned by the two vectors you just found, the first step is to take their cross product.
    要找到你刚刚找到的两个向量所跨越的平行四边形的面积，第一步是取它们的叉积。

2. (Warning: This one gets hairy)
   （警告：这个问题会变得复杂）

--- pic\Surface area example.pdf_05.png ---

1. It's best to calculate one component at a time.
   最好一次计算一个分量。

1. $i$-component : Cross out top row and left column, then take the determinant:
   $i$-分量：划掉顶行和左列，然后取行列式：

3. $j$-component : Cross out top row and middle column, then take the negative determinant:
   $j$-分量：划掉顶行和中列，然后取负行列式：

4. $k$-component : This one is nastier than the last two.
   $k$-分量：这一个比前两个更难处理。

5. Cross out top row and right column, then take the determinant:
   划掉顶行和右列，然后取行列式：

--- pic\Surface area example.pdf_06.png ---

1. Step 3: Find the magnitude of this cross product.
   步骤3：找到这个叉积的大小。

1. The cross product you just computed is a vector.
   你刚计算的叉积是一个向量。

2. In order to find the area of a parallelogram spanned by the two partial derivative vectors, we must find its magnitude.
   为了找到由两个偏导数向量跨度的平行四边形的面积，我们必须找到它的大小。

3. (Warning: This one gets even more hairy). 
   （警告：这个问题会变得更加复杂）。

1. Plugging in the answer we found in the last example, we get something which is at first enormous, but then simplifies down quite nicely.
   将我们在上一个例子中找到的答案代入，我们得到的结果起初看起来很大，但最后却可以简化得很好。

--- pic\Surface area example.pdf_07.png ---

1. Factor out $(3 + \cos(s))^2 \cos^2(s)$
   提取出$(3 + \cos(s))^2 \cos^2(s)$因子

2. Factor out $(3 + \cos(s)^2)$
   提取出$(3 + \cos(s)^2)$因子

3. Once you scale this down by $dt ds$, this tells you the area of each of the little parallelograms making up the torus, as a function of $s$ and $t$. 
   一旦你用$dt ds$缩小这个，这将告诉你构成圆环体的每一个小平行四边形的面积，作为$s$和$t$的函数。

4. Well, in this case, the answer Is just a function of $s$, which means the area of these parallelograms doesn't change as you let $t$ vary.
   好的，在这种情况下，答案只是$s$的函数，这意味着当你让$t$变化时，这些平行四边形的面积并不会改变。

5. Step 4: Set up the appropriate double integral
   步骤4：设立适当的双重积分

6. Which of the following represents the right bounds to place on the double integral representing surface area for this torus? 
   下列哪个代表了对表示这个圆环体表面积的双重积分设定的正确边界？

7. The third answer choice is correct:
   第三个答案选项是正确的：

--- pic\Surface area example.pdf_08.png ---

1. This comes from the definition for our parameterization of this torus given at the start of this section.
   这来自我们在本节开始时给出的对这个环面的参数化的定义。

2. In particular, both $t$ and $s$ range from $0$ to $2\pi$.
   特别地，$t$和$s$的范围都是从$0$到$2\pi$。

3. Step 5: Compute the double integral  
   步骤5：计算双重积分

1. Surface area of this torus:
这个环面的表面积：

1. First take the result from step 3: 
   首先取第3步的结果：

2. Then applying the double integral from step 4: 
   然后应用第4步的双重积分：

1. Integrating a constant with respect to $t$
对常数关于$t$进行积分

1.  There is something quite nice about this result.
    这个结果有些非常好的地方。

2.  The specific torus we chose has an outer radius of 3 and an inner radius of 1.
    我们选择的特定环面有一个外半径为3，内半径为1。

1. This gives the feeling that if you cut the torus and "unroll" it, you will get a flat rectangle with side lengths $2\pi(3)$ and $2\pi(1)$, since the circumference of a circle with radius $r$ is $2\pi r$.
   这给人的感觉是，如果你切开圆环并将其“展开”，你将得到一个扁平的矩形，其边长为 $2\pi(3)$ 和 $2\pi(1)$，因为半径为 $r$ 的圆的周长是 $2\pi r$。

--- pic\Surface area example.pdf_09.png ---

1. Of course, this "unrolling" process involves stretching the inner parts of the torus, and squishing its outer parts, so there is no guarantee that surface area will be preserved. 
   当然，这个“展开”过程涉及到拉伸圆环的内部部分，和挤压其外部部分，所以不能保证表面积会被保留。

2. Nevertheless, the area of that rectangle is 
   尽管如此，该矩形的面积是

3. This is the same as the surface area of our torus.
   这与我们的圆环的表面积相同。

4. This means that, in a sense, the stretching and squishing of this unrolling process perfectly cancel out!
   这意味着，从某种意义上说，这个展开过程中的拉伸和挤压完美地抵消了！

1. Congratulations!
   祝贺你！

2. These integrals are a lot of work, so pat yourself on the back for working all the way through this!
   这些积分工作量很大，所以为你一直坚持到现在的努力给自己一个鼓励！
