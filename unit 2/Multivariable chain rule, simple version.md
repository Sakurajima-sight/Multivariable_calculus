以下是从文本中提取的完整句子，按照它们出现的部分进行组织：

--- pic\Multivariable chain rule, simple version.pdf_00.png ---

1. The chain rule for derivatives can be extended to higher dimensions.（导数的链式法则可以推广到更高的维度。）
2. Here we see what that looks like in the relatively simple case where the composition is a single-variable function.（在这里，我们可以看到当复合函数是单变量函数的相对简单情况。）
3. Given a multivariable function f(x, y), and two single variable functions $\mathbf{x}(t)$  and $\mathbf{y}(t)$ , here's what the multivariable chain rule says:（给定一个多变量函数 f(x, y)，以及两个单变量函数 $\mathbf{x}(t)$  和 $\mathbf{y}(t)$ ，下面是多元链式法则的表述：）
4. As you can probably imagine, the multivariable chain rule generalizes the chain rule from single variable calculus.（正如你可能想象的那样，多元链式法则是对单变量微积分的链式法则的推广。）
5. The single variable chain rule tells you how to take the derivative of the composition of two functions.（单变量链式法则告诉你如何对两个函数的复合函数求导。）
6. What if instead of taking in a one-dimensional input, t, the function f took in a two-dimensional input, (x, y)?（如果函数 f 不再接受一维输入 t，而是接受二维输入 (x, y)，会怎样？）

--- pic\Multivariable chain rule, simple version.pdf_01.png ---

1. Well, in that case, it wouldn't make sense to compose it with a scalar-valued function g(t).（在这种情况下，将其与一个标量值函数 g(t) 进行复合就没有意义了。）
2.  Instead, let's say there are two separate scalar-valued functions $\mathbf{x}(t)$  and $\mathbf{y}(t)$ , and we plug these in as the coordinates of f.（相反，假设有两个独立的标量值函数 $\mathbf{x}(t)$  和 $\mathbf{y}(t)$ ，我们将它们作为 f 的坐标输入。）
3. The overall composition will be a single variable function, with a single-number input t, and a single-number output f (a(t), $\mathbf{y}(t)$ ), as shown in this diagram:（总的复合函数将是一个单变量函数，具有单个数字输入 t 和单个数字输出 f(a(t), $\mathbf{y}(t)$ )，如图所示。）
4.  There is still a chain rule that lets you compute the derivative of this new single-variable function f ($\mathbf{x}(t)$ , $\mathbf{y}(t)$ ), and it involves the partial derivatives of f.（仍然存在一个链式法则，可让您计算这个新的单变量函数 f($\mathbf{x}(t)$ , $\mathbf{y}(t)$ ) 的导数，并涉及到 f 的偏导数。）
5.  That is, both are functions of t, but Aa is evaluated via the intermediate functions a(t) and $\mathbf{y}(t)$ .（也就是说，两者都是 t 的函数，但 Aa 是通过中间函数 a(t) 和 $\mathbf{y}(t)$  进行评估的。）

--- pic\Multivariable chain rule, simple version.pdf_02.png ---

1. Rather than thinking of x(t) and $\mathbf{y}(t)$  as being separate functions, it's common to package them together into a single, vector-valued function.（与其将 x(t) 和 $\mathbf{y}(t)$  视为独立的函数，通常将它们合并为一个向量值函数。）
2. Then instead of writing the composition as f($\mathbf{x}(t)$ , $\mathbf{y}(t)$ ), you can write it as f(𝐯(𝑡)).（然后，您可以将复合函数写为 f(𝐯(𝑡))，而不是写为 f($\mathbf{x}(t)$ , $\mathbf{y}(t)$ )。）
3.  With this notation, the multivariable chain rule can be written more compactly as a dot product between the gradient of f and the vector-derivative of 𝐯(𝑡).（使用这种符号表示法，多元链式法则可以更简洁地写成 f 的梯度和 𝐯(𝑡) 的向量导数的点积。）
4.  Written like this, the analogy with the single-variable derivative is clearer.（以这种方式写，与单变量导数的类比更加清晰。）
5.  The gradient Vf plays the role of the derivative of f, and the vector derivative 𝐯(𝑡) plays the role as the ordinary derivative of g.（梯度 Vf 扮演 f 的导数的角色，而向量导数 𝐯(𝑡) 扮演 g 的普通导数的角色。）
6.  As a warm up, consider the single variable chain rule for a composition like f(g(t)).（作为热身，考虑一下复合函数 f(g(t)) 的单变量链式法则。）

--- pic\Multivariable chain rule, simple version.pdf_03.png ---

1. First, g maps a point t on the number line to another point g(t) the number line.（首先，g 将数轴上的一个点 t 映射到数轴上的另一个点 g(t)。）
2. Then f comes in and maps the point g(t) to yet another point on the number line, f(g(t)).（然后，f 进来，将点 g(t) 映射到数轴上的另一个点 f(g(t))。）
3.  Understanding the derivative of f(g(t)) requires understanding how a tiny change In t changes the final output.（理解 f(g(t)) 的导数需要理解微小变化 t 如何改变最终的输出。）
4.  The term dg/dt represents how a tiny change in t influences the intermediate output, g(t).（项 dg/dt 表示 t 的微小变化如何影响中间输出 g(t)。）
5.  If we move from an input t to an input t + h for a tiny value of h, the output of g will change by about dg/dt * h.（如果我们从输入 t 移动到输入 t + h（h 的值很小），则 g 的输出大约会改变 dg/dt * h。）
6.  You can imagine multiplying both sides by h in the limit above.（您可以想象在上面的极限中将两边都乘以 h。）
7.  The smaller h is, the smaller the error between this value and the real change g(to + h) — g(to).（h 越小，这个值与实际变化 g(to + h) — g(to) 之间的误差越小。）
8.  The term df/dg represents how a tiny change in g influences the final output f(g(t)).（项 df/dg 表示 g 的微小变化如何影响最终的输出 f(g(t))。）

--- pic\Multivariable chain rule, simple version.pdf_04.png ---

1. If we move from a point g(t0) to g(t0) + k for some small k, the output of f will change by about.（如果我们从点 g(t0) 移动到 g(t0) + k，其中 k 很小，那么 f 的输出将大约变化。）
2. The total change in f due to a small change in t is then the product of both these influences.（由于 t 的微小变化而导致的 f 的总变化就是这两个影响的乘积。）
3. Combining the previous two explanations, if the change in g was caused by a change of h to to, then this change k to g(to) is about.（结合前面两个解释，如果 g 的变化是由于 h 对 to 的改变而引起的，那么 k 对 g(to) 的改变大约是。）
4. The smaller h is, the more true this estimate Is.（h 越小，这个估计值越接近真实值。）
5. The intuition ts similar for the multivariable chain rule.（对于多元链式法则，直觉类似。）
6. You can think of v as mapping a point on the number line to a point on the xy-plane, and f(𝐯(𝑡)) as mapping that point back down to some place on the number line.（您可以将 v 视为将数轴上的一个点映射到 xy 平面上的一个点，将 f(𝐯(𝑡)) 视为将该点映射回数轴上的某个位置。）
7. The question is, how does a small change in the initial input t change the total output f(𝐯(𝑡))?（问题是，初始输入 t 的微小变化如何改变总输出 f(𝐯(𝑡))？）

--- pic\Multivariable chain rule, simple version.pdf_05.png ---

1. Let's break down what the multivariable chain rule is saying, spelling it out in terms of the component functions x(t) and $\mathbf{y}(t)$ :（让我们分解一下多元链式法则在分量函数 x(t) 和 $\mathbf{y}(t)$  方面的表述：）
2. The term dg/dt represents how a tiny change in t influences the intermediate output, g(t).（项 dg/dt 表示 t 的微小变化如何影响中间输出 g(t)。）
3. For small values of h（对于小的 h 值）
4. Likewise, the term dy/dt represents how a tiny change in t influences the second intermediate output, $\mathbf{y}(t)$ .（同样地，项 dy/dt 表示 t 的微小变化如何影响第二个中间输出 $\mathbf{y}(t)$ 。）
5. For small values of h（对于小的 h 值）
6. The term ∂f/∂x represents how a tiny change to the z-component of an input to f influences its output, and similarly the term ∂f/∂y accounts for how a small change to the y-component of the input changes f.（项 —— 表示对 f 的输入的 z 分量的微小变化如何影响其输出，类似地，项 2 表示输入的 y 分量的微小变化如何改变 f。）
7. For small values of k（对于小的 k 值）

--- pic\Multivariable chain rule, simple version.pdf_06.png ---

1. One way a small change to t influences f(x(t), $\mathbf{y}(t)$ ) is that it first changes x(t), which in turn changes f. This effect is captured in the (∂f/∂x)(∂x/∂t) product.（一个改变 t 的微小变化影响 f(x(t), $\mathbf{y}(t)$ ) 的一种方式是它首先改变了 x(t)，然后又改变了 f。这个效应在 (∂f/∂x)(∂x/∂t) 的乘积中得到了捕捉。）
2. The change in f due to the small change in x(t), which in turn is caused by a small change t, is expressed like this: （由于 x(t) 的微小变化，f 的变化也发生了变化，而 x(t) 的微小变化又是由于 t 的微小变化引起的，这样表达）
3. We know that x(t0 + h) is well approximated as （我们知道 x(t0 + h) 可以很好地近似为）
4. So the quantity we care about now becomes （因此，我们现在关心的数量变为）
5. But this expression is just asking how a certain small change to the x coordinate of the input to f influences the output, which we know to be well approximated using the partial derivative with respect to x.（但这个表达式只是在询问对 f 的输入的 x 坐标的某个微小变化如何影响输出，我们知道可以使用关于 x 的偏导数来很好地近似这个影响。）
6. The other way a change to t changes the output of f(x(t), $\mathbf{y}(t)$ ) is by first changing the second intermediate output $\mathbf{y}(t)$ , which in turn affects the output of f.（t 的变化改变了 f(x(t), $\mathbf{y}(t)$ ) 的输出的另一种方式是首先改变第二个中间输出 $\mathbf{y}(t)$ ，进而影响了 f 的输出。）
7. This effect is captured in the product (∂f/∂y)(dy/dt).（这个效应在 (∂f/∂y)(dy/dt) 的乘积中得到了捕捉。）
8. Adding these two products gives the total change in f.（将这两个乘积相加得到 f 的总变化。）
9. You might notice that the dot product expression for the multivariable chain rule looks a lot like a directional derivative.（您可能会注意到，多元链式法则的点积表达式与方向导数非常相似。）

--- pic\Multivariable chain rule, simple version.pdf_07.png ---

1. In fact, that's exactly what it is!（事实上，那确实就是它！）
2. The derivative v'(t0) at a particular value to gives a vector in the input space of f.（特定值 t0 处的导数 v'(t0) 给出了 f 的输入空间中的一个向量。）
3. If 𝐯(𝑡) is interpreted as a parametric path inside this space, perhaps thought of as the trajectory of a particle, the derivative at a particular point in time t0 gives the velocity vector of this particle at that time.（如果将 𝐯(𝑡) 解释为此空间内的参数路径，可以将其视为粒子的轨迹，则特定时间点 t0 处的导数给出了该粒子在该时间点的速度向量。）
4. With this interpretation, the chain rule tells us that the derivative of the composition f(𝐯(𝑡)) is the directional derivative of f along the derivative of 𝐯(𝑡).（根据这种解释，链式法则告诉我们，复合函数 f(𝐯(𝑡)) 的导数是 f 沿着 𝐯(𝑡) 的导数的方向导数。）
5. This should make sense, because a tiny change by "dt" to t should, by the meaning of the derivative, cause a tiny change dv to the output of 𝐯(𝑡).（这是有道理的，因为对 t 的微小变化 "dt" 应该根据导数的含义导致 𝐯(𝑡) 的输出发生微小变化 dv。）
6. And the point of the directional derivative is that a tiny change dv to the input of f should cause a change df as determined by ∂f/∂v = ∇v₀ f.（方向导数的目的是，对 f 的输入进行微小变化 dv 应该导致由 ∂f/∂v = ∇v₀ f 决定的 df 的变化。）
7. Example 1: With and without the new chain rule（示例1：使用和不使用新的链式法则）
8. Define f(x, y) like this: $f(x, y) = x^2 y$ (将 f(x, y) 定义为：$f(x, y) = x^2 y$)
9. And define 𝐯(𝑡) like this:（将𝐯(𝑡)定义为：） 

--- pic\Multivariable chain rule, simple version.pdf_08.png ---
1. Find the derivative $\frac{d}{dt} f(\mathbf{v}(t))$. (找到 $\frac{d}{dt} f(\mathbf{v}(t))$ 的导数。)
2. Before throwing our fancy new tool at the problem, it's worth pointing out that this is something we can solve by first writing out the composition as a single variable function of t: $f(\mathbf{v}(t)) = f(\cos(t), \sin(t))$ = $\cos(t)^2 \sin(t)$ (在我们使用新工具解决问题之前，值得指出的是，我们可以通过首先将复合函数写为t的单变量函数来解决这个问题：$f(\mathbf{v}(t)) = f(\cos(t), \sin(t)) = \cos^2(t) \sin(t)$。)
3. Now you can take the ordinary derivative: （现在可以进行普通的导数计算）
4. But of course, the purpose of this example is to get a feel for what the chain rule feels like.（当然，这个例子的目的是让你对链式法则有所感觉。）
5. "Solution using chain rule: First, let's explicitly state the component functions of 𝐯(𝑡): $\mathbf{x}(t)$  = $\cos(t)$  $\mathbf{y}(t)$  = $\sin(t)$  According to the chain rule, $\frac{d}{dt} f(\mathbf{v}(t))=\frac{\partial f}{\partial x} \frac{dx}{dt} + \frac{\partial f}{\partial y} \frac{dy}{dt}$"（使用链式法则的解决方案：首先，让我们明确地陈述𝐯(𝑡)的组成函数：$\mathbf{x}(t)$  = $\cos(t)$  $\mathbf{y}(t)$  = $\sin(t)$  根据链式法则，$\frac{d}{dt} f(\mathbf{v}(t))=\frac{\partial f}{\partial x} \frac{dx}{dt} + \frac{\partial f}{\partial y} \frac{dy}{dt}$）

--- pic\Multivariable chain rule, simple version.pdf_09.png ---

1. Taking the partial derivatives of $f(x, y) = x^2 y$ and the ordinary derivatives of $\mathbf{x}(t)$  = $\cos(t)$ , $\mathbf{y}(t)$  = $\sin(t)$ , we get.（对 $f(x, y) = x^2 y$ 和 $\mathbf{x}(t)$  = $\cos(t)$ , $\mathbf{y}(t)$  = $\sin(t)$  进行偏导数和普通导数运算，我们得到）
2. We want everything in terms of t, so we plug in $x$= $\cos(t)$  and y = $\sin(t)$ .（我们希望将所有内容都转换为 t 的形式，因此我们将 $x$= $\cos(t)$  和 y = $\sin(t)$  带入。）
3. Reassuringly, this is the same as the answer we got without using the chain rule.（令人欣慰的是，这与我们在不使用链式法则时得到的答案相同。）
4. You might be thinking that this new chain rule makes things unnecessarily complicated, and the dirty little secret is that for concrete computations like this one, it is often not needed.（你可能会认为这个新的链式法则使事情变得不必要地复杂，而事实是，对于像这样的具体计算，它通常是不需要的。）
5. However, it is useful for writing equations in terms of an unknown function, as the next example shows.（然而，对于用未知函数编写方程来说，它是有用的，正如下一个例子所示。）
6. Suppose the temperature across a two-dimensional region varies according to a function T(z, y), which we do not know.（假设跨越一个二维区域的温度根据一个我们不知道的函数 T(z, y) 变化。）
7. You wander throughout this region, sampling temperatures as you go, and your x and y coordinates as functions of time are $\mathbf{x}(t)$  = 30 cos(2t) $\mathbf{y}(t)$  = 40sin(3t) In taking your measurements, you notice that the temperature never changes along your path.（你在这个区域里四处游荡，一边走一边取样温度，你的 x 和 y 坐标作为时间的函数分别是 $\mathbf{x}(t)$  = 30 cos(2t) $\mathbf{y}(t)$  = 40sin(3t)。在进行测量时，你注意到沿着你的路径温度从不改变。）
8. What can you say about the partial derivatives of T°?（关于 T° 的偏导数，你能说些什么？）

--- pic\Multivariable chain rule, simple version.pdf_10.png ---

1. The temperature you experience, as a function of time, Is T (a(t), $\mathbf{y}(t)$ ) = T'(30 cos(2t), 40 sin(3t)).（作为时间函数，你所经历的温度是 T(a(t), $\mathbf{y}(t)$ ) = T'(30 cos(2t), 40 sin(3t))。）
2. The fact that the temperature you experience never changes means the derivative of this temperature, as a function of time, is 0.（你所经历的温度从不改变这个事实意味着该温度作为时间函数的导数为 0。）
3. Using the multivariable chain rule, we can write the derivative of this function in terms of the partial derivatives of T: （使用多元链式法则，我们可以根据 T 的偏导数来写出该函数的导数：）
4. More accurately, we should be evaluating these partial derivatives at (x,y) = (30 cos(2t), 40 sin(3t)), so the full expression for what we know about the unknown temperature function T is （更准确地说，我们应该在 (x,y) = (30 cos(2t), 40 sin(3t)) 处评估这些偏导数，因此我们关于未知温度函数 T 的全部表达式是 ）
5. Given a multivariable function f(x, y), and two single variable functions $\mathbf{x}(t)$  and $\mathbf{y}(t)$ , here's what the multivariable chain rule says:（给定一个多元函数 f(x, y)，以及两个单变量函数 $\mathbf{x}(t)$  和 $\mathbf{y}(t)$ ，下面是多元链式法则的表述：）
6. Written with vector notation, where $
\mathbf{v}(t) = \begin{bmatrix} x(t) \\ y(t) \end{bmatrix}
$, this rule has a very elegant form in terms of the gradient of f and the vector derivative of 𝐯(𝑡).（用向量表示法写成，其中 $\mathbf{v}(t) = \begin{bmatrix} x(t) \\ y(t) \end{bmatrix}$，这个规则在 f 的梯度和 𝐯(𝑡) 的向量导数方面具有非常优雅的形式。）

