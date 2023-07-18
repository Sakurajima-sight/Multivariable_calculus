   --- pic\Divergence.pdf_00.png ---

1. "Divergence measures the change in density of a fluid flowing according to a given vector field." 
   - 散度测量根据给定向量场流动的流体密度的变化。

2. "Interpret a vector field as representing a fluid flow. The divergence is an operator, which takes in the vector-valued function defining this vector field, and outputs a scalar-valued function measuring the change in density of the fluid at each point."
   - 将向量场解释为表示流体流动。散度是一个运算符，它接收定义此向量场的向量值函数，并输出一个标量值函数，用于测量每个点的流体密度变化。

3. This is the formula for divergence:
   - 这是散度的公式：

4. Here, v1 , v2, … are the component functions of v.
   - 这里，v1，v2，… 是向量v的分量函数。

5. Changing density in fluid flow
	- 改变流体流动的密度

6. Take a look at the following vector field:
	- 看看下面的这个向量场：


--- pic\Divergence.pdf_01.png ---

1. "Notice, this particular drawing of the vector field is color-coded, in the sense you should interpret blue vectors as being shorter, and greenish-yellow vectors as being longer, even though technically they are all drawn with the same length."
   - 注意，这个特定的向量场的绘制是用颜色编码的，你应该将蓝色向量解释为较短，将绿黄色向量解释为较长，尽管技术上它们都绘制成了相同的长度。

2. So that's the picture, but what's the function?
	- 这就是图像，但是函数是什么呢？

2. "The inputs to v are points in two-dimensional space, (x, y), and the outputs are two-dimensional vectors, which in the vector field are attached to the corresponding point (x, y)."
   - v的输入是二维空间中的点（x，y），输出是二维向量，在向量场中，这些向量附着在对应的点（x，y）上。

3. "A nice way to think about vector fields is to imagine the fluid flow they could represent. Specifically, for each point (x, y) in two-dimensional space, imagine a particle sitting at (x, y) flowing in the direction of the vector attached to that point, v(x, y). Moreover, suppose the speed of the particle's movement is determined by the length of that vector."
   - 思考向量场的一个好方法是想象它们可能代表的流体流动。具体来说，对于二维空间中的每个点（x，y），想象一个粒子位于（x，y）处，沿着附着在该点的向量v（x，y）的方向流动。此外，假设粒子的运动速度由该向量的长度决定。

3. The following animation shows what
this might look like for our given function v for just a brief instant: 
   - 以下的动画展示了我们给定的函数v在短暂的瞬间可能的样子：

--- pic\Divergence.pdf_02.png ---

1. "Notice, during this fluid flow, some regions tend to become less dense with dots as particles flow away, such as the upper middle section. On the other hand, down and to the left of that region, particles tend to flow towards each other and the dots get more dense."
   - 注意，在这种流体流动中，一些区域随着粒子的流动，点的密度趋于变小，例如上部中间区域。另一方面，在该区域的下方和左侧，粒子倾向于向彼此流动，点变得更密集。

2. "For a given vector-valued function v(x, y), how can we measure the change in density of particles around a point (x, y) as these particles flow along the vectors given by v(x, y)?"
   - 对于给定的向量值函数v(x, y)，当这些粒子沿着由v(x, y)给出的向量流动时，我们如何测量点(x, y)周围粒子密度的变化？

3.  We can answer this question using a variation of the derivative called divergence.We'll talk more about fluid flow below, but first, let's establish the notation and formula used to express this concept.
   - 我们可以使用一种叫做散度的导数变化来回答这个问题。我们将在下面更深入地讨论流体流动，但首先，让我们建立用来表达这个概念的符号和公式。

4. "The notation for divergence uses the same symbol '$\triangledown$' which you may be familiar with from the gradient. As with the gradient, we think of this symbol loosely as representing a vector of partial derivative symbols."
   - 散度的符号使用的是你可能熟悉的梯度的同一个符号"$\triangledown$"。就像梯度一样，我们把这个符号大致上看作是表示偏导数符号的向量。

--- pic\Divergence.pdf_03.png ---

1. "This is mildly nonsensical since $\triangledown$ isn't really a vector. Its entries are operators, not numbers. Nevertheless, using this dot product notation is super helpful for remembering how to compute divergence."
   - 这有点不合理，因为$\triangledown$实际上并不是一个向量。它的条目是运算符，而不是数字。然而，使用这种点积符号对于记住如何计算散度非常有帮助。

2. just take a look:
   - 只需要看一下：

2. "More generally, the divergence can apply to vector fields of any dimension. This means v can have any number of input variables, as long as its output has the same dimensions. Otherwise, it couldn't represent a vector field."
   - 更一般地，散度可以应用于任何维度的向量场。这意味着v可以有任意数量的输入变量，只要它的输出有相同的维度。否则，它就不能表示一个向量场。

2. If we write v component-wise like this:
   - 如果我们这样按部分写出v：

3. Then the divergence of v looks like this: 
   - 那么，向量v的散度看起来像这样：

4. You could imagine taking the matrix of all possible partial derivatives (we could be fancy and call this the Jacobian), and adding all the diagonal elements:
   - 你可以想象得到所有可能的偏导数的矩阵（我们可以高级一点，称这个为雅可比矩阵），然后加上所有的对角线元素：

--- pic\Divergence.pdf_04.png ---

1. Let's summarize this with a quick diagram:
   - 让我们用一个快速的图表来总结一下：

2. "A useful mnemonic is to imagine taking this dot product. This is the reason for the “$\triangledown$” notation."
   - 一个有用的记忆方法是想象取这个点积。这就是“$\triangledown$”符号的原因。

3. "Let's say you evaluate the divergence of a function v at some point (x0, y0), and it comes out negative. 
   - 假设你在某个点（x0，y0）处评估函数v的散度，结果为负。

4. This means a fluid flowing along the vector field defined by v would tend to become more dense at the point (x0, y0)."
   - 这意味着沿着由v定义的向量场流动的流体在点（x0，y0）处会变得更密集。

5. For example, the following animation shows a vector field with negative divergence at the origin.
   - 例如，下面的动画展示了一个在原点处有负散度的向量场。

6. On the other hand, if the divergence at a point ( x , y ) is positive，
   - 另一方面，如果在点(x, y)处的散度是正数，

--- pic\Divergence.pdf_05.png ---

1. the fluid flowing along the vector field becomes less dense around ($x_0, y_0$) Here's an example:
   - 沿着向量场流动的流体在($x_0, y_0$)附近变得更少密集。这是一个例子：

2. "Finally, the concept of zero-divergence is very important in fluid dynamics and electrodynamics. It indicates that even though a fluid flows freely, its density stays constant. This is particularly handy when modeling incompressible fluids, such as water."
   - 最后，零散度的概念在流体动力学和电动力学中非常重要。它表明，即使流体自由流动，其密度也保持不变。这在建模不可压缩流体（如水）时特别方便。

2. In fact, the very idea that a fluid is incompressible can be tightly communicated with the following equation:
   - 事实上，流体是不可压缩的这个概念可以通过以下方程紧密地表达：

3. "Such vector fields are called "divergence-free"."
   - 这样的向量场被称为"无散度"。

3. Here's an example of what that might look like:
   - 这是它可能的样子：

--- pic\Divergence.pdf_06.png ---

1. Sources and sinks
   - 源和汇

1. "Sometimes, for points with negative divergence, instead of thinking about a fluid getting more dense after a momentary fluid motion, some people imagine the fluid draining at that point while the fluid flows constantly."
   - 有时，对于散度为负的点，一些人会想象流体在那个点排出，而流体则持续流动，而不是想象流体在瞬间流动后变得更密集。

1. Here's what this might look like:
   - 这可能是它的样子：

2. "As such, points of negative divergence are often called "sinks".
   - 因此，负散度的点通常被称为"汇"。

3. Likewise, instead of thinking of points with positive divergence as becoming less dense during a momentary motion, these points might be thought of as "sources" constantly generating more fluid particles."
   - 同样，正散度的点可能被认为是"源"，不断产生更多的流体粒子，而不是在瞬间运动中变得更稀疏。

1. Divergence in higher dimensions
   - 高维度下的散度

--- pic\Divergence.pdf_07.png ---

1. "Although all the diagrams and animations I'm making show the two-dimensional case, you should understand that all these concepts could apply to three or more dimensions as well."
   - 尽管我制作的所有图表和动画都显示了二维情况，但你应该理解所有这些概念也可以应用到三维或更多维度。

2. "Try this as a good mental exercise to test if you understand what divergence represents: Imagine a three-dimensional vector field, and picture what points of positive, negative, and zero divergences might look like."
   - 试试这个很好的思维练习，看看你是否理解散度代表什么：想象一个三维向量场，想象正散度、负散度和零散度的点可能是什么样子。

1. Example 1: Compute and interpret divergence
   - 例1：计算和解释散度

3. "Define a vector field by $\mathbf{v}(x,y) = (x^2 - y^2)\mathbf{i} + 2xy\mathbf{j}$. Compute the divergence, and determine whether the point (1, 2) is more of a source or a sink."
   - 定义一个向量场$\mathbf{v}(x,y) = (x^2 - y^2)\mathbf{i} + 2xy\mathbf{j}$。计算散度，并确定点（1，2）是更多的源还是汇。
   - 更多的源还是汇: 在这个点，向量是主要从这个点发散出去（像源），还是主要向这个点汇聚（像汇）？

--- pic\Divergence.pdf_08.png ---

1. "Step 1: Compute the divergence." 
   - 步骤1：计算散度。

1. We compute divergence by applying the formula. Add the partial derivative with respect to x of the first component to the partial derivative with respect to y to the second component.
   - 我们通过应用公式来计算散度。将第一个部分对x的偏导数加到第二个部分对y的偏导数。

2. "Step 2: Plug in (1, 2)." 
   - 步骤2：代入（1，2）。

1. Evaluating this function at the point ( 1 , 2 ) , we get
   - 在点（1，2）处求这个函数的值，我们得到

3. "Step 3: Interpret. Is the fluid more of a source or a sink at (1, 2)?"
   - 步骤3：解释。在（1，2）处的流体是更多的源还是汇？

--- pic\Divergence.pdf_09.png ---

1. "Because this is positive, the density of a fluid flowing along the vector field given by v(x, y) decreases at the point (1, 2). Therefore, it is more of a source."
   - 因为这是正的，所以沿着由v(x, y)给出的向量场流动的流体在点(1, 2)处的密度会减小。因此，它更像是一个源。

1. Confusing signs
   - 混淆的符号

2. "It always trips me up that positive divergence indicates a negative change in density, and that a negative divergence indicates a positive change in density."
   - 我总是被这个问题绊倒，即正散度表示密度的负变化，而负散度表示密度的正变化。

3. "The sources/sinks interpretation helps a bit, because points of positive divergences are generating more fluid, while points of negative divergence are sucking it away."
   - 源/汇的解释有一点帮助，因为正散度的点正在产生更多的流体，而负散度的点正在吸走流体。

4. Personally, the way I always remember is to think of the case when f is the identity function, taking the point ( x , y ) to the vector $\begin{bmatrix} x \\ y \end{bmatrix}$ .The resulting 
vector field has all vectors pointing away from the origin (can you see why?),and it's relatively quick to compute ∇ ⋅ f .
   - 个人来说，我总是通过考虑f是恒等函数的情况来记住这一点，将点 (x, y) 映射到向量 $\begin{bmatrix} x \\ y \end{bmatrix}$。得到的向量场所有向量都指向原点外（你能理解为什么吗？），并且计算∇ ⋅ f相对来说很快。

5. So each time I return to divergence after not having seen it for a while and think 'hmm, is it positive or negative divergence that indicates a loss in density,' I go through this little exercise and remember, 'Ah yes, that's how it goes, positive divergence indicates an outward flow.'
   - 每次我在一段时间没有接触散度后再回到它，我就会想“嗯，是正散度还是负散度表示密度的减少”，我会做这个小练习并记住，“啊，对了，就是这样，正散度表示向外的流动。”

6. In the next article, I'll give an intuition for why the formula for divergence has anything to do with fluid flow. 
   -在下一篇文章中，我将解释为什么散度的公式与流体流动有关。

7. Later on, once line integrals and surface integrals are covered, I talk about the formal definition of divergence.
   - 稍后，一旦涵盖了线积分和面积分，我将讨论散度的正式定义。
   

--- pic\Divergence.pdf_10.png ---

1. "In the next article, I'll give an intuition for why the formula for divergence has anything to do with fluid flow. Later on, once line integrals and surface integrals are covered, I'll talk about the formal definition of divergence."
   - 在下一篇文章中，我将给出为什么散度公式与流体流动有关的直觉。稍后，一旦涵盖了线积分和面积分，我将讨论散度的正式定义。

2. Summary
Interpret a vector field as representing a fluid flow. 
   - 摘要
   - 将向量场解释为表示流体流动。

3. The divergence Is an operator, which takes in the vector-valued function
defining this vector field, and outputs a scalar-valued function measuring
the change in density of the fluid at each point. 
   - 散度是一个运算符，它接收定义这个向量场的向量值函数，并输出一个标量值函数，用来测量每个点处流体密度的变化。

4. The formula for divergence is div$\mathbf{v}$ where $v_1$, $v_2$, ... are the component functions of $\mathbf{v}$. 
   - 散度的公式是div $\mathbf{v}$，其中$v_1$，$v_2$，...是$\mathbf{v}$的组成函数。

5. Keep in mind, though, divergence is used in all sorts of contexts which can
have nothing to do with fluid. Electrodynamics is a big one, for example. The
fluid flow interpretation is very useful, and gives a much stronger intuition
than a blind use of symbols would, but it should be taken with a grain of salt from time to time.
   - 然而，请记住，散度在各种可能与流体无关的情境中都有用。例如，电动力学就是一个重要的应用领域。流体流动的解释非常有用，比盲目使用符号能提供更强的直观感，但有时也应适当怀疑。











