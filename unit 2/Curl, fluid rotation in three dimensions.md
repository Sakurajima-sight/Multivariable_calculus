
--- pic\Curl, fluid rotation in three dimensions.pdf_00.png ---
1. Curl, fluid rotation in three dimensions
   旋度，三维流体旋转

2. Curl is an operator which measures rotation in a fluid flow indicated by a three-dimensional vector field.
   旋度是一种运算符，用于测量由三维向量场表示的流体流动中的旋转。

3. Background
   背景

4. Partial derivatives
   偏导数

5. Vector fields
   向量场

6. Cross product
   向量叉积

7. Curl warmup
   旋度热身

8. Note: Throughout this article I will use the convention that
   注意：在本文中，我将使用以下约定

10. i represents the unit vector in the x-direction. 
    i 代表x方向上的单位向量。

10. j represents the unit vector in the y-direction. 
    j 代表y方向上的单位向量。

10. k represents the unit vector in the z-direction. 
    k 代表z方向上的单位向量。

10. What we're building to
    我们要建立的是

11. Curl is an operator which takes in a function representing a three-dimensional vector field and gives another function representing a different three-dimensional vector field.
    旋度是一种运算符，它接受代表三维向量场的函数，输出代表不同的三维向量场的另一函数。

12. If a fluid flows in three-dimensional space along a vector field, the rotation of that fluid around each point, represented as a vector, is given by the curl of the original vector field evaluated at that point.
    如果流体在三维空间的向量场中流动，那么流体围绕每个点的旋转，表示为向量，由在该点评估的原始向量场的旋度给出。

13. The curl vector field should be scaled by one-half if you want the magnitude of curl vectors to equal the rotational speed of the fluid.
    如果你想让旋度向量的大小等于流体的旋转速度，那么旋度向量场应该缩小一半。

14. If a three-dimensional vector-valued function $\mathbf{v}$(x, y, z)$$ has component functions $\mathbf{v_1}$(x, y, z)$$, $\mathbf{v_2}$(x, y, z)$$ and $\mathbf{v_3}$(x, y, z)$$, the curl is computed as follows:
    如果一个三维向量值函数$\mathbf{v}$(x, y, z)$$有组成函数$\mathbf{v_1}$(x, y, z)$$, $\mathbf{v_2}$(x, y, z)$$和$\mathbf{v_3}$(x, y, z)$$，旋度的计算如下：

15. Notation for curl
    旋度的符号表示

16. Describing rotation with a vector
    用向量描述旋转

17. lf an object is rotating in two dimensions, you can describe the rotation completely with a single number: the angular velocity.
    如果一个物体在二维空间内旋转，你可以用一个单独的数值来完全描述旋转：角速度。

18. A positive angular
velocity indicates a counter-clockwise rotation while a negative number
indicates a clockwise rotation. 
    正的角速度表示逆时针旋转，而负数表示顺时针旋转。

--- pic\Curl, fluid rotation in three dimensions.pdf_01.png ---

1. The absolute value of the angular velocity gives the speed of rotation, typically in radians per second.
    角速度的绝对值给出了旋转的速度，通常以每秒弧度为单位。

2.  Rotation in two dimensions is described with a single number.
    二维旋转用一个单一的数字描述。

3.  For an object rotating in three dimensions, the situation is more complicated.
    对于在三维空间内旋转的物体，情况更为复杂。

4.  We need to represent both angular velocity and the direction in three-dimensional space in which the object is rotating.
    我们需要同时表示物体旋转的角速度和旋转方向。

5.  To do this, rotation in three dimensions Is typically described using a single vector.
    为了实现这个，三维旋转通常用一个单一的向量来描述。

6.  The magnitude of the vector indicates the angular speed, and the direction is determined by a super-important convention called the "right-hand rule".
    向量的大小表示角速度，方向由一个超级重要的约定确定，称为"右手规则"

7.  Rotation in three dimensions is described with a single vector.
    三维旋转用一个单一的向量描述。

8.  Right hand rule to determine the direction of a rotation vector.
    右手规则用来确定旋转向量的方向。

9.  Or just a thumbs up.
    或者简单的说，就是竖起大拇指。

10. RIGHT-HAND RULE: Curl the fingers of your right hand in the direction of rotation, and stick out your thumb.
    右手规则：将你的右手的手指卷在旋转的方向上，并伸出大拇指。

11. The vector representing this three-dimensional rotation is, by definition, oriented in the direction of your thumb.
    代表这个三维旋转的向量，按定义，是朝着你的大拇指的方向。

12. Your thumb should point along the axis of rotation.
    你的大拇指应该指向旋转轴。

13. Adopting the convention of using the right hand instead of the left lets us encode the difference between a certain three-dimensional rotation, and the reverse rotation.
    采用使用右手而非左手的约定让我们可以编码一个特定的三维旋转和反向旋转之间的差异。

1. Basically, it extends the idea of clockwise vs. counterclockwise into three dimensions.
    基本上，它将顺时针和逆时针的概念扩展到三个维度。

2.  For example, the rotation of the earth in space would be described using a vector pointing from the center of the earth to its north pole, whose length is equal to the angular speed of the earth's rotation (which happens to be 0.0000729 radians/second).
    例如，地球在空间中的旋转可以用一个从地球中心指向北极的向量来描述，这个向量的长度等于地球旋转的角速度（恰好是0.0000729弧度/秒）。


--- pic\Curl, fluid rotation in three dimensions.pdf_02.png ---

1. Two-dimensional fluid rotation revisited
    再访二维流体旋转

2. In the curl warmup article, I introduce how fluid flows along a two-dimensional vector field defined by the function $v(x,y)$.
    在旋度预热文章中，我介绍了流体如何沿着由函数$v(x,y)$定义的二维向量场流动。

3. The following animation gives a simulation of this, where fluid particles (drawn as blue dots) always move in the direction of the vector they are closest to. 
    下面的动画给出了这个的模拟，其中流体粒子（以蓝色点绘制）总是朝着它们最接近的向量的方向移动。

4. For the purposes of studying curl, notice what happens in and around the circled regions.
    为了研究旋度，注意圈出区域内外发生了什么。

5. The fluid rotates counterclockwise in the left and right circles, and clockwise in the top and bottom circles. 
    流体在左圈和右圈中逆时针旋转，在顶部和底部的圈中顺时针旋转。

6. In studying curl, the key question is this: How much does the fluid rotate around each specific point $(x_0, y_0)$ in the plane? 
    在研究旋度时，关键问题是：流体在平面上每个特定点$(x_0, y_0)$周围旋转多少？

7. In the last article, I gave an intuition for how the answer to this question is what you might call the 2d-curl of v, which has the following formula: 
    在上一篇文章中，我给出了对于这个问题的答案可能是你所说的v的2d旋度的直观理解，该公式为：

1. Here, $v_1$ and $v_2$ are the components of the vector-valued function $\mathbf{v}$.
   在这里，$v_1$ 和 $v_2$ 是向量值函数 $\mathbf{v}$ 的组成部分。

--- pic\Curl, fluid rotation in three dimensions.pdf_03.png ---

1. For example, with specific vector field given above, defined by $(y^3 - 9y)\mathbf{i} + (x^3 - 9x)\mathbf{j}$, this answer would be
例如，对于上面给出的特定向量场，由$(y^3 - 9y)\mathbf{i} + (x^3 - 9x)\mathbf{j}$定义，这个答案将是

1. Notice, the result is a scalar-valued function. 
    注意，结果是一个标量值函数。

2. You plug in a point, like (2,1), and you get out a single number which indicates angular velocity of the fluid near your point, $3(2)^2 - 3(1)^2 = 12 - 3 = 9$ 
    你插入一个点，比如(2,1)，你得到一个单一的数字，这个数字表示流体在你的点附近的角速度，$3(2)^2 - 3(1)^2 = 12 - 3 = 9$

3. As it turns out this number represents twice the angular speed of the fluid near the point, so the speed of rotation is 4.5 radians/second (more on this later).
事实证明，这个数字表示的是流体在点附近的角速度的两倍，所以旋转的速度是每秒4.5弧度（稍后会有更多解释）。

1. Reflection question: In the fluid flow animated above, does the fluid have a rotational component at the origin (0, 0)? Choose 1 answer:
    反思问题：在上面的流体流动动画中，流体在原点（0,0）有旋转分量吗？选择一个答案：

3. The important point that you get a single scalar describing the rotation.
你得到了一个描述旋转的单一标量，这是重要的一点。

1. Evaluating the formula $3x^2 - 3y^2$ found above at the point $(x, y) = (0, 0)$, we get $3(0)^2 - 3(0)^2 = 0$.
评估上述公式$3x^2 - 3y^2$在点$(x, y) = (0, 0)$处的值，我们得到$3(0)^2 - 3(0)^2 = 0$。

1. This means there is no fluid rotation around this point. 
   这意味着这个点周围没有流体旋转。

2. This should make sense because the rotation of a single object in two dimensions can be described with a single number (or scalar), so rotation around all possible points in a flowing fluid should be described with a scalar-valued function.
这是有道理的，因为在二维中，单个物体的旋转可以用一个数字（或标量）来描述，所以在流动的流体中所有可能的点周围的旋转应该用一个标量值函数来描述。

1. Reflection question: In the fluid flow animated above, does the fluid have a rotational component at the origin (0, 0)?
反思问题：在上面动画显示的流体流动中，原点（0,0）处的流体是否有旋转分量？

1. This should feel consistent with the animation above. 
    这应该与上面的动画一致。

2. Around the origin, fluid particles flow in from the upper right and lower left, and flow out towards the upper left and lower right, but there is no noticeable rotation in how they do this.
    在原点周围，流体粒子从右上方和左下方流入，然后向左上方和右下方流出，但在这个过程中没有明显的旋转。


--- pic\Curl, fluid rotation in three dimensions.pdf_04.png ---

1. Moving to three dimensions
    进入三维

2. In preparation for moving to three dimensions, let's express the fluid rotation above using vectors. 
    为了准备进入三维，让我们使用向量来表达上面的流体旋转。

3. Focus on a region of counterclockwise rotation, such as the right-most circle in the animation above.
    关注一个逆时针旋转的区域，比如上面动画中最右边的圈。

7. Imagine wrapping the fingers of your right hand around this circle, so they point in the direction of the arrows (counterclockwise in this case), and stick out your thumb. 
想象一下，你的右手的手指围绕这个圆，指向箭头的方向（在这种情况下是逆时针），并伸出你的拇指。

8. Your thumb should be pointing out of the page, in the positive z-direction, parallel to the unit vector k.
你的拇指应该指向页面外，沿着正z方向，平行于单位向量k。

9. Vector indicating rotation of fluid flow within right circle of the animation above.
向量表示上面动画中右圆内的流体流动的旋转。

10. If we did this at evexy point, assigning a vector to the rotation around each point on the x y-plane according to the formula $2d-\text{curl} \ \mathbf{v}(x, y) = 3x^2 - 3y^2$, you would end up with something like this:
如果我们在每个点都这样做，根据公式$2d-\text{curl} \ \mathbf{v}(x, y) = 3x^2 - 3y^2$，为xy平面上每个点周围的旋转分配一个向量，你会得到类似这样的结果：

4. Vectors pointing in the positive z-direction indicate counterclockwise rotation near that point, and vectors pointing the other way indicate clockwise rotation, as viewed from above the $xy$-plane. 
    指向正z方向的向量表示该点附近的逆时针旋转，向另一方向指的向量表示顺时针旋转，从zy平面上方看。

11. The length of each vector indicates the speed of that rotation. 
每个向量的长度表示旋转的速度。

12. You could describe this system of vectors with the expression $(3x^2 - 3y^2)\mathbf{k}$.
你可以用表达式$(3x^2 - 3y^2)\mathbf{k}$来描述这个向量系统。

5. This is almost a three-dimensional vector field, except that we are only looking at points on the xy-plane, not in all of space.
    这几乎是一个三维向量场，只不过我们只看xy平面上的点，而不是全空间的点。

--- pic\Curl, fluid rotation in three dimensions.pdf_05.png ---

1. Curl itself only applies to three-dimensional vector fields, so to properly set the stage for the material below, let's make this a fully three-dimensional example.
旋度本身只适用于三维向量场，所以为了正确地为下面的材料做准备，让我们把这个例子完全变成三维的。

1. To start, we extend our original vector-valued function v to a similar three-dimensional function $\mathbf{v}_{3d}$. 
    首先，我们将原始的向量值函数v扩展到一个类似的三维函数$\mathbf{v}_{3d}$。

14. As three-dimensional vector fields go, this still feels vexy flat, doesn't it?
对于三维向量场来说，这仍然感觉非常平坦，不是吗？

15. The k component is 0 evexywhere, and none of the components depend on the z input variable at all.
k分量在所有地方都是0，而且没有任何分量依赖于z输入变量。

3. We have basically just copied the original two-dimensional vector field onto evexy slice of three-dimensional space parallel to the $xy$-plane. 
    我们基本上只是将原始的二维向量场复制到了与$xy$平面平行的三维空间的每一层。

4. The next video shows what that vector field $v_{3d}$ looks like, where we keep the flat $xy$-plane (drawn in grey) and red circles as reference points. 
    下一个视频显示了向量场$v_{3d}$的样子，我们保留了平面$xy$平面（以灰色画出）和红圈作为参考点。

5. Notice that at each layer parallel to the $xy$-plane, the vectors are identical to the original vectors we had sitting in the $xy$-plane from the purely 2d vector field v in the previous section. 
    注意，在与$xy$平面平行的每一层，向量与我们在上一节的纯二维向量场v中在$xy$平面上的原始向量相同。

6. Treating 2d vector field as 3d vector field
    将2d向量场视为3d向量场。

7. Again, imagine this vector field as representing a fluid flow, like air in a room or water in a pool.
    再次想象这个向量场表示的是一种流体流动，就像房间里的空气或者池塘里的水一样。

16. When we represent the rotation of this fluid around each point with a vector attached to that point, we get a new vector field, as shown in the next video:
当我们用附着在每个点上的向量来表示这种流体围绕每个点的旋转时，我们得到了一个新的向量场，如下一个视频所示：

--- pic\Curl, fluid rotation in three dimensions.pdf_06.png ---

1. This is given by the vector-valued function $w$(x, y, z)$ = (0)i + (0)j + (3x^2 - 3y^2)k$.
   这由向量值函数$w$(x, y, z)$ = (0)i + (0)j + (3x^2 - 3y^2)k$给出。

1. This is the same formula that we had before, $(3x^2 - 3y^2)k$, but the important point is that now we apply it to all points $$(x, y, z)$$ in space, not just the points $(x, y)$ in the xy-plane.
这是我们之前的公式$(3x^2 - 3y^2)k$，但重要的是，现在我们将它应用到空间中的所有点$$(x, y, z)$$，而不仅仅是xy平面上的点$(x, y)$。

3. The fact that the z-input does not influence the output reflects the fact that our fluid motion Is the same in all slices of space parallel to the $xy$-plane.
   z输入不影响输出反映出我们的流体运动在与$xy$平面平行的所有空间切片中都是相同的。

4. The fact that the i and j components are 0 means all rotation vectors point purely in the z-direction, meaning all actual fluid rotation is parallel to the $xy$-plane.
   i和j分量为0意味着所有旋转向量纯粹指向z方向，也就是说所有实际的流体旋转都平行于$xy$平面。

5. This new (blue) vector field w is called the "curl" of the initial (green) vector field $v_{3d}$.
   这个新的（蓝色）向量场w被称为初始（绿色）向量场$v_{3d}$的"旋度"。

6. One way you might see this written is $w = \text{curl} v_{3d}$.
   你可能会看到这样写的一种方式是$w =\text{curl} v_{3d}$。

7. This is our first example of honest-to-goodness three-dimensional curl: Curl, as a mathematical operator, takes in a three-dimensional vector-valued function $v_{3d}$, thought of as representing a fluid flow, and outputs another three-dimensional vector-valued function "curl $v_{3d}$," which represents the rotation near each point of that fluid.
   这是我们真正的第一个三维旋度的例子：旋度作为一种数学运算符，输入一个三维向量值函数$v_{3d}$，这被认为代表了流体流动，并输出另一个三维向量值函数"旋度$v_{3d}$"，这表示了流体在每个点附近的旋转。

18. Visualizing fluid rotation in three dimensions
在三维中可视化流体旋转

--- pic\Curl, fluid rotation in three dimensions.pdf_07.png ---

1. For a general fluid flow in three dimensions, the rotation may not always be purely parallel to the $xy$-plane.
   对于三维中的一般流体流动，旋转可能并不总是纯粹平行于$xy$-plane。

10. This can make it hard to picture what's going on. Really hard.
    这可能使得想象正在发生的事情变得困难。真的很困难。

11. For instance, imagine that the air around you is blowing and swirling in some chaotic motion.
    例如，想象你周围的空气在以某种混乱的运动吹动和旋转。

12. Now pick some specific point $(x_0, y_0, z_0)$ in space.
    现在在空间中选择一个特定的点$(x_0, y_0, z_0)$。

13. How can you think about what "air rotation near that point" means? Here are a couple of tactics:
    你怎么理解"在该点附近的空气旋转"是什么意思？这里有一些策略：

19. Here are a couple of tactics:
这里有几种策略：

14. Imagine there is a tiny tennis ball whose center is fixed to the point $(x_0, y_0, z_0)$; but which is free to rotate.
    想象有一个小网球，其中心固定在点$(x_0, y_0, z_0)$；但它可以自由旋转。

15. Perhaps you have invented magic to hold it there, or otherwise have some sort of ingenious magnetic suspension device.
    也许你已经发明了魔法来固定它在那里，或者有一些巧妙的磁悬浮设备。

16. The air blowing around it may cause it to spin in some way or another.
    空气的吹动可能会使它以某种方式旋转。

17. The curl vector attached to that point will be the vector describing this tiny tennis ball's rotation, in the same way, we described the earth's rotation using a single vector above.
    附着在那个点的旋度向量将是描述这个小网球旋转的向量，就像我们上面使用单一向量描述地球旋转的方式一样。

18. Alternatively, take an archer's arrow with nice thick feathers.
    或者，取一只弓箭手的箭，箭尾有着粗大的羽毛。

19. The kind you might imagine Robin Hood shooting.
    你可能会想象罗宾汉射出的那种。

20. Situate the arrow in midair such that its feathers are at the point $(x_0, y_0, z_0)$.
    将箭放在半空中，使其羽毛位于点$(x_0, y_0, z_0)$。

21. Again, you've invented magic and finagle a way so that the base of the arrow is fixed to this point, but you are free to orient the arrow in any direction you want, and it freely rotates based on how the wind blows its feathers.
 再次，你已经发明了魔法并找到了一种方法使箭的基部固定在这个点，但是你可以自由地将箭定向到你想要的任何方向，并且它根据风吹动其羽毛的方式自由旋转。

22. Find the orientation which maximizes the rotation of the arrow.
    找到最大化箭旋转的方向。

23. If you experiment with various orientations for the arrow and find the one direction in which the air currents cause the arrow to rotate the fastest, this is the direction of the curl vector at the point $(x_0, y_0, z_0)$.
    如果你对箭的各种方向进行试验，并找到一种方向，使得空气流动使箭最快旋转，那么这就是在点$(x_0, y_0, z_0)$的旋度向量的方向。

24. This is somewhat analogous to how the gradient points in the "direction of steepest ascent"; the curl points in the "direction of greatest rotation".
    这有点类似于梯度指向"最陡峭上升的方向"；旋度指向"最大旋转的方向"。

--- pic\Curl, fluid rotation in three dimensions.pdf_08.png ---

1. Curl is a limiting operation
    旋度是一个极限运算

2. Technically, all the descriptions above describe fluid flow in a region.
    严格来说，上面所有的描述都在描述一个区域内的流体流动。

3. The circled regions of the animation, the region occupied by the tiny tennis ball, the region spanned by the feathers of the arrow, etc.
    动画中的圆形区域，被小网球占据的区域，被箭头的羽毛覆盖的区域等等。

4. None of these are literally rotation at just one point.
    这些都不是真正的在某一点处的旋转。

5. In fact, the idea of "rotation at a point" is kind of ridiculous, isn't it?
    实际上，“在一点处旋转”的概念是有些荒谬的，不是吗？

6. It only ever makes sense to talk about the rotation of a fluid around a point.
    我们只能谈论流体围绕某一点的旋转。

7. Nevertheless, the curl of a vector field, as a mathematical operation, takes in just one point as its input, not a region, so what does it really mean.
    然而，作为一种数学运算，向量场的旋度只把一个点作为输入，而不是一个区域，那么它的真正含义是什么呢。

8. As with all differential operators, the formal definition of a curl involves a limiting process.
    就像所有的微分运算符一样，旋度的正式定义涉及到一个极限过程。

9. You can think of it as taking the limit of rotation in smaller and smaller regions which all surround a given point.
    你可以把它理解为在越来越小的区域内取旋转的极限，这些区域都围绕着一个给定的点。

10. For example, imagine the tennis ball above is shrinking.
    例如，想象上面的网球正在缩小。

11. If you are hungxy for a formal definition, I wrote about the formal definition of curl later on, once line integrals are covered.
    如果你想了解正式的定义，我在后面讲到线积分时，写了关于旋度的正式定义。

20. Consider smaller and smaller regions around the relevant point
考虑到相关点周围越来越小的区域

12. Just keep in mind that all descriptions using animations, images of small rotating balls, or anything of this sort, are necessarily approximations of what true curl is measuring.
    请记住，所有使用动画、小旋转球的图片或者任何这类的描述，都必然是真正的旋度所测量的近似值。

13. Notation and formula for curl
    旋度的符号和公式

14. Let's write v as a general vector-valued function, with three inputs $(x, y, z)$ and a three-coordinate output.
    我们把v写作一个一般的向量值函数，有三个输入$(x, y, z)$和一个三坐标的输出。

15. We will write this three-coordinate output in terms of three scalar valued functions: $v_1(x, y, z)$, $v_2(x, y, z)$, and $v_3(x, y, z)$.
    我们会用三个标量值函数：$v_1(x, y, z)$，$v_2(x, y, z)$和$v_3(x, y, z)$来表示这个三坐标的输出。

21. The notation for curl uses the same symbol "∇" used in the expressions for gradient and divergence, and once again we think of it as representing a vector of partial derivative operators:
旋度的符号使用的是梯度和散度表达式中使用的相同的符号"∇"，我们再次将它视为表示偏导数运算符的向量：

--- pic\Curl, fluid rotation in three dimensions.pdf_09.png ---

1. The curl is thought of as the cross product of this "vector" and the function v, computed using the determinant as usual:
旋度被认为是这个"向量"和函数v的叉积，通常使用行列式来计算：

--- pic\Curl, fluid rotation in three dimensions.pdf_10.png ---

1. THAT'S A DETERMINANT OF VECTORS, OPERATORS AND FUNCTIONS... CAN YOU EVEN DO THAT?
这是向量、运算符和函数的行列式...你真的能做到吗？

18. I Know what you're thinking: "That's the funkiest determinant I've ever seen."
    我知道你在想什么：“那是我见过的最奇怪的行列式。”

19. None of the elements are even numbers!
    元素中甚至没有一个是数字！

20. One row has vectors, one has operators, and one has functions.
    一行是向量，一行是操作符，一行是函数。

21. Can you even do that?
    你能做到吗？

22. It's a bit weird, sure, but it works as a notational trick if nothing else.
    确实有点奇怪，但如果没有别的，它至少可以作为一个符号技巧。

我明白了，我会在可能是数学公式的地方替换成LaTeX公式。以下是按照您的要求修改后的输出：

1. When you "multiply" an operator like $\frac{\partial}{\partial x}$ with a function like $v_2$, you're not really multiplying, but applying the operator to get a new function, $\frac{\partial v_2}{\partial x}$.
当你将像$\frac{\partial}{\partial x}$这样的运算符与像$v_2$这样的函数"相乘"时，你并不是真的在相乘，而是在应用运算符得到一个新的函数，$\frac{\partial v_2}{\partial x}$。

2. Similarly, multiplying a vector like with a function like $\frac{\partial v_2}{\partial x}$ gives a vector-valued function $\frac{\partial v_2}{\partial x}k$.
同样，将像这样的向量与像$\frac{\partial v_2}{\partial x}$这样的函数相乘，得到一个向量值函数$\frac{\partial v_2}{\partial x}k$。 

1.  The final expression for the determinant is the sum of 6 vector-valued functions like this one.
    这个行列式的最终表达式是6个像这样的向量值函数的和。

1. Intuition for the formula
对公式的直觉理解

2. Let's take a close look at this final result:
让我们仔细看看这个最终结果：

--- pic\Curl, fluid rotation in three dimensions.pdf_11.png ---

1. Notice, each component is like its own version of 2d-curl operator we found in the curl warm up article.
    注意，每个分量都像是我们在旋度预热文章中找到的2d-curl运算符的自己的版本。

27. In fact, the k component has precisely the same formula as the 2d-curl.
    实际上，k分量的公式与2d-curl的公式完全相同。

28. This should make sense because the k-component of curl should measure the component of fluid rotation which is parallel to the xy-plane.
    这应该是有意义的，因为旋度的k分量应该测量与xy平面平行的流体旋转的分量。

29. Likewise, the i and j components measure the component of the fluid rotation parallel to the yz and xz planes respectively.
    同样，i和j分量分别测量与yz平面和xz平面平行的流体旋转的分量。

30. One little nuance I should point out is that when you evaluate the curl near a point to get a vector (thought of as a rotation vector), the magnitude of that vector does not equal the angular speed of the imagined fluid near that point.
    我应该指出的一个小细节是，当你在一个点附近计算旋度得到一个向量（被认为是旋转向量）时，该向量的大小并不等于假想流体在该点附近的角速度。

31. Instead the magnitude is equal to twice the angular speed of the fluid.
    相反，大小等于流体角速度的两倍。

32. In short, this is because there are two terms in each component, which should be averaged and not summed.
    简单来说，这是因为每个分量中有两个项，应该取平均而不是求和。

33. Let's look at 2d-curl evaluated at some point $(x_0, y_0)$, since each of the components of curl are of this form.
    让我们看一下在某点$(x_0, y_0)$处评估的2d-curl，因为旋度的每个分量都是这种形式。

34. You may recall the intuition for this formula given in the 2d-curl article:
    你可能记得在2d-curl文章中给出的这个公式的直观理解：

35. The term $\frac{\partial v_2}{\partial x} (x_0, y_0)$ gives the angular speed of particles to the left and right of $(x_0, y_0)$.
    项$\frac{\partial v_2}{\partial x} (x_0, y_0)$给出了粒子在$(x_0, y_0)$左右的角速度。

36. The term $-\frac{\partial v_1}{\partial y}(x_0, y_0)$ gives the angular speed of particles above and below $(x_0, y_0)$.
    项$-\frac{\partial v_1}{\partial y}(x_0, y_0)$给出了粒子在$(x_0, y_0)$上下的角速度。

1. What we really mean by "total rotation around $(x_0, y_0)$" is the average angular speed of all particles around $(x_0, y_0)$, so we should really be averaging the influences of these two directions, not summing them.
我们所说的"围绕$(x_0, y_0)$的总旋转"实际上是指围绕$(x_0, y_0)$的所有粒子的平均角速度，所以我们实际上应该是平均这两个方向的影响，而不是求和。


--- pic\Curl, fluid rotation in three dimensions.pdf_12.png ---
1. For example, think of a wheel rotating at 3 radians per second. 
    例如，想象一个轮子以每秒3弧度的速度旋转。

2. The points on the left and right sides of the rim could be described as having angular speeds of 3 radians per second each, relative to the center of the wheel. 
    轮辋的左右两边的点可以被描述为相对于轮子中心每秒有3弧度的角速度。

3. Likewise points on the top and bottom of the rim have angular speeds of 3 radians per second, relative to the center of the wheel.
    同样，轮辋的上下两边的点相对于轮子中心每秒有3弧度的角速度。

4. But this does not mean the total rotation of the wheel suddenly becomes 6 radians per second. The rotation as a whole is still 3 radians per second. 
    但这并不意味着车轮的总旋转突然变为每秒6弧度。作为一个整体，旋转仍然是每秒3弧度。

5. Rotating fluids are a bit more flimsy than a rigid wheel, so the angular speeds of particles above and below a point $(x_0, y_0)$ may not equal the angular speeds of particles to the left and right of $(x_0, y_0)$.
    旋转的流体比刚性的轮子稍微松散一些，所以在点$(x_0, y_0)$上方和下方的粒子的角速度可能不等于点$(x_0, y_0)$左右的粒子的角速度。

6. Still, though, adding these two speeds is not the right way to measure "total rotation", averaging is. 
    尽管如此，将这两个速度相加并不是衡量“总旋转”的正确方式，平均值才是。

7. Example: Finding rotation in a three-dimensional vector field using curl
    示例：使用旋度在三维向量场中找到旋转

8. Problem: Suppose a fluid flows in three dimensions according to the following vector field
    问题：假设一个流体按照下面的向量场在三维中流动

9. Describe the rotation of the fluid near the point $(0, 1, 2)$
    描述靠近点$(0, 1, 2)$的流体的旋转

10. Step 1: Evaluate curl (you may want some paper for this one).
    步骤1：计算旋度（你可能需要一些纸来做这个）

--- pic\Curl, fluid rotation in three dimensions.pdf_13.png ---

1. First, we find the curl of this function. Personally, I can never remember the final formula for curl off the top of my head.
首先，我们找到这个函数的旋度。就我个人而言，我无法凭记忆回忆起旋度的最终公式。

2. I just remember that curl is $\nabla \times \mathbf{v}$, and write out the full cross product, determinant and all, whenever I need to compute curl by hand:
我只记得旋度是$\nabla \times \mathbf{v}$，每当我需要手动计算旋度时，我就写出完整的叉积，包括行列式等所有内容。

The calculation involves the following formula:
这个计算涉及到下面的公式:

$ \nabla \times v = (i, j, k) \begin{vmatrix} \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z} \\ v_x & v_y & v_z \end{vmatrix} $

1.  Let's go through this determinant one component at a time. 
    让我们一次处理这个行列式的一个分量。

2.  The i component is…
    i分量是…

3.  The j component is…
    j分量是…

4.  And the k component is…
    而k分量是…

1. Putting this all together, the curl is
把所有这些放在一起，旋度是

--- pic\Curl, fluid rotation in three dimensions.pdf_14.png ---
1. Step 2: Plug in $(0, 1, 2)$
步骤2：代入$(0, 1, 2)$

1. Step 3: Interpret
步骤3：解释

1. Near the point $(0, 1, 2)$, the fluid rotation is about 8.51 radians per second, with rotation nearly parallel to the $xz$-plane.
在点(0,1,2)附近，流体的旋转大约为每秒8.51弧度，旋转几乎与$xz$平面平行。

1. From the previous question, the rotation of the fluid near $(0, 1, 2)$ is about the axis $-i + 17j$. 
从前面的问题中，我们知道流体在$(0, 1, 2)$附近的旋转大约沿着轴线 $-i + 17j$。

1. Since the angular speed is given by one half the magnitude of curl, the angular speed of our fluid near the point (0,1, 2) is 8.51 radians/second.
由于角速度由旋度的大小的一半给出，因此我们的流体在点(0,1,2)附近的角速度为每秒8.51弧度。

1. Since this vector points predominantly in the j direction, the rotation of the fluid near this point is almost entirely parallel to the xz-plane.
由于这个向量主要指向j方向，所以流体在这一点附近的旋转几乎完全平行于xz平面。

1.  Curl is an operator which takes in a function representing a three-dimensional vector field, and gives another function representing a different three-dimensional vector field.
旋度是一种运算符，它接受一个表示三维向量场的函数，并给出表示另一个不同的三维向量场的函数。

1. If a fluid flows in three-dimensional space along a vector field, the rotation of that fluid around each point, represented as a vector, is given by the curl of the original vector field evaluated at that point.
如果流体在三维空间中沿着一个向量场流动，那么该流体在每个点周围的旋转，表示为一个向量，由在该点评估的原始向量场的旋度给出。

--- pic\Curl, fluid rotation in three dimensions.pdf_15.png ---
11. The curl vector field should be scaled by a half if you want the magnitude of curl vectors to equal the rotational speed of the fluid.
如果你想让旋度向量的大小等于流体的旋转速度，那么旋度向量场应该缩放一半。

12. If a three-dimensional vector-valued function $v(x, y, z)$ has component function $v_1(x, y, z)$, $v_2(x, y, z)$ and $v_3(x, y, z)$, the curl is computed as follows:
如果一个三维向量值函数$v(x, y, z)$有组成函数$v_1(x, y, z)$, $v_2(x, y, z)$和$v_3(x, y, z)$，那么旋度如下计算：

13. Here's an animation of the fluid flow I showed at the vexy start of the article, but this time each dot is treated more accurately like a droplet of water, flexing and twisting based on how the vector field pulls on each individual particle in the droplet.
这是一个我在文章开头就展示的流体流动的动画，但这次每个点都被更精确地处理成一个水滴，根据向量场如何拉动每个水滴中的单个粒子来弯曲和扭曲。

1. I also took away the actual vectors from the vector field so that it's easier to see how the fluid moves.
我还从向量场中去掉了实际的向量，这样更容易看到流体是如何移动的。

14. Hopefully this gives an impression for how complex yet beautiful the fluid-flow conception of vector fields can be.
希望这可以给你留下流体流动的向量场是多么复杂而又美丽的印象。

