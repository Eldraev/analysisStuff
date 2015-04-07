# Front Page

![Screenshot](screenshot.JPG)

So yeah, see this as a candidate for a universal front page. It's kind of dynamic as well, the author field adds an "s" if you add more than one author.

## Usage

This requires the geometry package. Add the directory named "front" into your document directory. Then add this code **before** your <code>\begin{document}</code>:

```
\input{front/front.tex}
```

Then add this where you want your front page:

```
\front{Title}{Author}{Author}{Author}
```

As you can see, the front page only supports three authors in this current state. Also, if the names are too short or too long, bad things will happen...

Anywho. You need to have four parameters, even if you leave some empty. If you have one author, the code will therefore look like this:

```
\front{Title}{Author}{}{}
```
