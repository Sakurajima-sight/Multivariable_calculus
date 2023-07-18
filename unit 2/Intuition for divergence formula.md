  --- pic\Intuition for divergence formula.pdf_00.png ---

1. Intuition for divergence formula
  对散度公式的直观理解

2. Why does adding up certain partial derivatives have anything to do with outward fluid flow?
  为什么加起某些偏导数与流体向外流动有关？

3. Background: Divergence
  背景：散度

4. Warmup for the intuition
  对直观理解的热身

5. In the last article, I showed you the formula for divergence, as well as the physical concept it represents.
  在上一篇文章中，我向你展示了散度的公式，以及它代表的物理概念。

6. However, you might still be wondering how these two are connected.
  然而，你可能仍在想这两者如何联系在一起。

7. Before we dive into the intuition, the following questions should help us warm up by thinking of partial derivatives in the context of a vector field.
  在我们深入理解之前，以下的问题应该通过在矢量场的背景下思考偏导数来帮助我们进行热身。

8. Reflection question: A two-dimensional vector field is given by a function v defined with two components $v_1$ and $v_2$.
  反思问题：一个二维向量场由一个由两个分量$v_1$和$v_2$定义的函数v给出。

9. A few vectors near a point $(x_0, y_0)$ are sketched below:
  在点$(x_0, y_0)$附近的几个向量如下图所示：

10. Which of the following describes $v_1$ $(x_0, y_0)$?
    以下哪个描述了 $v_1$ $(x_0, y_0)$？



--- pic\Intuition for divergence formula.pdf_01.png ---

1. Remember, since $v_1$ is the first component of v, it measures the component of each vector in the x direction, or the horizontal component.
    记住，由于$v_1$是v的第一部分，所以它衡量的是每个向量在x方向上的部分，或者说是水平部分。

12. The arrow attached to the point $(x_0, y_0)$ has no horizontal component, since it points straight up, so $v_1$ $(x_0, y_0)$ = 0.
    附在点$(x_0, y_0)$的箭头没有水平分量，因为它直接指向上，所以$v_1$$(x_0, y_0)$= 0。

13. Which of the following describes $v_2$$(x_0, y_0)$? Choose 1 answer: (a) Positive (b) Zero (c) Negative
    以下哪个描述了$v_2$$(x_0, y_0)$？请选择1个答案：（a）正数 (b) 零 (c) 负数

14. Since $v_2$ is the second component of v, it measures the component of each vector in the y direction, or the vertical component.
    由于$v_2$是v的第二部分，所以它衡量的是每个向量在y方向上的部分，或者说是垂直部分。

15. The arrow attached to $(x_0, y_0)$ points up, hence it has a positive vertical component.
    附在$(x_0, y_0)$的箭头指向上，因此它有一个正的垂直分量。

16. Which of the following describes $\frac{\partial v_1}{\partial x}$ $(x_0, y_0)$?
    以下哪个描述了$\frac{\partial v_1}{\partial x}$ $(x_0, y_0)$？



--- pic\Intuition for divergence formula.pdf_02.png ---

1. The partial derivative$\frac{\partial v_1}{\partial x}$ $(x_0, y_0)$ measures how much $v_1$ changes as x changes.
偏导数$\frac{\partial v_1}{\partial x}$ $(x_0, y_0)$ 测量的是当x变化时，$v_1$变化多少。

18. In other words, what happens to the horizontal components of vectors as we move from the left to the right.
换句话说，当我们从左到右移动时，向量的水平分量发生了什么变化。

19. As you pan from left to right around $(x_0, y_0)$, the arrows go from pointing a little right, to having zero horizontal component, to pointing a little left.
当你在$(x_0, y_0)$周围从左到右平移时，箭头从稍微指向右边，到没有水平分量，再到稍微指向左边。

20. Therefore the horizontal component of vectors near $(x_0, y_0)$ decreases as x increases, so  $\frac{\partial v_1}{\partial x}$ $(x_0, y_0)$ < 0.
因此，当x增大时，接近$(x_0, y_0)$的向量的水平分量会减小，所以$\frac{\partial v_1}{\partial x}$ $(x_0, y_0)$ < 0。

21. Which of the following describes $\frac{\partial v_2}{\partial y}$ $(x_0, y_0)$? Choose 1 answer: (a) Positive (b) Zero (c) Negative
以下哪个描述了$\frac{\partial v_2}{\partial y}$ $(x_0, y_0)$？请选择1个答案：（a）正数 (b) 零 (c) 负数

22. The partial derivative $\frac{\partial v_2}{\partial y}$ $(x_0, y_0)$ measures how much $v_2$ changes as y changes.
偏导数 $\frac{\partial v_2}{\partial y}$ $(x_0, y_0)$ 测量的是当y变化时，$v_2$变化多少。

23. In other words, what happens to the vertical components of vectors as we move from the bottom to the top.
换句话说，当我们从底部移动到顶部时，向量的垂直分量发生了什么变化。

24. As you pan from down to up around $(x_0, y_0)$, the upward component of each vector gets longer and longer.
当你在$(x_0, y_0)$周围从下到上平移时，每个向量的向上分量变得越来越长。

25. Therefore the vertical component of vectors near $(x_0, y_0)$ increases as y increases, so $\frac{\partial v_2}{\partial y}$ $(x_0, y_0)$ > 0.
    因此，当y增大时，接近$(x_0, y_0)$的向量的垂直分量会增大，所以 $\frac{\partial v_2}{\partial y}$ $(x_0, y_0)$ > 0.

26. Intuition behind the divergence formula
    散度公式背后的直观理解

27. Let's limit our view to a two-dimensional vector field,
    让我们将视角限制在二维向量场上，

28. Remember, the formula for divergence looks like this:
    记住，散度的公式如下：



--- pic\Intuition for divergence formula.pdf_03.png ---

1. Why does this have anything to do with changes in the density of a fluid flowing according to $v(x, y)$?
    这和按照$v(x, y)$流动的流体密度的变化有什么关系？

30. Let's look at each component separately.
    我们分别看看每个部分。

31. For example, suppose $v_1$ $(x_0, y_0)$ = 0, meaning the vector attached to $(x_0, y_0)$ has no horizontal component.
    例如，假设$v_1$$(x_0, y_0)$= 0，意味着附在$(x_0, y_0)$的向量没有水平分量。

32. And let's say$\frac{\partial v_1}{\partial x}$ $(x_0, y_0)$ happens to be positive.
    并且假设 $\frac{\partial v_1}{\partial x}$ $(x_0, y_0)$ 恰好是正数。

33. This means that near the point $(x_0, y_0)$, the vector field might look something like this.
    这意味着在点$(x_0, y_0)$附近，向量场可能看起来像这样。

34. Vectors point more to the right as you pan from left to right.
    当你从左向右平移时，向量更多地指向右边。

35. The value of $v_1$ $(x_0, y_0)$ increases as x grows.
    当x增大时，$v_1$$(x_0, y_0)$的值增加。

36. The value of $v_1$ $(x_0, y_0)$ decreases as x gets smaller.
    当x变小时，$v_1$$(x_0, y_0)$的值减小。

37. Therefore, vectors to the left of $(x_0, y_0)$ will point a little to the left, and vectors to the right of $(x_0, y_0)$ will point a little to the right.
    因此，$(x_0, y_0)$左边的向量会稍微指向左边，而$(x_0, y_0)$右边的向量会稍微指向右边。

38. see the diagram above.
    看上面的图。

39. This suggests an outward fluid flow, at least as far as the x-component is concerned.
    这暗示了一个向外的流体流动，至少在x分量上是这样。

40. In contrast, here's how it looks if $\frac{\partial v_1}{\partial x}$ $(x_0, y_0)$ is negative:
    相比之下，如果$\frac{\partial v_1}{\partial x}$$(x_0, y_0)$是负数，它看起来是这样的：

41. Vectors point more to the left as you pan from left to right.
    当你从左向右平移时，向量更多地指向左边。

42. The vectors to the left of $(x_0, y_0)$ will point to the right.
    $(x_0, y_0)$左边的向量会指向右边。

43. The vectors to the right of $(x_0, y_0)$ will point to the left.
    $(x_0, y_0)$右边的向量会指向左边。

44. This indicates an inward fluid flow, according to the x-component.
    根据x分量，这表示内向的流体流动。

45. The same intuition applies if v$(x_0, y_0)$ is nonzero.
    如果v$(x, y_0)$非零，同样的直观认识也适用。

46. For instance, if $v_1$ $(x_0, y_0)$ is positive and $\frac{\partial v_1}{\partial x}$ $(x_0, y_0)$ is also positive, this means all the vectors around $(x_0, y_0)$ point to the right, but they get bigger as we look from left to right.
    例如，如果$v_1$$(x, y_0)$是正的并且$\frac{\partial v_1}{\partial x}$$(x_0, y_0)$也是正的，这意味着围绕$(x_0, y_0)$的所有向量都指向右边，但当我们从左向右看时，它们变得更大。

47. You can imagine the fluid flowing slowly towards $(x_0, y_0)$ from the left, but flowing fast away from it to the right.
    你可以想象流体从左边慢慢地流向$(x_0, y_0)$，但从右边快速地流出。



--- pic\Intuition for divergence formula.pdf_04.png ---

1. Since more is leaving than is coming in, the density at this point decreases.
由于离开的比进来的要多，所以这一点的密度在减小。

49. Some fluid enters.
有一些流体进入。

50. More fluid leaves
更多的流体离开

51. Analyzing the value of $\frac{\partial v_2}{\partial y}$ is similar.
分析$\frac{\partial v_2}{\partial y}$的值是相似的。

52. It indicates the change in the vertical component of vectors, $v_2$, as one moves up and down in the vector field, changing y.
它指示了当在向量场中上下移动，改变y时，向量$v_2$的垂直分量的变化。

53. For example, suppose $v_2$$(x_0, y_0)$ = 0, meaning the vector attached to $(x_0, y_0)$ has no vertical component.
    例如，假设$v_2$$(x_0, y_0)$= 0，意味着附在$(x_0, y_0)$的向量没有垂直分量。

54. Also suppose $\frac{\partial v_2}{\partial y}$ $(x_0, y_0)$ is positive, meaning the vertical component of vectors increases as we move upward.
    也假设 $\frac{\partial v_2}{\partial y}$ $(x_0, y_0)$ 是正数，意味着当我们向上移动时，向量的垂直分量增加。

55. Here's how that might look:
    这可能是这样的：

56. Vectors point more up as you pan from the bottom to the top.
    当你从下往上平移时，向量更多地指向上方。

57. Vectors below $(x_0, y_0)$ will point slightly downward.
    $(x_0, y_0)$下方的向量会稍微指向下方。

58. Vectors above $(x_0, y_0)$ will point slightly upward.
    $(x_0, y_0)$上方的向量会稍微指向上方。

59. This indicates an outward fluid flow, as far as the y-direction is concerned.
    这表明了一个向外的流体流动，至少在y方向上是这样。

60. Likewise, if $\frac{\partial v_2}{\partial y}$ $(x_0, y_0)$ is negative, it indicates an inward fluid flow near $(x_0, y_0)$ as far as the y-direction is concerned.
    同样，如果$\frac{\partial v_2}{\partial y}$$(x_0, y_0)$是负数，它表示在y方向上，$(x_0, y_0)$附近的流体流动是内向的。

61. Vectors point more down as you pan from the bottom to the top.
    当你从底部向顶部移动时，向量更多地指向下方。

62. Divergence adds these two influences
    散度将这两种影响因素加在一起

63. Adding the two components $\frac{\partial v_1}{\partial x}$ and $\frac{\partial v_2}{\partial y}$ brings together the separate influences of the x and y directions in determining whether fluid-density near a given point increases or decreases.
    将两个分量$\frac{\partial v_1}{\partial x}$和$\frac{\partial v_2}{\partial y}$加在一起，汇集了x和y方向在决定给定点附近的流体密度是增加还是减少时的独立影响。



--- pic\Intuition for divergence formula.pdf_05.png ---

1. Change in density in the x-direction
x方向上的密度变化

65. Change in density in the y-direction
y方向上的密度变化