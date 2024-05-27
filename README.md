---
layout: default
title: LaTeX Example
---

<script type="text/javascript" async
  src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

<script type="text/x-mathjax-config">
MathJax.Hub.Config({
  tex2jax: {
    inlineMath: [['$', '$'], ['\\(', '\\)']],
    processEscapes: true
  }
});
</script>

# LaTeX Rendering Example

This is an example of inline LaTeX: $E = mc^2$

This is an example of a displayed LaTeX equation:

$$
\int_{a}^{b} f(x) \, dx = F(b) - F(a)
$$

# 

> *[John Adams to Abigail](https://www.masshist.org/digitaladams/archive/doc?id=L17800512jasecond)*

![](https://upload.wikimedia.org/wikipedia/commons/4/49/%22The_School_of_Athens%22_by_Raffaello_Sanzio_da_Urbino.jpg)

### [God](https://www.economist.com/culture/2024/05/14/god-an-ageing-product-outperforms-expectations): 1st, 3rd, 5th, ♭♭7th, 9th  
1. Hunter-gatherer: spiritual teachings  (I)
2. Peasant: [humanism](https://www.uuftc.org) (B)
### Community: 11th, 13th
3. Farmer: judeo, christian (G)
4. Manufacturer: world religions (Y)
### Individual: ♯9,♭9,♯11,♭13 
5. Electricity: prophetic utterances (O)
6. Railway: individual experience (R)

#

I could fill Volumes with Descriptions of Temples and Palaces, Paintings, Sculptures, Tapestry, Porcelaine, etc -- if I could have time. But I could not do this without neglecting my duty. The Science of Government it is my Duty to study, more than all other Studies Sciences: the Art of Legislation and Administration and Negotiation, ought to take Place, indeed to exclude in a manner all other Arts. I must study Politicks and War that my sons may have liberty to study Painting and Poetry Mathematicks and Philosophy. My sons ought to study Mathematicks and Philosophy, Geography, natural History, Naval Architecture, navigation, Commerce and Agriculture, in order to give their Children a right to study Painting, Poetry, Musick, Architecture, Statuary, Tapestry and Porcelaine.

#

To demonstrate diminishing marginal utility visually, I'll create a plot that shows the relationship between total utility and the quantity of a good consumed, alongside a marginal utility curve. Additionally, I'll include some calculus notation and Greek symbols to illustrate the concept mathematically.

Here's a step-by-step plan:

1. **Define Utility Functions:**
   - **Total Utility (U):** A typical utility function $U(Q)$ where $Q$ is the quantity of the good.
   - **Marginal Utility (MU):** The derivative of total utility with respect to quantity, $MU(Q) = \frac{dU(Q)}{dQ}$

2. **Illustrate Diminishing Marginal Utility:**
   - Show that as $Q$ increases, $MU$ decreases.

3. **Mathematical Representation:**
   - Use calculus notation to explain the relationship between total utility and marginal utility.
   - Include Greek symbols like $\Delta$ (Delta) for change, and $\epsilon$ (epsilon) for a small increment.

Let’s create the visual:

```python
import numpy as np
import matplotlib.pyplot as plt

# Define the total utility function U(Q)
def total_utility(Q):
    return 100 * np.log(Q + 1)  # Logarithmic utility function for illustration

# Define the marginal utility function MU(Q)
def marginal_utility(Q):
    return 100 / (Q + 1)  # Derivative of the total utility function

# Generate data
Q = np.linspace(1, 100, 500)  # Quantity range from 1 to 100
U = total_utility(Q)
MU = marginal_utility(Q)

# Plotting
plt.figure(figsize=(14, 7))

# Plot Total Utility
plt.subplot(1, 2, 1)
plt.plot(Q, U, label=r'Total Utility $U(Q) = 100 \log(Q + 1)$', color='blue')
plt.title('Total Utility')
plt.xlabel('Quantity (Q)')
plt.ylabel('Total Utility (U)')
plt.legend()
plt.grid(True)

# Plot Marginal Utility
plt.subplot(1, 2, 2)
plt.plot(Q, MU, label=r'Marginal Utility $MU(Q) = \frac{dU(Q)}{dQ} = \frac{100}{Q + 1}$', color='red')
plt.title('Marginal Utility')
plt.xlabel('Quantity (Q)')
plt.ylabel('Marginal Utility (MU)')
plt.legend()
plt.grid(True)

# Adding some calculus notation and Greek symbols
plt.figtext(0.5, 0.02, r"$MU(Q) = \frac{dU(Q)}{dQ} = \lim_{\Delta Q \to 0} \frac{U(Q + \Delta Q) - U(Q)}{\Delta Q}$", ha="center", fontsize=12)

plt.tight_layout()
plt.show()
