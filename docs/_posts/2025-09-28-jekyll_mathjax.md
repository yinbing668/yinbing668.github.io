---
layout: post
---

# The following tutorial from google search Overview, It is really works.

To enable MathJax on a Jekyll site hosted with GitHub Pages, the primary method involves including the MathJax library within your site's HTML templates. Include MathJax CDN Script.
Edit your Jekyll layout files (e.g., _layouts/default.html or _layouts/post.html) to include the MathJax CDN script within the <head> section. A common way is to create an _includes/mathjax.html file with the script and then include it in your layouts.
Example _includes/mathjax.html content:

Then, in your layout file (e.g., _layouts/post.html), include it like this Code:



Configure MathJax (Optional).
You can customize MathJax's behavior, such as delimiters for inline and display math, by adding configuration options within the script tag or in a separate JavaScript file. Prevent Markdown Interference.
Jekyll's Markdown parser (Kramdown) can sometimes interfere with LaTeX syntax, particularly with underscores (interpreted as italics). To prevent this:
Escape underscores with a backslash (\_) in your LaTeX code.
Wrap inline math in <span>...</span> and display math in <div>...</div> tags.
Write Math Equations.
Use standard LaTeX syntax for your equations within your Markdown files. MathJax will render these equations in the browser. Push to GitHub Pages.
Commit your changes and push them to your GitHub Pages repository. GitHub Pages will build your Jekyll site, and the MathJax script will be included, enabling mathematical rendering.