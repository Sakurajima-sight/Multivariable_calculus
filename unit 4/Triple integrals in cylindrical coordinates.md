
--- pic\Triple integrals in cylindrical coordinates.pdf_00.png ---

1. Triple integrals in cylindrical coordinates
   三重积分在柱坐标中

2. How to perform a triple integral when your function and bounds are expressed in cylindrical coordinates.
   当你的函数和边界用柱坐标表示时，如何进行三重积分。

3. Background
   背景

4. Triple integrals
   三重积分

5. Double integrals in polar coordinates
   极坐标中的双重积分

6. Cylindrical coordinates are essentially the same as polar coordinates in two-dimensions, just with a $z$-coordinate thrown in to make it three-dimensional.
   柱坐标本质上与二维的极坐标相同，只不过加入了$z$坐标，使其成为三维。

7. Each point in space is described with three coordinates: 
   空间中的每个点都用三个坐标描述：

8. As with any coordinate system, these three numbers give instructions for how to get to a given point starting at the origin.
   与任何坐标系统一样，这三个数字提供了如何从原点开始到达给定点的指示。

9. Start by drawing a line of length $r$ away from the origin, along the $z$-axis.
   从$z$轴上原点开始画一条长度为$r$的线。

No problem! I'll correct the math expressions and replace them with LaTeX equations, following your instructions. Here are the revised sentences:

--- pic\Triple integrals in cylindrical coordinates.pdf_01.png ---

1. Rotate that line by $\theta$ radians on the $xy$-plane, counterclockwise away from the $x$-axis, fixing one end at the origin.
   将该线在 $xy$ 平面上逆时针旋转 $\theta$ 弧度，远离 $x$ 轴，一端固定在原点。

11. From the tip of the line, move a distance $z$ in the third dimension, perpendicular to the $xy$-plane.
从线的尖端，垂直于$xy$平面，在第三维度移动距离$z$。

12. Converting between cylindrical coordinates and cartesian coordinates is the same as converting to polar coordinates in two dimensions.
在柱坐标和笛卡尔坐标之间转换，就像在二维中转换为极坐标一样。


1.  The only new coordinate in three dimensions, $z$, remains unchanged as you convert back and forth.
当你来回转换时，唯一新增的三维坐标，$z$，保持不变。

1.  Note, many authors will use the coordinates $(\rho, \phi, z)$ instead of $(r, \theta, z)$, but I have opted to use $(r, \theta, z)$ to emphasize the connection with polar coordinates.
注意，许多作者会使用坐标$(\rho, \phi, z)$而不是$(r, \theta, z)$，但我选择使用$(r, \theta, z)$来强调与极坐标的联系。

1.  What we're building to
我们正在建立的是

17. The main thing to remember about triple integrals in cylindrical coordinates is that $dV$, representing a tiny bit of volume, is expanded as $dV = r \, d\theta \, dr \, dz$ (Don't forget to include the $r$)
在柱坐标中进行三重积分要记住的主要事情是，表示一点体积的$dV$被展开为$dV = r \, d\theta \, dr \, dz$ （不要忘记包含$r$）

1.  Using cylindrical coordinates can greatly simplify a triple integral when the region you are integrating over has some kind of rotational symmetry about the $z$-axis.
当你要积分的区域在$z$轴周围有某种旋转对称性时，使用柱坐标可以极大地简化三重积分。

1. The one rule
   唯一的规则

1.  When performing double integrals in polar coordinates, the one key thing to remember is how to expand the tiny unit of area $dA$ in terms of $dr$ and $d\theta$.
在极坐标中进行双重积分时，要记住的一件关键事情是如何用$dr$和$d\theta$来扩展微小的面积单位$dA$。

--- pic\Triple integrals in cylindrical coordinates.pdf_02.png ---

1. Note that the variable $r$ is part of this expansion. 
   注意变量$r$是这个展开式的一部分。

2. Expanding the tiny unit of volume $dV$ in a triple integral over cylindrical coordinates is basically the same, except that now we have a $dz$ term. 
   在柱坐标下对三重积分进行的小体积$dV$的展开基本相同，只不过现在我们有一个$dz$项。

3. Remember, the reason this little $r$ shows up for polar coordinates is that a tiny "rectangle" cut by radial and circular lines has side lengths $r d\theta$ and $dr$. 
   记住，这个小$r$出现在极坐标中的原因是，由径向和圆形线条切割的小"矩形"的边长是$r d\theta$和$dr$。

4. The key thing to remember here is that $\theta$ is not a unit of length, so $d\theta$ does not represent a tiny length in the same way that $dr$ and $dz$ do. 
   这里需要记住的关键是，$\theta$不是长度单位，所以$d\theta$并不以$dr$和$dz$相同的方式表示微小的长度。

5. It measures radians, which need to be multiplied by the distance $r$ from the origin to become a length.
   它度量的是弧度，需要乘以源点到$r$的距离才能成为长度。

--- pic\Triple integrals in cylindrical coordinates.pdf_03.png ---

1. Think of your little unit of volume $dV$ as a block with the following properties.
   把你的小单位体积$dV$想象成具有以下性质的一个块。

2. One pair of faces represent constant values of $\theta$.
   一对面代表$\theta$的常数值。

3. One pair of faces represent constant values of $r$ (these will be slightly curved, as if hugging a cylinder).
   一对面代表$r$的常数值（这些面会稍微弯曲，好像在拥抱一个圆柱体）。

4. One pair of faces represent constant values of $z$ (these are the flat top and bottom).
   一对面代表$z$的常数值（这是平的顶部和底部）。

5. When you are integrating over a three-dimensional region $R$, you can think of it as being composed of infinitely many infinitely small blocks like this.
   当你在对一个三维区域$R$进行积分时，你可以把它想象成由无穷多个无穷小的这样的块组成。

6. When they are small enough, the curved edge will basically be a straight line, so you can treat it as a rectangular prism.
   当它们足够小的时候，弯曲的边缘基本上会是一条直线，所以你可以把它当作一个长方体来处理。

7. As the size of the block approaches zero, each edge will represent an infinitesimal change in one variable.
   当块的大小接近零时，每一条边都将代表一个变量的无穷小变化。

8. One edge will have length $dr$, representing a small change in $r$ while $\theta$ and $z$ stay constant.
   一条边的长度将为$dr$，表示在$\theta$和$z$保持不变的情况下，$r$的微小变化。

9. One edge will have length $dz$, representing a small change in $z$ while $r$ and $\theta$ stay constant.
   一条边的长度将为$dz$，表示在$r$和$\theta$保持不变的情况下，$z$的微小变化。

10. Another edge will represent a tiny change in $\theta$ while $r$ and $z$ remain constant.
    另一条边将表示在$r$和$z$保持不变的情况下，$\theta$的微小变化。

11. The length of this edge is not $d\theta$, since $\theta$ is not a unit of length.
    这条边的长度不是$d\theta$，因为$\theta$不是长度单位。

12. Its length is $r d\theta$ where $r$ is the distance from the box to the origin.
    它的长度是$r d\theta$，其中$r$是箱子到原点的距离。

13. In total, the volume of this box is $dV = (r d\theta) (dr) (dz)$.
    总的来说，这个箱子的体积是$dV = (r d\theta) (dr) (dz)$.

1. Example 1: Volume of a sphere
   示例 1：球的体积


--- pic\Triple integrals in cylindrical coordinates.pdf_04.png ---

1. Problem: Find the volume of a sphere with radius 1 using a triple integral in cylindrical coordinates.
   问题：使用柱坐标系中的三重积分找出半径为1的球的体积。

2. First of all, to make our lives easy, let's place the center of the sphere on the origin.
   首先，为了简化问题，让我们将球的中心放在原点。

3. Next, I'll give the sphere a name, $S$, and write the abstract triple integral to find its volume.
   接下来，我将给球体命名为$S$，并写下抽象的三重积分来找出其体积。

4. As always, the hard part is putting bounds on the integral.
   一如既往，积分上下限的确定是困难的部分。

5. However, doing this with cylindrical coordinates is much easier than it would be for cartesian coordinates.   
   然而，使用柱坐标系进行这样的操作要比使用笛卡尔坐标系容易得多。

6. In particular, $r$ and $\theta$ will just live within the unit disc, which is very natural to describe in polar coordinates:
   特别地，$r$和$\theta$将位于单位圆盘内，这在极坐标系中描述非常自然。

--- pic\Triple integrals in cylindrical coordinates.pdf_05.png ---

1. Concept check: Which of the following sets of bounds for $r$ and $\theta$ should we use to integrate over the unit disc?
   概念检查：我们应该使用以下哪一组$r$和$\theta$的范围对单位圆盘进行积分？

2. Choose 1 answer: 
   选择一个答案：

3. The first choice is correct: Within the unit disc, the radius varies between 0 and 1, and the angle $\theta$ runs along its full range from 0 to $2\pi$.
   第一个选择是正确的：在单位圆盘内，半径在0和1之间变化，角度$\theta$的取值范围从0到$2\pi$。


--- pic\Triple integrals in cylindrical coordinates.pdf_06.png ---

1. Since the bounds of $z$ will depend on the value of $r$, we let the innermost integral handle $z$, while the outer two integrals take care of $r$ and $\theta$. 
   由于$z$的界限将取决于$r$的值，我们让最内层的积分处理$z$，而外面两层的积分处理$r$和$\theta$。

2. Writing down what we have so far, we get  
   我们迄今为止得到的结果是 

3. Remember, it's important to make sure the order of the differential terms $dz$, $dr$ and $d\theta$ matches up with the appropriate integral.
   请记住，确保微分项$dz$，$dr$和$d\theta$的顺序与相应的积分相匹配是很重要的。

1. This next question is a little trickier.
这个问题稍微复杂一些。

2. Concept check: For a given value of $r$, which of the following shows the right range of values for $z$?
概念检查：对于给定的$r$值，以下哪个显示了$z$的正确值范围？

3. Choose 1 answer
选择1个答案


1. The first choice Is correct. 
   第一个选项是正确的。

2. In cylindrical coordinates, the distance from a point $(r, \theta, z)$ to the origin is $\sqrt{r^2 + z^2}$.
   在柱面坐标中，点$(r, \theta, z)$到原点的距离是$\sqrt{r^2 + z^2}$。

3. To see why, relate this to cartesian coordinates using the fact that $r^2=x^2 + y^2$     $\sqrt{r^2 + z^2} = \sqrt{x^2 + y^2 + z^2}$.
   为了理解为什么，使用$r^2=x^2 + y^2$  $\sqrt{r^2 + z^2} = \sqrt{x^2 + y^2 + z^2}$这个事实，将其与笛卡尔坐标系进行关联。

1. Therefore, the unit sphere could be defined as all points such that  $r^2 + z^2=1^2$
   因此，单位球可以定义为所有满足 $r^2 + z^2=1^2$ 的点。

--- pic\Triple integrals in cylindrical coordinates.pdf_07.png ---

1. Solving for $z$, we get its upper and lower bounds if it is to remain inside the sphere.
   解出$z$，如果它要保持在球内，我们得到它的上下界。

2. Applying this bound to our innermost integral, we get something that can be worked out.  
   将这个界应用到我们最内层的积分，我们得到可以计算出来的东西。

3. Concept check: Solve this triple integral. 
   概念检查：求解这个三重积分。

4. Integrate with respect to $z$
   关于$z$进行积分

5. Using the inverse chain rule, we can quickly scribble down some notes to see what this antiderivative is:
   使用反链式法则，我们可以快速记下一些笔记来看这个原函数是什么：

1. Antiderivative of $\sqrt{\text{something}}$.
   对 $\sqrt{\text{某物}}$ 的反导数。

2. Divide by $\frac{d}{dr}(1 - r^2)$.
   除以 $\frac{d}{dr}(1 - r^2)$。

--- pic\Triple integrals in cylindrical coordinates.pdf_08.png ---

1. Continuing on with our integral then,
继续我们的积分，


1. And with that, you just found the volume of a unit sphere! 
而且有了这个，你就找到了单位球体的体积！

1. Moreover, this tool is powerful enough to do more than just find the volume of the sphere. 
此外，这个工具的功能强大，不仅能找到球体的体积。

1. For example, you could integrate a three-variable function $f(r, \theta, z)$ inside the sphere,
例如，你可以在球体内部积分一个三变量函数$f(r, \theta, z)$，


1. The hard part of finding the bounds is no different, but the computation of the integrals (done by either you or a computer) will change.
   找到边界的难部分没有不同，但是积分的计算（由你或计算机完成）将会改变。

1. Example 2: Integrating over a pie slice
例2：对饼状切片进行积分

1.  For this example, we will integrate over a region which looks kind of like a Slanted pie slice:
对于这个例子，我们将对一个区域进行积分，这个区域看起来有点像倾斜的饼状切片：


--- pic\Triple integrals in cylindrical coordinates.pdf_09.png ---

1. Wedge shaped region
   楔形区域


2. In a problem, this region might be described to you using the following list of properties:
   在问题中，这个区域可能会使用以下属性列表来描述给你：

3. This time, we will not just be finding the volume of this region.
   这次，我们不仅要找到这个区域的体积。

4. Instead, our task is to integrate the following three-variable function:
   相反，我们的任务是积分以下三变量函数：

5. This might seem out of place in an article about integrating in cylindrical coordinates, since everything here is given in cartesian coordinates.
   这可能在关于在柱坐标系中进行积分的文章中看起来不合适，因为这里的一切都是以笛卡尔坐标给出的。

6. Indeed, you could setup the triple integral using cartesian coordinates if you wanted.
   的确，如果你愿意，你可以使用笛卡尔坐标设置三重积分。

7. However, there's one key fact suggesting that our lives can be made dramatically easier by converting to cylindrical coordinates first:
   但是，有一个关键事实表明，我们的生活可以通过首先转换为柱坐标来大大简化。

2. The expression $x^2 + y^2$ shows up in the function $f$ , as well as in the description of the bounds.
   表达式 $x^2 + y^2$ 出现在函数 $f$ 中，也出现在边界的描述中。

--- pic\Triple integrals in cylindrical coordinates.pdf_10.png ---

1. This suggests some rotational symmetry around the $z$-axis, which cylindrical coordinates are well-suited for.
   这暗示了围绕$z$轴的一些旋转对称性，圆柱坐标非常适合处理这种情况。

1. For example, look at the range for our $x$ and $y$ values:
例如，观察我们的$x$和$y$值的范围：

2. Describing this with a pair of integrals over $dx$ and $dy$ is a real pain.
用一对关于$dx$和$dy$的积分来描述这个真的很麻烦。

3. However, in polar coordinates, this becomes very simple: 
   但是，在极坐标中，这变得非常简单：


4. This means the bounds on the integrals handling $d\theta$ and $dr$ will be constants.
   这意味着处理$d\theta$和$dr$的积分的界限将是常数。

5. You can't do better than that!
   你不能做得比这更好了！
   
2. What about the other criteria, such as 
   那其他的标准呢，比如说


--- pic\Triple integrals in cylindrical coordinates.pdf_11.png ---

1. Since converting to polar coordinates involves the property $\tan(\theta) = \frac{y}{x}$.
   由于转换到极坐标涉及到性质 $\tan(\theta) = \frac{y}{x}$。

2. The bounds on $z$ can be translated to $-0 \leq z \leq \tan(\theta)$.
   $z$ 的界限可以转化为 $-0 \leq z \leq \tan(\theta)$。

3. Putting this together, our triple integral looks like this: 
   把这些放在一起，我们的三重积分看起来像这样：

4. Notice how simple the bounds are.
注意看这些界限是多么的简单。

5. If you are up for a little pain, you can try finding the appropriate triple integral bounds in cartesian coordinates to see just how much uglier they are.
如果你愿意尝试一点困难，你可以试着找出笛卡尔坐标下相应的三重积分界限，看看它们是多么的复杂。

5. We now write the function $f$ using polar coordinates.
   我们现在用极坐标写函数 $f$。

6. And of course, we incorporate the main takeaway of this article, which is how to write $dV$ in polar coordinates: 
   当然，我们要把本文的主要结论融入进来，即如何在极坐标中写出 $dV$：

1. Putting this all together, we get our triple integral in its final solvable state.
   将这些全部放在一起，我们得到了最终可解的三重积分。

2. More practice : Solve this integral
   更多练习：求解此积分。

--- pic\Triple integrals in cylindrical coordinates.pdf_12.png ---

1. Again, in practice, the computation of integrals like this one are taken care of by programs performing numerical integration, or even computer algebra systems. 
   再次，实际上，像这样的积分计算由执行数值积分的程序或甚至计算机代数系统负责。

2. By hand, here's what it looks like: 
   手动计算，看起来像这样：


3. Here, I had to look things up.
这里，我不得不查阅资料。

4. The antiderivative of $\tan^2(\theta)$ is $\tan(\theta) - \theta$.
$\tan^2(\theta)$的原函数是$\tan(\theta) - \theta$。

4. The antiderivative of $\tan(\theta)$ is $- \ln(| \cos(\theta)|)$
   $\tan(\theta)$的原函数是$- \ln(| \cos(\theta)|)$

1. Continuing on our merry way then:
   那么，我们继续愉快地前进：

--- pic\Triple integrals in cylindrical coordinates.pdf_13.png ---

1. Summary
    摘要

2. The main thing to remember about triple integrals in cylindrical coordinates is that $dV$, representing a tiny bit of volume, is expanded as $dV = r d\theta dr dz$.
   关于圆柱坐标下的三重积分，要记住的主要一点是，表示一小部分体积的$dV$，被展开为$dV = r d\theta dr dz$。

3. (Don't forget to include the $r$.)
   （不要忘记包括$r$。）

4. Using cylindrical coordinates can greatly simplify a triple integral when the region you are integrating over has some kind of rotational symmetry about the $z$-axis.
   当你要积分的区域在$z$轴上具有某种旋转对称性时，使用圆柱坐标可以大大简化三重积分。

