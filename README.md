# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do *not* have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## Answers

Let us assume that inorder for two graphs to be isomprhic they must be completely connected. This means that if two graphs are not completly connected, they cannot be isomorphic.

Let us define two graphs. The first will be described as an adjancy list with values [[],[0],[0,1,3],[1]]. The second will be also described as an adjancy list with values [[1,2,3],[2],[3],[]].

Say we have a mapping function $f$ that is both one-to-one and onto that maps $V_1$ to $|V_2|$:
* $0 \rightarrow 3$
* $1 \rightarrow 2$
* $2 \rightarrow 0$
* $3 \rightarrow 1$

If we apply this mapping to the first graph, we transform [[],[0],[0,1,3],[1]] into [[],[3],[3,2,1],[2]] and if we sort the sub arrays this gives us [[0],[3],[1,2,3],[2]]. Now swapping the subarrays so they coralate with the mapping gives us [[1,2,3],[2],[3],[]] which is equal to the adjancy list of graph 2. This means that the first and second graph are isomorphic to one another.

From our previous assumption however that only completly connected graphs can be isomorphic, the first and second graph are not isomprphic. This is a contradiction so it must be that graphs that are not completly connected can be isomorphic.

## Sources

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.