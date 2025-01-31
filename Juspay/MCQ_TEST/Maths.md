# Mathematics Notes
# Mathematics Formula Table

## 1. Linear Algebra
| Concept                | Formula                                              | Description |
|------------------------|------------------------------------------------------|-------------|
| **Matrix Addition**    | `C = A + B`                                          | Add corresponding elements |
| **Scalar Multiplication** | `λA = [λa_ij]`                                   | Multiply each element by `λ` |
| **Matrix Multiplication** | `C = A × B`, where `C_ij = Σ(A_ik × B_kj)`        | Multiply row of A with column of B |
| **Determinant (2×2)**  | `\|A\| = ad - bc`                                      | `|A|` for a `2×2` matrix |
| **Determinant (3×3)**  | `\|A\| = a(ei − fh) − b(di − fg) + c(dh − eg)`        | Expansion method for `3×3` matrix |
| **Eigenvalue Equation** | `\|A - λI\| = 0`                                      | Solve for `λ` (eigenvalues) |
| **Eigenvector Equation** | `(A - λI)v = 0`                                   | Solve for `v` (eigenvectors) |

---

## 2. Calculus
| Concept               | Formula                                              | Description |
|-----------------------|------------------------------------------------------|-------------|
| **Derivative Definition** | `f'(x) = lim(h→0) [f(x+h) - f(x)] / h`           | Rate of change |
| **Power Rule**       | `d/dx [x^n] = n * x^(n-1)`                           | Differentiate `x^n` |
| **Product Rule**     | `d/dx [uv] = u'v + uv'`                              | Differentiation of product |
| **Quotient Rule**    | `d/dx [u/v] = (u'v - uv') / v²`                      | Differentiation of division |
| **Chain Rule**       | `d/dx [f(g(x))] = f'(g(x)) * g'(x)`                  | Derivative of composite functions |
| **Basic Integrals**  | `∫x^n dx = (x^(n+1)) / (n+1) + C`                    | Integral of `x^n` |
| **Integration by Parts** | `∫udv = uv - ∫vdu`                               | Integration of product functions |
| **Definite Integral** | `∫[a to b] f(x)dx = F(b) - F(a)`                    | Evaluating area under a curve |
| **Limit Definition** | `lim(x→a) f(x) = L`                                  | Value of function as `x` approaches `a` |
| **L'Hôpital's Rule** | `lim(x→a) f(x)/g(x) = lim(x→a) f'(x)/g'(x)`          | Solving indeterminate limits |

---

## 3. Probability & Statistics
| Concept                  | Formula                                          | Description |
|--------------------------|-------------------------------------------------|-------------|
| **Basic Probability**    | `P(A) = n(A) / n(S)`                            | Probability of event A |
| **Addition Rule**        | `P(A or B) = P(A) + P(B) - P(A and B)`          | Probability of union |
| **Conditional Probability** | `P(A \| B) = P(A and B) / P(B)`               | Probability of A given B |
| **Bayes’ Theorem**       | `P(A \| B) = [P(B \| A) * P(A)] / P(B)`           | Updating probabilities |
| **Mean (Average)**       | `Mean = Σx / n`                                 | Average value |
| **Median**               | Middle value of sorted data                     | Central data point |
| **Standard Deviation**   | `σ = √(Σ(x_i - μ)² / n)`                        | Measure of data spread |

---

## 4. Algebra & Equations
| Concept                  | Formula                                          | Description |
|--------------------------|-------------------------------------------------|-------------|
| **Quadratic Equation**   | `ax² + bx + c = 0`                              | Standard form of quadratic equation |
| **Quadratic Formula**    | `x = (-b ± √(b² - 4ac)) / 2a`                   | Finding roots of quadratic equation |
| **Logarithm Definition** | `log_b(x) = y` → `b^y = x`                      | Inverse of exponentiation |
| **Logarithm Properties** | `log(ab) = log a + log b`                       | Product rule |
|                          | `log(a/b) = log a - log b`                       | Quotient rule |
|                          | `log(a^n) = n log a`                            | Power rule |
| **Arithmetic Progression (AP)** | `a_n = a_1 + (n-1)d`                  | nth term formula |
| **Sum of AP**            | `S_n = n/2 * (2a + (n-1)d)`                      | Sum of first `n` terms |
| **Geometric Progression (GP)** | `a_n = a_1 * r^(n-1)`                  | nth term formula |
| **Sum of GP**            | `S_n = a(1 - r^n) / (1 - r)` (for `r < 1`)      | Sum of `n` terms |

---

## 5. Trigonometry
| Concept                | Formula                                         | Description |
|------------------------|------------------------------------------------|-------------|
| **Basic Identities**   | `sin²(x) + cos²(x) = 1`                        | Pythagorean identity |
|                       | `1 + tan²(x) = sec²(x)`                         | Pythagorean identity |
|                       | `1 + cot²(x) = cosec²(x)`                       | Pythagorean identity |
| **Sine Rule**         | `sin A / a = sin B / b = sin C / c`             | Relationship between sides & angles |
| **Cosine Rule**       | `cos A = (b² + c² - a²) / 2bc`                  | Relation between sides & angles |
| **Radians to Degrees** | `Degrees = Radians × (180/π)`                  | Conversion formula |
| **Degrees to Radians** | `Radians = Degrees × (π/180)`                  | Conversion formula |

---
## 1. Linear Algebra

### **1.1 Matrices**
A **matrix** is a rectangular array of numbers, symbols, or expressions arranged in rows and columns.  
A matrix of size `m × n` has `m` rows and `n` columns.

#### **Matrix Operations:**
1. **Addition & Subtraction**: If `A` and `B` have the same dimensions,
   - `C = A + B` → Add corresponding elements.
   - `C = A - B` → Subtract corresponding elements.
2. **Scalar Multiplication**: `λA = [λa_ij]` (Multiply each element by scalar `λ`).
3. **Matrix Multiplication**: If `A (m × p)` and `B (p × n)`, then:
   - `C = A × B` where `C_ij = Σ(A_ik × B_kj)` for `k = 1` to `p`.

### **1.2 Determinants**
The **determinant** of a square matrix provides information about the matrix properties, such as invertibility.

**For a 2×2 matrix:**

$$
|A| = \begin{vmatrix} 
a & b \\ 
c & d 
\end{vmatrix} = (ad - bc)
$$

---

**For a 3×3 matrix:**

$$
|A| = \begin{vmatrix} 
a & b & c \\ 
d & e & f \\ 
g & h & i 
\end{vmatrix} = a(ei - fh) - b(di - fg) + c(dh - eg)
$$
       
### **1.3 Eigenvalues and Eigenvectors**
For a **square matrix** `A`, an **eigenvector** `v` and an **eigenvalue** `λ` satisfy:

\[
Av = \lambda v
\]

- **Eigenvalues** are solutions of `|A - λI| = 0`, where `I` is the identity matrix.
- **Eigenvectors** are nonzero vectors satisfying `(A - λI)v = 0`.

---

## 2. Calculus

### **2.1 Differentiation**
Differentiation gives the rate of change of a function. If `f(x)` is a function, its **derivative** is:

\[
f'(x) = \lim_{h→0} \frac{f(x+h) - f(x)}{h}
\]

#### **Basic Differentiation Rules**
1. **Power Rule:** `d/dx [x^n] = n * x^(n-1)`
2. **Product Rule:** `d/dx [u * v] = u' * v + u * v'`
3. **Quotient Rule:** `d/dx [u / v] = (u' * v - u * v') / v²`
4. **Chain Rule:** `d/dx [f(g(x))] = f'(g(x)) * g'(x)`

#### **Common Derivatives**
- `d/dx [sin(x)] = cos(x)`
- `d/dx [cos(x)] = -sin(x)`
- `d/dx [e^x] = e^x`
- `d/dx [ln(x)] = 1/x`

### **2.2 Integration**
Integration is the reverse process of differentiation, used to find the **area under a curve**.

\[
\int f(x)dx = F(x) + C
\]

#### **Basic Integration Rules**
1. **Power Rule:** `∫x^n dx = (x^(n+1)) / (n+1) + C`, for `n ≠ -1`
2. **Integration by Parts:** `∫u dv = uv - ∫v du`
3. **Definite Integral:** `∫[a to b] f(x)dx = F(b) - F(a)`

### **2.3 Limits**
Limits describe the behavior of a function as the input approaches a specific value.

\[
\lim_{x→a} f(x) = L
\]

#### **Common Limits**
1. `lim(x→0) (sin x / x) = 1`
2. `lim(x→∞) (1 + 1/x)^x = e`
3. `lim(x→0) (1 - cos x) / x² = 1/2`

---

## 3. Probability & Statistics

### **3.1 Basic Probability**
The **probability** of an event `A` occurring is:

\[
P(A) = \frac{\text{Number of favorable outcomes}}{\text{Total number of outcomes}}
\]

#### **Probability Rules**
1. `0 ≤ P(A) ≤ 1`
2. `P(A or B) = P(A) + P(B) - P(A and B)`
3. `P(A | B) = P(A and B) / P(B)`

### **3.2 Mean, Median, Mode**
- **Mean (Average):** `Mean = Σx / n`
- **Median:** Middle value of sorted data.
- **Mode:** The most frequently occurring value.

### **3.3 Standard Deviation**
Measures the spread of data:

\[
σ = \sqrt{\frac{\sum (x_i - μ)^2}{n}}
\]

where `μ` is the mean, `x_i` are data points, and `n` is the number of values.

---

## 4. Algebra & Equations

### **4.1 Quadratic Equations**
A quadratic equation is:

\[
ax^2 + bx + c = 0
\]

The **roots** are found using the **quadratic formula**:

\[
x = \frac{-b ± \sqrt{b^2 - 4ac}}{2a}
\]

### **4.2 Logarithms**
A logarithm is the inverse of exponentiation:

\[
\log_b(x) = y \text{ if and only if } b^y = x
\]

#### **Logarithm Properties**
1. `log(ab) = log a + log b`
2. `log(a/b) = log a - log b`
3. `log(a^n) = n log a`

### **4.3 Progressions**
- **Arithmetic Progression (AP):**
  - nth term: `a_n = a_1 + (n-1)d`
  - Sum of `n` terms: `S_n = n/2 * (2a + (n-1)d)`
- **Geometric Progression (GP):**
  - nth term: `a_n = a_1 * r^(n-1)`
  - Sum of `n` terms: `S_n = a(1 - r^n) / (1 - r)`, for `r < 1`

---

## 5. Trigonometry

### **5.1 Basic Identities**
1. `sin²(x) + cos²(x) = 1`
2. `1 + tan²(x) = sec²(x)`
3. `1 + cot²(x) = cosec²(x)`

### **5.2 Sine & Cosine Rules**
- **Sine Rule:** `sin A / a = sin B / b = sin C / c`
- **Cosine Rule:** `cos A = (b² + c² - a²) / 2bc`

### **5.3 Angle Conversion**
1. **Radians to Degrees:** `Degrees = Radians × (180/π)`
2. **Degrees to Radians:** `Radians = Degrees × (π/180)`
