---
title: Markdown
subtitle: This page is written in Markdown.
---

Here's some inline KaTeX: \\(x^{2} + y^{2} = z^{2}\\).
The paragraph continues on after the equation like this.

Here's some block-level KaTeX without any markup wrapping it:

$$
    \int x^2 \cdot cos(x) \, dx
$$

In general, you should wrap KaTeX markup in a block-level HTML tag so the
Markdown parser will ignore it.

Here's a block-level equation inside a `<div>` tag:

<div>
    \begin{equation}
        1 + 2 = 3
    \end{equation}
</div>

Here's a block-level equation inside a `<p>` tag:

<p>
    \begin{equation}
        x + y = z
    \end{equation}
</p>

Here's a matrix inside a `<p>` tag:

<p>
    $$
    \begin{pmatrix}
        a & b \\
        c & d
    \end{pmatrix}
    $$
</p>

The matrix won't render without the `$$` wrappers, even though the KaTeX
documentation says it should.

One final equation for luck, without any wrappers:

\begin{equation}
    e = m \cdot c^2
\end{equation}

And a final paragraph with no math markup.
