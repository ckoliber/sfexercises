# LP Answers

-   **Answer Set**: No. 01
-   **Full Name**: Mohammad Hosein Nemati
-   **Student Code**: `610300185`

---

## Exercise 1

-   Prove that $|F_m| = \aleph_0$:

1. First we describe the set $F_m$ by **partitioning** into the sets with **same length sentences**:

    $$
    \begin{aligned}
        & F_{m_1} = \{\overbrace{\bot, a, b, c, \dots}^{\aleph_0}\}
        \\
        & F_{m_2} = \{\bot \odot a, a \odot b, b \odot c, c \odot d, \dots\}
        \\
        & F_{m_3} = \{\bot \odot a \odot b, a \odot b \odot c, \dots\}
        \\
        & \vdots
        \\
        & F_{m_k} = \{\bot \odot a \odot b \odot c \odot \dots\}
    \end{aligned}
    $$

2. Now we find the size of each set:

    $$
    \begin{aligned}
        & |F_{m_1}| = \aleph_0
        \\
        & |F_{m_2}| = \aleph_0 \times 3 \times \aleph_0 = 3^1 \times \aleph_0^2
        \\
        & |F_{m_3}| = \aleph_0 \times 3 \times \aleph_0 \times 3 \times \aleph_0 = 3^2 \times \aleph_0^3
        \\
        & \vdots
        \\
        & |F_{m_k}| = \aleph_0 \times 3 \times \dots \times \aleph_0 = 3^{k-1} \times \aleph_0^{k}
    \end{aligned}
    $$

3. As we know, $k \times \aleph_0^q$ which $k$ and $q$ are constants, is equals to $\aleph_0$, so:

    $$
    \begin{aligned}
        & |F_{m_1}| = \aleph_0
        \\
        & |F_{m_2}| = \aleph_0
        \\
        & |F_{m_3}| = \aleph_0
        \\
        & \vdots
        \\
        & |F_{m_k}| = \aleph_0
        \\
        \\
        & |F_m| = \underbrace{\aleph_0 + \aleph_0 + \dots + \aleph_0}_{k} = k \times \aleph_0 = \aleph_0
    \end{aligned}
    $$

---

## Exercise 2

-   Proof these propositions in **Hilbert-System**:

1. $\vdash A \land B \to B \land A$

    $$
    \begin{align}
        & A \to B \lor A
    \end{align}
    $$

2. $\vdash A \lor B \to B \lor A$
3. $\vdash p \to \neg \neg p$
4. $\vdash (p \to (q \to r)) \to (p \land q \to r)$

---

## Exercise 3

-   Show that $\vdash p \to \neg \neg p$ but $\not\vdash \neg \neg p \to p$:

$$
\begin{align*}
    & \vdash p \to \neg \neg p
    \\
    & \vdash p \to ((p \to \bot) \to \bot)
    \\
    & p, (p \to \bot) \vdash \bot
\end{align*}
$$

---

## Exercise 4

-   Prove that if $M,x \models A$ and $x R y$ then $M,y \models A$:

1. Using the definition of kripke models we know:

    $$
    \begin{aligned}
        & \forall z (x R z \to V_z(A) = True)
    \end{aligned}
    $$

2. As we know the kripke models for intuitionistic logic has **Transitive** relation, so:

    $$
    \begin{aligned}
        & \forall z (y R z \to x R z)
    \end{aligned}
    $$

3. Using the inference rules **1** and **2**, we know:

    $$
    \begin{aligned}
        & \forall z (y R z \to V_z(A) = True)
    \end{aligned}
    $$

4. Now using the inference rule **3** we can see that $M,y \models A$.

---

## Exercise 5

-   Prove or find counter example:

1. $\models \neg \neg p \to p$
2. $\models p \lor q \to r \iff (p \to r) \land (q \to r)$
3. $\models \neg (p \lor \neg p)$
4. $\models (p \to q) \lor (q \to p)$

---

## Exercise 6

-   Prove that $m,\Gamma \models B$ iff $B \in \Gamma$:

---

## Exercise 7

-   Prove that $\vdash \neg \neg (p \lor \neg p)$:

---
