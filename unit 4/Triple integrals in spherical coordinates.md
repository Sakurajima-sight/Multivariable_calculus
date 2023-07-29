

--- pic\Triple integrals in spherical coordinates.pdf_00.png ---

1. Triple integrals in spherical coordinates
   球坐标系下的三重积分

2. How to perform a triple integral when your function and bounds are expressed in spherical coordinates.
   当你的函数和边界以球坐标表示时，如何执行三重积分。

3. Background
   背景

4. Triple integrals
   三重积分

5. Spherical coordinates: 
   球坐标：

6. Different authors have different conventions on variable names for spherical coordinates.
   对于球坐标的变量名，不同的作者有不同的约定。

7. For this article, I will use the following convention.
   对于这篇文章，我将使用以下约定。

8. In each description the "radial line" is the line between the point we are giving coordinates to and the origin.
   在每个描述中，“径向线”是我们给出坐标的点与原点之间的线。

9. Specifically, if you project the radial line onto the $xy$-plane, $\theta$ is the angle that line makes with the $x$-axis.
   具体来说，如果你将径向线投影到$xy$平面，$\theta$就是这条线与$x$轴形成的角度。

1. $\phi$ is the angle between the radial line and the $z$-axis.
   $\phi$ 是径线与 $z$ 轴之间的角度。

2. The following two are not strictly required, but they might help as warm up and practice for this topic.
   下面两个不是严格要求的，但它们可能有助于热身和练习这个主题。


--- pic\Triple integrals in spherical coordinates.pdf_01.png ---

1. Double integrals in polar coordinates.
   极坐标下的双重积分。

2. Triple integrals in cylindrical coordinates.
   圆柱坐标下的三重积分。

3. What we're building to.
   我们正在构建的内容。

4. When you are performing a triple integral, if you choose to describe the function and the bounds of your region using spherical coordinates, $(r, \theta, \phi)$, the tiny volume $dV$ should be expanded as follows: 
   当你在执行三重积分时，如果你选择用球坐标$(r, \theta, \phi)$来描述函数和你的区域的界限，那么微小体积$dV$应该按照以下方式展开：

5. The key term to remember (or re-derive) is $r^2 sin(\phi)$.
   需要记住（或重新推导）的关键项是$r^2sin(\phi)$。

6. Converting to spherical coordinates can make triple integrals much easier to work out when the region you are integrating over has some spherical symmetry.
   当你积分的区域具有某种球形对称性时，转换为球坐标可以使三重积分的计算变得更加简单。

1. Dissecting tiny volumes in spherical coordinates
   在球坐标系中切割微小体积

7. As discussed in the introduction to triple integrals, when you are integrating over a three-dimensional region $R$, it helps to imagine breaking it up into infinitely many infinitely small pieces, each with volume $dV$.
   如在三重积分的介绍中所讨论的，当你在对三维区域$R$进行积分时，可以想象将其分解成无限多个无限小的部分，每个部分的体积为$dV$。

8. When you were working in cartesian coordinates, these tiny pieces were thought of as rectangular blocks.
   当你在笛卡尔坐标下工作时，这些微小的部分被视为矩形块。

9. In spherical coordinates, on the other hand, it helps to think of your tiny pieces as being slightly curved blocks "hugging" a sphere.
   另一方面，在球坐标中，可以将你的微小部分想象成轻微弯曲的块，它们"拥抱"着一个球体。

10. I'll be drawing a fairly large version of one of these chunks, partly to exaggerate its curvature, and partly just so we can see it.
    我会画出这些块的一个相当大的版本，部分是为了夸大其曲率，部分只是为了我们能看到它。

11. For example, here's what one looks like in three dimensions.
    例如，这就是它在三维中的样子。

--- pic\Triple integrals in spherical coordinates.pdf_02.png ---

1. The reason for this shape is that each face represents a constant value for one of the spherical coordinates: 
   这种形状的原因是每个面代表球面坐标之一的一个常数值：

2. One pair of faces represents constant values of $r$ (these will be slightly curved, as if hugging a sphere).
   一对面代表 $r$ 的常数值（这些将略微弯曲，仿佛拥抱着一个球体）。

3. One pair of faces represents constant values of $\phi$.
   一对面代表 $\phi$ 的常数值。

4. One pair of faces represents constant values of $\theta$.
   一对面代表 $\theta$ 的常数值。

5. Why is that significant?
为什么这很重要？

6. Because the way multiple integrals work is that each individual integral treats all coordinate as constants, except for one.
因为多重积分的工作方式是，每个单独的积分都把所有的坐标当作常数，除了一个。

6. Therefore, as we consider how the multiple integral as a whole assembles these tiny pieces together, it is more natural to think about pieces whose volume can be expressed in terms of changes to individual coordinates.
   因此，当我们考虑整个多重积分如何将这些微小的部分组合在一起时，更自然地想到的是那些体积可以用对单个坐标的变化来表示的部分。

7. This will become clearer as you read further.
   随着你进一步阅读，这将变得更清楚。

8. As the size of these blocks approaches zero, the curve will become so negligible that we can treat them as rectangular prisms.
   随着这些块的大小接近零，曲线将变得可以忽略不计，我们可以将它们视为长方体。

9.  One edge represents a tiny change in the length in the distance from the origin, $dr$.
    一边代表了从原点开始的长度的微小变化，$dr$。

--- pic\Triple integrals in spherical coordinates.pdf_03.png ---

1. The other two edges are related to the tiny changes in the other two coordinates, $d\theta$ and $d\phi$.
   另外两个边与另外两个坐标的微小变化$d\theta$和$d\phi$有关。

2. However, since $\theta$ and $\phi$ measure radians, not a unit of length, these values must be multiplied by a unit of length in order to properly reflect the lengths of the edges in our rectangular prism.
   然而，由于$\theta$和$\phi$度量的是弧度，而不是长度单位，这些值必须乘以长度单位，以便正确反映我们矩形棱柱边缘的长度。

3. For example, the edge representing a change in $\phi$ has length $r d\phi$.
   例如，表示$\phi$变化的边的长度为$r d\phi$。


--- pic\Triple integrals in spherical coordinates.pdf_04.png ---

1. The edge representing a change in $\theta$ is a little trickier.
   这条表示$\theta$变化的边缘有点复杂。

2. This edge is part of some circle wrapping around the $z$-axis, and the radius of that circle is not $r$, but $r\sin(\phi)$.
   这个边缘是围绕$z$轴包裹的某个圆的一部分，这个圆的半径不是$r$，而是$r\sin(\phi)$。

3. This means the arc length due to a small change in $\theta$ is $r\sin(\phi)d\theta$.
   这意味着由于$\theta$的微小变化而产生的弧长是$r\sin(\phi)d\theta$。

4. That can be confusing at first, so it might be worth a moment of contemplation to ensure you understand how that works.
   刚开始这可能会令人困惑，所以值得花一点时间去思考，以确保你理解其工作原理。

--- pic\Triple integrals in spherical coordinates.pdf_05.png ---

1. Putting all this together, we can express the volume of our "rectangular" block in terms of dr, d$\theta$ and d$\phi$ by taking the product of all its side lengths.
   我们可以将"矩形"块的体积以$dr$、$d\theta$和$d\phi$的形式表示出来，这是通过取所有边长的乘积来实现的。


2. In other words, when you have some triple integral $\iiint_R f dV$, and you choose to express the bounds and the function using spherical coordinates, you cannot just replace dV with $dr d\theta d\phi$.
   换句话说，当你有一个三重积分$\iiint_R f dV$，并且你选择用球坐标来表示界限和函数，你不能只用$dr d\theta d\phi$来替换$dV$。

3. You must also remember the $r^2 \sin\phi$ term.
   你还必须记住$r^2 \sin\phi$项。

4. Personally, I can never quite remember exactly how to expand the dV term off the top of my head.
   个人来说，我总是不能准确地记住如何在脑海中展开$dV$项。

1. "Was it $\sin(\phi)$ or $\sin(\theta)$ ... and is it $r$ or $r$ ...?" 
   "是 $\sin(\phi)$ 还是 $\sin(\theta)$... 是 $r$ 还是 $r$...?"

6. Instead, I think through the process I just illustrated above, asking what the arc lengths resulting from changes to $\phi$ and $\theta$ are.
   相反，我会思考我刚才说明的过程，询问由于$\phi$和$\theta$的变化而产生的弧长是多少。

7. Example 1: Volume of a sphere revisited.
   示例1：再次讨论球体的体积。

8. This might be the simplest possible starting example for triple integration in spherical coordinates, but it let's us compute an interesting non-trivial fact: The volume of a sphere.
   这可能是球坐标三重积分的最简单的起始示例，但它让我们计算出一个有趣的非琐碎的事实：球体的体积。

9.  Question: What is the volume of a sphere with radius $R$?
问题：半径为 $R$ 的球体的体积是多少？

1.  Situate the sphere such that its center is on the origin.
    将球体置于原点，使其中心在原点上。

--- pic\Triple integrals in spherical coordinates.pdf_06.png ---

1. If we were doing this integral in cartesian coordinates, we would have that ugly-but-common situation where the bounds of inner integrals are functions of the outer variables.
   如果我们在笛卡尔坐标系中进行这个积分，我们会遇到那种丑陋但常见的情况，即内部积分的边界是外部变量的函数。

1. However, because spherical coordinates are so well suited to describing, well, actual spheres, our bounds are all constants.
   然而，因为球坐标系非常适合描述，呃，实际的球体，我们的边界都是常数。

2. Concept check: Which of the following sets of bounds on the coordinates $r$, $\theta$, and $\phi$ accurately describes all the points inside a sphere of radius $R$ (without running over the entire sphere multiple times)?
   概念检查：下列哪组坐标$r$，$\theta$和$\phi$的边界准确地描述了半径为$R$的球内的所有点（不会多次覆盖整个球体）？

3. Choose 1 answer:
   选择一个答案：


--- pic\Triple integrals in spherical coordinates.pdf_07.png ---

1. The second answer choice is correct. 
   第二个答案选择是正确的。

2. Although $\theta$ runs around a full circle, which you can think of as lines of latitude, $\phi$ only needs to run from 0 to $\pi$, which you can think of as running from the north pole to the south pole.
   尽管$\theta$围绕着一个完整的圆跑（你可以把它想象成纬线），$\phi$只需要从0跑到$\pi$，你可以把它想象成从北极到南极的跑。

3. If you accidentally let $\phi$ run from 0 to $2\pi$, your integral will run over every point in the sphere twice, and hence evaluate to twice the value that you want.
   如果你不小心让$\phi$从0运行到$2\pi$，你的积分会在球体的每一个点上运行两次，因此评估的值会是你想要的两倍。

4. If you only let $\theta$ run from 0 to $\pi$, you will miss half the sphere.
   如果你只让$\theta$从0运行到$\pi$，你将会错过球体的一半。

2. Using these bounds, together with the fact that $dV$.
   使用这些边界，结合事实 $dV$。


--- pic\Triple integrals in spherical coordinates.pdf_08.png ---

1. we can start setting up our integral like this:
   我们可以开始这样设置我们的积分：

2. Concept check: Work through this integral, and appreciate just how lovely it is compared with the other nasty triple integrals you may have encountered.
   概念检查：理解这个积分，相比于你可能遇到的其他复杂的三重积分，欣赏它是多么的优美。

3.  Next, tackle the $\phi$-integral
    接下来，解决 $\phi$-积分

4.  Finally, solve the $\theta$ integral
    最后，解决 $\theta$ 积分

--- pic\Triple integrals in spherical coordinates.pdf_09.png ---

1. If you dare, imagine trying to do this integral in cartesian coordinates.
   如果你敢，试着想象在笛卡尔坐标系中进行这个积分。

1. It's a nightmare! 
   这真是一场噩梦！

2. This gives us an important takeaway: Key takeaway If you are integrating over a region with some spherical symmetry, passing to spherical coordinates can make the bounds much nicer to deal with. 
   这给我们一个重要的启示：如果你在一个具有某种球形对称性的区域内进行积分，转换到球坐标可以使边界处理得更好。

3. Example 2: Integrating a function
   示例 2：积分一个函数

4. Integrate the function $f(x,y,z) = x+ 2y + 3z$ in the region of the first octant where $x^2+y^2+z^2\leq 3$.
   在第一卦限区域内积分函数$f(x,y,z) = x+ 2y + 3z$，其中$x^2+y^2+z^2\leq 3$。

5. When referring to three-dimensional space, especially in terms of the coordinates $x$, $y$ and $z$, the "octants" are the 8 regions that space Is divided Into when you slice it using the $xy$-plane, the $xz$-plane, and the $yz$-plane.
   当我们在谈论三维空间时，尤其是在使用坐标$x$、$y$和$z$时，"octants"（八分体）是空间被分割成的8个区域，这些区域是在你使用$xy$-平面、$xz$-平面和$yz$-平面切割它时产生的。

6. The "first" octant is the one where $x$, $y$ and $z$ are all positive.
   "第一"八分体是指$x$、$y$和$z$都是正的区域。


--- pic\Triple integrals in spherical coordinates.pdf_10.png ---

1. This is analogous to the "first quadrant" of the $xy$-plane.
   这类似于$xy$平面的"第一象限"。

2. Step 1: Express the region in spherical coordinates. 
   第一步：用球坐标表示区域。

3. How could you know that we should pass to spherical coordinates?
你怎么知道我们应该转到球坐标呢？

4. We could do this whole integral in cartesian coordinates, couldn't we?
我们也可以在笛卡尔坐标中做这个完整的积分，不是吗？

5. Cylindrical coordinates would work too.
柱坐标也可以。

4. The fact that our boundary includes the condition $x^2+y^2+z^2 \leq 3$.
   我们的边界条件包括$x^2+y^2+z^2 \leq 3$。

5. Since the spherical coordinate $r$ expresses precisely this idea, we can feel confident that describing the boundary of our region using $r$ will make the bounds of our three integrals simpler than if we did so in terms of $x$, $y$ and $z$.
   由于球坐标$r$恰好表示了这个概念，我们可以有信心地认为，用$r$描述我们区域的边界，将使我们三个积分的边界比用$x$，$y$ 和$z$更简单。

6. Specifically, this condition becomes $r \leq \sqrt{3}$.
   具体来说，这个条件变成$r \leq \sqrt{3}$。

7. Concept check: What about $\theta$ and $\phi$? 
   概念检查：那$\theta$和$\phi$呢？

1. What bounds should we place on these two coordinates to keep our integral within the first octant?
我们应该对这两个坐标设置什么边界，以保持我们的积分在第一八分体内？


这是我对你提供的段落进行处理的尝试：

--- pic\Triple integrals in spherical coordinates.pdf_11.png ---

1. The correct answer is
   正确答案是

2. You can think of $\theta$ as sweeping out the region $x \geq 0$ and $y \geq 0$ as It ranges from $0$ to $\frac{\pi}{2}$.
   你可以将$\theta$视为在$x \geq 0$和$y \geq 0$的范围内扫掠，范围从$0$到$\frac{\pi}{2}$。

3. Similarly, $\phi$ sweeps out the "top half" of space, the region where $z \geq 0$, as it ranges from $0$ to $\frac{\pi}{2}$.
   同样，$\phi$在$z \geq 0$的区域扫掠"空间的上半部分"，范围从$0$到$\frac{\pi}{2}$。

1. Step $2$: Express the function in spherical coordinates.
步骤$2$：用球坐标表示函数。

4. Next, we convert the function $f(x,y,z) = x+ 2y + 3z$ into spherical coordinates.
   接下来，我们将函数$f(x,y,z) = x+ 2y + 3z$转换为球坐标。

5. To do this, we use the conversions for each individual cartesian coordinate.
   为了做到这一点，我们使用每个独立的笛卡尔坐标的转换。

6. Plugging each of these in, we get 
   将这些插入，我们得到

7. You might say that this makes things more complicated than they were in cartesian coordinates.
   你可能会说，这使得事情比在笛卡尔坐标中更复杂。

8. And you'd be right!
   你是对的！

2. And you'd be right! But when it comes to triple integrals, a more complicated function is a relatively small price to pay for getting our bounds to be constants.
   没错！但是在处理三重积分时，为了让我们的积分界限成为常数，接受一个更复杂的函数是相对较小的代价。

以下是我按照您的要求对段落进行拆分，翻译并添加LaTeX公式的尝试：

--- pic\Triple integrals in spherical coordinates.pdf_12.png ---

1. Step 3: Compute the triple integral.
   第3步：计算三重积分。

2. Concept check: Putting the previous two steps together, what is the integral that we need to solve? 
   概念检查：将前两步结合起来，我们需要解决的积分是什么？

3. Choose 1 answer: 
   选择一个答案：

4. The second answer choice is correct: 
   第二个答案选择是正确的：

5.  To start, this accurately reflects the bounds discussed in step 1:
   开始，这准确地反映了第1步中讨论的边界：

6.  Also, unlike the third choice, this one includes the crucial $r^2sin(\phi)$term.
   另外，不像第三个选择，这个包括关键的 $r^2sin(\phi)$项。

7.  Bring it on home: Solve that integral!
   带它回家：求解那个积分！

8.  Integral from previous question:
    上一题的积分：

这是你请求的段落的处理结果：

--- pic\Triple integrals in spherical coordinates.pdf_13.png ---

1. Remember, for triple integrals that come up in practice, once you know how to express the bounds, it will typically be a computer which takes care of the computation itself.
   记住，对于实践中出现的三重积分，一旦你知道如何表示边界，通常会有计算机负责计算本身。

2. Factor out all non-r terms.
   提取出所有非$r$项。

3. Factor out non-$\theta$ terms appropriately.
   合适地提取出非$\theta$项。

4. (Look up these antiderivatives if necessary)
   (如有必要，查阅这些反导数)

5. Antiderivative of $\sin^2(\phi)$ is $\frac{\phi}{2} - \frac{1}{2} \cos(\phi) \sin(\phi)$.
   $\sin^2(\phi)$的反导数是$\frac{\phi}{2} - \frac{1}{2} \cos(\phi) \sin(\phi)$。

6. Antiderivative of $\cos(\phi) \sin(\phi)$ is $-\frac{1}{2} \cos^2(\phi)$.
   $\cos(\phi) \sin(\phi)$的反导数是$-\frac{1}{2} \cos^2(\phi)$。

7.  Jumping back in where we were and plugging these in, we get:
    回到我们原来的地方，把这些代入，我们得到：

--- pic\Triple integrals in spherical coordinates.pdf_14.png ---

1. Phew! Working through triple integrals is the worst. 
   唉！计算三重积分是最糟糕的。

2. Just remember, the main skill to acquire here is setting up these integrals.
   只需记住，这里要掌握的主要技能是建立这些积分。

3. And the point here is that setting up this integral was much easier using spherical coordinates than It would have been using cartesian coordinates. 
   而这里的重点是，使用球坐标系设置这个积分要比使用笛卡尔坐标系容易得多。

4. When you are performing a triple integral, if you choose to describe the function and the bounds of your region using spherical coordinates, $(r, \phi, \theta)$, the tiny volume $dV$ should be expanded as follows: 
   当你在进行三重积分时，如果你选择用球坐标系$(r, \phi, \theta)$描述你的函数和区域的范围，那么微小体积$dV$应该按照以下方式展开：

5. The key term to remember (or re-derive) is $r^2 \sin(\phi)$.
   要记住（或重新推导）的关键项是 $r^2 \sin(\phi)$。

6. Converting to spherical coordinates can make triple integrals much easier to work out when the region you are integrating over has some spherical symmetry.
   当你要积分的区域具有某种球面对称性时，转换为球坐标系可以使三重积分的计算变得更容易。
