# Front Page

![Screenshot](screenshot.JPG)

So yeah, see this as a candidate for a universal front page. It's kind of dynamic as well, the author field adds an "s" if you add more than one author. If you have no authors, that field will not show at all.

## Usage

Check the <code>../index.tex</code> file for a live example.

This requires the geometry package: <code>\usepackage[a4paper]{geometry}</code>. Add the directory named "front" into your document directory. Then add this code **before** your <code>\begin{document}</code>:

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

Feel free to improve the code if you have some time over. The code in this current state is a result from an insomnia driven Ted. I might as well have produced the code by banging my head on my home built and arduino driven keyboard X)
