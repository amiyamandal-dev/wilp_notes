# Comprehensive Mathematical Foundations Notes

## 1. Linear Algebra

### Matrices and Linear Systems
- A **matrix** is a rectangular array of numbers arranged in rows and columns.
- Matrices represent linear systems of equations succinctly.

### Gaussian Elimination
- Solve linear equations using elementary row operations:
  - Swap rows, multiply rows by non-zero scalars, add multiples of one row to another.
- Goal: Convert to Row Echelon Form (REF) or Reduced Row Echelon Form (RREF).
- Types of solutions:
  - Unique solution (pivot in every column).
  - Infinite solutions (free variables).
  - No solution (inconsistent equations).

### Rank, Determinant, and Inverse
- **Rank:** Number of linearly independent rows or columns.
- **Determinant:** Indicates invertibility of a matrix.
  \[ \text{det}\begin{bmatrix}a & b\\c & d\end{bmatrix}=ad-bc \]
- **Inverse:**
  - Exists if determinant ≠ 0.
  - Computed using: \[ A^{-1} = \frac{1}{\text{det}(A)}\text{adj}(A) \]
  - Solves equations quickly: \[ Ax = b \Rightarrow x = A^{-1}b \]

## 2. Vectors and Vector Spaces

### Vectors
- Defined by an ordered list of numbers, having magnitude and direction.
- Operations:
  - **Addition:** Component-wise addition.
  - **Scalar Multiplication:** Multiply each component by scalar.

### Linear Combinations
- Any expression \( c_1v_1 + c_2v_2 + \dots + c_nv_n \).
- **Span:** Set of all linear combinations of given vectors.

### Linear Independence
- Vectors are independent if the only solution to \( c_1v_1 + \dots + c_nv_n = 0 \) is \( c_1 = \dots = c_n = 0 \).
- Verify using matrix rank or Gaussian elimination.

### Dot Product and Projections
- **Dot Product:** \[ a\cdot b = a_1b_1 + a_2b_2 + \dots + a_nb_n \]
- **Projection of vector \(v\) onto vector \(u\):**
\[ \text{proj}_u v = \frac{v \cdot u}{u \cdot u}u \]
- Orthogonality: vectors are orthogonal if dot product is 0.

## 3. Probability

### Basics
- **Sample Space (Ω):** All possible outcomes.
- **Events:** Subsets of the sample space.
- Probability axioms:
  - Non-negative probabilities.
  - Total probability equals 1.
  - Additivity for mutually exclusive events.

### Random Variables
- A numerical function mapping sample space outcomes.
- Types:
  - **Discrete:** Finite or countably infinite outcomes (e.g., die roll).
  - **Continuous:** Outcomes in continuous ranges, described by PDFs.

### Expectation, Variance, Covariance
- **Expectation (Mean):**
  - Discrete: \(E[X]=\sum xp(x)\)
  - Continuous: \(E[X]=\int xf(x)dx\)
- **Variance:** Measures spread around mean.
  - Formula: \(\text{Var}(X)=E[X^2]-(E[X])^2\)
- **Covariance:** Joint variability measure between two RVs.
  - \(\text{Cov}(X,Y)=E[XY]-E[X]E[Y]\)

## 4. Calculus

### Continuity
- A function \(f(x)\) is continuous at point \(c\) if \(\lim_{x \to c}f(x)=f(c)\).
- Types of discontinuities:
  - **Removable:** Limit exists, different from value.
  - **Jump:** Different left and right limits.
  - **Infinite:** Vertical asymptote.

### Derivatives
- Represents instantaneous rate of change.
- Formal definition:
  \[ f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}{h} \]
- Key derivative rules:
  - **Power Rule:** \(\frac{d}{dx}(x^n)=nx^{n-1}\)
  - **Product Rule:** \((uv)'=u'v+uv'\)
  - **Quotient Rule:** \((\frac{u}{v})'=\frac{u'v-uv'}{v^2}\)
  - **Chain Rule:** \((f(g(x)))'=f'(g(x))g'(x)\)

### Maxima and Minima
- **Critical Points:** Derivative zero or undefined.
- Tests to classify extrema:
  - **First Derivative Test:** Checks sign changes.
  - **Second Derivative Test:** Uses concavity (\(f''(x)\)).

## 5. Linear Programming

### Formulation
- Optimize linear objective function under linear constraints.
- Example: Maximize profit \(Z=ax+by\) with resource constraints.

### Graphical Method
- Graph constraints, determine feasible region.
- Optimal solutions at vertices (corners) of feasible region.

### Optimization
- Evaluate objective function at feasible region vertices.
- Select vertex providing optimal (maximum/minimum) solution.

## Practice Problems (Detailed Examples)
1. **Linear Systems:** Solve \(3x+2y=10, x-y=1\).
2. **Vector Projection:** Find projection of \((3,4)\) onto \((1,0)\).
3. **Variance:** Calculate variance for a fair die roll.
4. **Continuity:** Determine if \(f(x)=\frac{x^2-9}{x-3}\) is continuous at \(x=3\).
5. **Linear Programming:** Solve graphically to maximize \(Z=4x+3y\), constraints \(2x+y\le8, x+2y\le8\).

## Further Resources
- [Khan Academy - Comprehensive lessons and practice](https://www.khanacademy.org)
- [MIT OpenCourseWare - Detailed lecture notes and video lectures](https://ocw.mit.edu)
- [Paul’s Online Math Notes - Excellent summaries and examples](https://tutorial.math.lamar.edu)
- [3Blue1Brown - Visual explanations of math concepts](https://www.youtube.com/channel/UCYO_jab_esuFRV4b17AJtAw)

