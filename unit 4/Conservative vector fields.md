
--- pic\Conservative vector fields.pdf_00.png ---
1. Conservative vector fields
   保守向量场

2. Especially important for physics, conservative vector fields are ones in which integrating along two paths connecting the same two points are equal. 
   特别重要的是，在物理学中，保守向量场是一种沿着连接同两点的两条路径进行积分得到的结果相等的向量场。

3. Fundamental theorem of line integrals, also known as the gradient theorem.
   线积分的基本定理，也被称为梯度定理。

4. What we're building to
   我们正在建立的是

5. At the end of this article, you will see how this paradoxical Escher drawing cuts to the heart of conservative vector fields.
   在本文的结尾，你会看到这个悖论性的Escher图如何深入保守向量场的核心。

6. A vector field $F(x, y)$ is called a conservative vector field if it satisfies any one of the following three properties (all of which are defined within the article): 
   如果一个向量场 $F(x, y)$ 满足以下三个属性中的任何一个（都在文章中定义），则称之为保守向量场：

7. Line integrals of $F$ are path independent.
   $F$ 的线积分与路径无关。

8. Line integrals of $F$ over closed loops are always 0.
   封闭循环上的 $F$ 的线积分总是0。

1. $F$ is the gradient of some scalar-valued function, i.e. $F = \nabla g$ for some function $g$.
$F$ 是某个标量值函数的梯度，即$F = \nabla g$，其中 $g$ 是某个函数。


--- pic\Conservative vector fields.pdf_01.png ---

1. There is also another property equivalent to all these: $F$ is irrotational, meaning its curl is zero everywhere (with a slight caveat).
   还有一个等价于所有这些的性质：$F$ 是无旋的，也就是说它的旋度在任何地方都是零（稍有例外）。

2. However, I'll discuss that in a separate article which defines curl in terms of line integrals.
   然而，我将在另一篇定义了旋度的文章中讨论这个问题。

3. The key takeaway here is not just the definition of a conservative vector field, but the surprising fact that the seemingly different conditions listed above are equivalent to each other.
   这里的关键不仅仅是保守向量场的定义，而且令人惊讶的是，上述看似不同的条件实际上是等价的。

4. Madness!
   疯狂！

5. Path independence
   路径独立性

6. Imagine you have any ol' off-the-shelf vector field $F(x, y)$, and you consider the line integrals of $F$ of two separate paths, $C_1$ and $C_2$, each starting at a point A and ending at a point B.
   想象你有任何一个现成的向量场 $F(x, y)$，并且你考虑两条不同路径 $C_1$ 和 $C_2$ 上 $F$ 的线积分，每条路径都从 A 点开始，到 B 点结束。

7. For almost all vector fields $F$, and almost all choices for the two paths $C_1$ and $C_2$, these integrals will be different.
   对于几乎所有的向量场 $F$，以及几乎所有的两条路径 $C_1$ 和 $C_2$ 的选择，这些积分都会不同。

8. And this makes sense!
   这是有道理的！

9. Each integral is adding up completely different values at completely different points in space.
   每个积分都在空间中的完全不同的点上加起来的完全不同的值。

10. What's surprising is that there exist some vector fields where distinct paths connecting the same two points will always be equal, no matter the choice of paths (of which there are super-infinitely many).
   令人惊讶的是，存在一些向量场，其中连接同两点的不同路径总是相等的，无论路径的选择如何（其中有超级无限多的路径）。

11. In the last article, covering the gradient theorem we saw that in the special case of vector fields which are the gradient of some scalar-valued function, $\nabla f$, this magical property is true.
   在上一篇文章中，我们讨论了梯度定理，我们看到在向量场是某个标量值函数的梯度的特殊情况下，$\nabla f$，这个神奇的属性是真的。

12. The line integrals along distinct paths connecting the same two points A and B will always evaluate to the same thing:
   沿着连接同两点A和B的不同路径的线积分总是会评估为相同的东西：

--- pic\Conservative vector fields.pdf_02.png ---

1. Definition: This property is called path independence.
   定义：这种属性被称为路径无关性。

2. Specifically, a line integral through a vector field $F(x, y)$ is said to be path independent if the value of the integral only depends on the point where the path starts and the point where it ends, not the specific choice of path in between.
   具体来说，如果一个线积分穿过一个矢量场$F(x, y)$，那么如果积分的值只依赖于路径的起点和终点，而不依赖于路径之间的特定选择，那么这个积分就被认为是路径无关的。

3. This is because line integrals against the gradient of $f$ measure the change in the value of $f$.
   这是因为相对于$f$的梯度的线积分测量了$f$的值的变化。

4. Actually, when you properly understand the gradient theorem, this statement isn't totally magical.
   实际上，当你正确理解梯度定理时，这个声明并不完全神奇。

5. This is because line integrals against the gradient of $f$ measure the change in the value of $f$.
   这是因为对$f$的梯度进行线积分可以测量$f$的值的变化。


6. \nabla isualizing this with the graph of $f$, this says that any two paths bringing you from one point to another change your altitude by the same amount.
通过 $f$ 的图形可视化，这意味着任何两条将你从一个点带到另一个点的路径都会使你的高度改变相同的量。

6. Alternate paths in a gradient field.
   在梯度场中的替代路径。

4. The takeaway from this result is that gradient fields are very special vector fields.
   从这个结果可以得出，梯度场是非常特殊的矢量场。

5. Because this property of path independence is so rare, in a sense, "most" vector fields cannot be gradient fields.
   因为路径无关性这个属性非常罕见，从某种意义上说，“大多数”矢量场不能成为梯度场。

4. Path independence implies gradient field.
路径无关性意味着梯度场。

7. Okay, so gradient fields are special due to this path independence property.
   好的，所以由于这个路径无关性质，梯度场是特殊的。

8.  But can you come up with a vector field $F(x, y)$ in which all line integrals are path independent, but which is not the gradient of some scalar-valued function?
    但是，你能否想出一个矢量场$F(x, y)$，在该矢量场中，所有线积分都是路径无关的，但它并不是某个标量值函数的梯度？

9.  I've spoiled the answer with the section title and the introduction: All vector fields in which line integrals are path independent must be the gradient of some function. 
    我已经在章节标题和介绍中透露了答案：所有线积分是路径无关的矢量场都必须是某个函数的梯度。

10. But why? Really, why would this be true?
    但为什么呢？真的，为什么这会是真的？

11. Consider an arbitrary vector field $F(x, y)$ in which line integrals are path independent, meaning $\int_{C1} F \cdot ds = \int_{C2} F \cdot ds$ for all paths $C_1$ and $C_2$ which connect the same two points $A$ and $B$.
考虑一个任意的向量场$F(x, y)$，在该向量场中，线积分是路径无关的，意味着对于所有连接同一两点$A$和$B$的路径$C_1$和$C_2$，都有$\int_{C1} F \cdot ds = \int_{C2} F \cdot ds$。



--- pic\Conservative vector fields.pdf_03.png ---

1. What is it about this property that ensures the existence of some function $g$ such that $\nabla g=F$? 
   是什么性质确保了存在某个函数 $g$，使得 $\nabla g=F$?

2. Challenge question: Can you think of a way to construct such a function $g$ in terms of $F$ using the fact that $F$ is path-independent? 
   挑战问题：你能想到一个方法，用 $F$ 构造这样一个函数 $g$，并利用 $F$ 的路径无关性吗？

4. This is a tricky question, but it might help to look back at the gradient theorem for inspiration.
   这是一个棘手的问题，但回顾梯度定理可能有所启发。

5. I could just spit out the answer here, but it's more fun and enlightening to walk through how you might discover the answer yourself. 
   我可以在这里直接给出答案，但是自己发现答案的过程更有趣，也更有启发性。

6. Getting inspiration from the gradient theorem. 
   从梯度定理中获取灵感。

4. The gradient theorem relates the value of a function to the line integral of its gradient: $\int_{C} \nabla f \cdot \mathbf{ds} = f(B) - f(A)$ where $A$ and $B$ are points in space, and $C$ is some curve connecting them.
梯度定理将函数的值与其梯度的线积分关联起来：$\int_{C} \nabla f \cdot \mathbf{ds} = f(B) - f(A)$，其中$A$和$B$是空间中的点，$C$是连接它们的某条曲线。

9. Suppose it just so happened to be the case that $f(A) = 0$, then this equation would look like $f(B) = \int_{C} \nabla f \cdot \mathbf{ds}$
   假设 $f(A) = 0$，那么这个等式将变成 $f(B) = \int_{C} \nabla f \cdot \mathbf{ds}$

10. In other words, for any point $B$ in space, you could compute $f$ using just its gradient (along with a line integral).
    换句话说，对于空间中的任何一点 $B$，你只需要用它的梯度（再加上线积分）就可以计算出 $f$。

5. Since our goal is to see how the vector field $\mathbf{F}$ can be seen as a gradient, this might spark the idea in your mind to replace $\nabla f$ with $\mathbf{F}$, producing a new scalar value function, which we'll call $g$.
由于我们的目标是看到如何将矢量场$\mathbf{F}$视为梯度，这可能会在你的脑海中引发一个想法，即用$\mathbf{F}$替换$\nabla f$，从而产生一个新的标量值函数，我们将其称为$g$。


--- pic\Conservative vector fields.pdf_04.png ---

1. Usually, we define functions using formulas with respect to the coordinates $(x,y)$ of a point, so this might feel like a wacky definition for $g$.
   我们通常根据点的坐标$(x,y)$定义函数，所以对$g$的这种定义可能感觉很奇怪。

2. To start, $A$ is just some arbitrarily chosen point in space.
   首先，$A$只是空间中任意选择的一个点。

3. Then the value of $g$ at a point $B$ is defined by taking an arbitrary curve connecting $A$ to $B$, and evaluating the line integral of $F$ along this curve.
   然后，点$B$处的$g$值是通过取一个连接$A$到$B$的任意曲线，并沿这条曲线计算$F$的线积分来定义的。

4. This is a very indirect definition, but it is a valid definition nevertheless.
   这是一个非常间接的定义，但它仍然是一个有效的定义。

5. After all, it gives you a way to compute $g(x, y)$ for any point $(x, y)$, doesn't it?
   毕竟，它为你提供了一种计算任意点$(x, y)$处的$g(x, y)$的方法，不是吗？

6. Notice, this definition would not make sense for most vector fields $F$.
   注意，对于大多数矢量场$F$，这个定义是没有意义的。

7. The choice of which path connects $A$ to $B$ would change the value of the integral, leaving the defining value of $g(B)$ ambiguous.
   哪条路径连接$A$和$B$的选择会改变积分的值，使得$g(B)$的定义值模糊不清。

8. However, because line integrals are path independent in $F$, this is a real definition.
   然而，因为$F$中的线积分是路径无关的，所以这是一个真正的定义。

9. Defining $g$ in this way, it turns out that $\nabla g=F$.
   以这种方式定义$g$，结果发现$\nabla g=F$。

10. This should not be too surprising, if you think about what the gradient theorem looks like for $g$.
   如果你考虑一下梯度定理对$g$的描述，这应该不会太让人惊讶。

4. I will not cover the proper proof of this fact here, since I think the details would distract from the main point:
我不会在这里详细证明这个事实，因为我认为细节会分散主要的注意力：

11. Key takeaway: If line integrals are path independent in a vector field $F$, you can use those line integrals to define a function $g$ such that $\nabla g=F$.
   关键要点：如果矢量场$F$中的线积分是路径无关的，你可以使用这些线积分来定义一个函数$g$，使得$\nabla g=F$。


5. Closed loops
封闭的循环

12. Definition: A path is called closed if it starts and ends at the same point. Such paths are also commonly called closed loops.
    定义：如果一条路径的起点和终点是同一点，则称该路径为闭合的。这种路径也常被称为闭环。

13. For example, the path $C$ pictured below starts and ends at $A$.
    例如，下图中的路径$C$起点和终点都在$A$。

14. Where all line integrals are path independent, the line integral of $F$ on any closed loop will be $0$.
   在所有线积分都是路径无关的情况下，$F$在任何闭环上的线积分将为$0$。

15. Why?
   为什么？

--- pic\Conservative vector fields.pdf_05.png ---

1.  Let $C$ be a closed path, starting at $A$ and ending at $A$, and let $\bar{C}$ be the reverse path. 
    让$C$是一个闭合的路径，起点在$A$，终点在$A$，让$\bar{C}$是反向的路径。

2.  That is, $C$ and $\bar{C}$ cover the same points in space, but when you parameterize them you should be walking in opposite directions. 
    也就是说，${C}$和$\bar{C}$覆盖了空间中的同一些点，但当你参数化它们时，你应该走的方向是相反的。

3.  We know that reversing the orientation of a path flips the sign of the line integral: $\int_C F ds = -\int_{\bar{C}} F ds$.
    我们知道，反转路径的方向会改变线积分的符号：$\int_C F ds = -\int_{\bar{C}} F ds$。

4.  This is a general statement about line integrals through a vector field, not specific to conservative vector fields. 
    这是关于通过矢量场的线积分的一般声明，不特指保守矢量场。

5.  However, because $F$ is path independent, and because both $C$ and $\bar{C}$ start at $A$ and end at $A$, it must also be true that $\int_C F ds = \int_{\bar{C}} F ds$.
    然而，因为$F$是路径无关的，且因为$C$和$\bar{C}$都从$A$开始，到$A$结束，所以$\int_C F ds = \int_{\bar{C}} F ds$也必然是真的。

6.  The only way both of these can be true is if the integral equals $0$. 
    这两个都是真的唯一的方式就是积分等于$0$。

7.  You can apply this argument to any closed loop, so the line integral over any closed loop must be $0$. 
    你可以把这个论点应用到任何闭环，所以任何闭环上的线积分必须是$0$。

8. Take any closed path $C$, which starts and ends at the point $A$.
   取任何一个起点和终点都在点$A$的闭路径$C$。

9. Look at what the gradient theorem says about such a path for some scalar-valued function $f$: $\int_{C} \nabla f \cdot ds = f(B) - f(A) = 0$.
   看一看梯度定理对于某个标量值函数$f$的这种路径是怎么说的：$\int_{C} \nabla f \cdot ds = f(B) - f(A) = 0$。

10. Therefore, integrals over closed loops in a gradient field must always be zero. 
    因此，梯度场中闭环上的积分必须始终为零。

11. Since we just saw that vector fields in which line integrals are path independent must also be gradient fields, this answers the question.
    既然我们刚看到，线积分是路径无关的矢量场也必须是梯度场，这就回答了问题。

--- pic\Conservative vector fields.pdf_06.png ---

1. The converse of this fact is also true: If the line integrals of $F$ on all closed loops evaluate to $0$, then all line integrals must be path independent. Why? 
    这个事实的逆也是真的：如果$F$在所有闭环上的线积分都等于$0$，那么所有线积分必须是路径无关的。为什么？

24. Consider a two separate paths $C_1$ and $C_2$, each going from point $A$ to point $B$. 
    考虑两个分开的路径$C_1$和$C_2$，每个都从点$A$到点$B$。

25. Now define a closed loop $C_3$ to be a certain combination of these two paths, where you walk from $A$ to $B$ along $C_1$, then from $B$ to $A$ backwards along $C_2$. 
    现在定义一个闭环$C_3$是这两条路径的某种组合，你沿着$C_1$从$A$走到$B$，然后沿着$C_2$从$B$走回$A$。

26. The line integral of $F$ along this combined path will be $\int_{C_3} F ds = \int_{C_1} F ds - \int_{C_2} F ds$.
    $F$沿着这条组合路径的线积分将是$\int_{C_3} F ds = \int_{C_1} F ds - \int_{C_2} F ds$。

27. The minus sign is because we are going backwards along $C_2$. 
    负号是因为我们沿着$C_2$反向行走。

28. On the other hand, we are assuming that the line integral on all closed loops is $0$, and $C_3$ is a closed loop, so $\int_{C_3} F ds = 0$. 
    另一方面，我们假设所有闭环上的线积分都是$0$，而$C_3$是一个闭环，所以$\int_{C_3} F ds = 0$。

29. Together, these equations imply 
    这些等式联合起来意味着

30. Since $C_1$ and $C_2$ were arbitrarily chosen, this shows that all line integrals in $F$ must be path independent.
    由于$C_1$和$C_2$是任意选择的，这说明$F$中的所有线积分必须是路径无关的。

--- pic\Conservative vector fields.pdf_07.png ---

1. Funky notation for closed-loop integrals.
   闭环积分的奇特记号。

2. You will sometimes see a line integral over a closed loop $C$ written as $\oint_{C} \mathbf{F} \cdot \mathbf{dr}$
   你有时会看到在闭环$C$上的线积分写成
   $\oint_{C} \mathbf{F} \cdot \mathbf{dr}$

3. Don't worry, this is not a new operation that needs to be learned.
   不用担心，这不是需要学习的新操作。

4. It is just a line integral, computed in just the same way as we have done before, but it is meant to emphasize to the reader that $C$ is a closed loop.
   它只是一个线积分，计算方式与我们之前所做的完全相同，但是它是为了强调给读者$C$是一个闭环。

5. Potential energy 势能

1. In the article introducing line integrals through a vector field, I mentioned briefly how in physics, the work done by a force on an object in motion is computed by taking a line integral of the force's vector field along the path of motion.
   在介绍向量场中线积分的文章中，我简要地提到了在物理学中，一个力对一个运动对象所做的功是通过在运动路径上取力的向量场的线积分来计算的。

2. A force is called conservative if the work it does on an object moving from any point $A$ to another point $B$ is always the same, no matter what path is taken.
   如果一个力在任何一个点$A$到另一个点$B$的过程中对一个运动物体所做的功总是相同的，无论走什么路径，那么这个力就被称为保守力。

3. In other words, if this integral is always path-independent.
   换句话说，如果这个积分总是路径无关的。

6. Fundamental forces like gravity and the electric force are conservative, and the quintessential example of a non-conservative force is friction.
基本力量如重力和电力是保守的，而非保守力的典型例子是摩擦力。

4. This has an interesting consequence based on our discussion above: If a force is conservative, it must be the gradient of some function.
   基于我们上面的讨论，这有一个有趣的结果：如果一个力是保守的，那么它必须是某个函数的梯度。

1. Moreover, according to the gradient theorem, the work done on an object by this force as it moves from point A to point B can be computed just by evaluating this function $U$ at each point:
此外，根据梯度定理，当物体从点A移动到点B时，这个力对物体做的功只能通过在每个点评估这个函数$U$来计算。

--- pic\Conservative vector fields.pdf_08.png ---

1. As the physics students among you have likely guessed, this function $U$ is potential energy.
   猜测你们中的物理学生已经猜到，这个函数 $U$ 就是势能。

2. For example, if you take the gradient of gravitational potential or electric potential, you will get the gravitational force or electric force respectively.
   例如，如果你求重力势或电势的梯度，你会分别得到重力或电力。

3. This is why computing the work done by a conservative force can be simplified to comparing potential energies.
   这就是为什么计算保守力所做的工作可以简化为比较势能。

1. Escher
艾舍尔

4. Moving from physics to art, this classic drawing "Ascending and Descending" by M. C. Escher shows what the world would look like if gravity were a non-conservative force.
   从物理转向艺术，M. C. Escher 的这幅经典画作 "上升和下降" 显示了如果重力是非保守力，世界会是什么样子。

1. Closed loop perspective:
闭环视角

5. Imagine walking clockwise on this staircase. With each step gravity would be doing negative work on you.
   想象一下在这个楼梯上顺时针走。每走一步，重力对你都会做负功。

6. So integrating the work along your full circular loop, the total work gravity does on you would be quite negative.
   所以，沿着你的完整的圆形路径积分这个工作，重力对你做的总功将会是相当的负数。

7. However, that's an integral in a closed loop, so the fact that it's nonzero must mean the force acting on you cannot be conservative.
   然而，这是一个在封闭环路中的积分，所以它是非零的事实必须意味着作用在你身上的力不能是保守的。

1. Path independence perspective:
路径独立视角

--- pic\Conservative vector fields.pdf_09.png ---

1. Imagine walking from the tower on the right corner to the left corner.
   想象一下从右角的塔走到左角。

2. If you get there along the clockwise path, gravity does negative work on you.
   如果你顺时针走过去，重力会对你做负功。

3. If you get there along the counterclockwise path, gravity does positive work on you.
   如果你逆时针走过去，重力会对你做正功。

4.  Since both paths start and end at the same point, path independence fails, so the gravity force field cannot be conservative.
    由于两条路径的起点和终点相同，路径无关性失败，所以重力场不能是保守的。

1. Gradient perspective:
   梯度视角：

2. In the real world, gravitational potential corresponds with altitude, because the work done by gravity is proportional to a change in height.
   在现实世界中，重力势对应的是高度，因为重力做的工与高度变化成正比。

3. What makes the Escher drawing striking is that the idea of altitude doesn't make sense.
   使埃舍尔的画令人震撼的是，高度的概念在这里没有意义。

4. Many steps "up" with no steps down can lead you back to the same point.
   许多向“上”走的步骤，没有向下走的步骤，可以把你带回到同一点。

5. This corresponds with the fact that there is no potential function $U$ such that $\nabla U$ give the gravity field.
   这对应于这样一个事实，即不存在潜在函数 $U$，使得 $\nabla U$ 给出重力场。
