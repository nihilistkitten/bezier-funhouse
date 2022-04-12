## Running

There are some performance issues on my machine (which is not the best,
especially GPU wise), especially to do with compiling the shader. Just a warning
to expect that to take a little while.

## Basics

Slerping works:

![Slerping](pics/slerping.png)

There is still some issue with discontinuities. Either my slerping is not
accurate enough, or more subdivisions are needed. Here's a picture with a more
extreme curve which demonstrates this:

![Slerping Discontinuities](pics/slerping-discontinuities.png)

I think this is just an issue with the granularity of this subdivision scheme;
similar discontinuities (in particular slight square-ish-ness of reflections of
spheres) seem to exist in the example photo.

The mirror's shadow also works, though it's very binary, and so it doesn't look
great:

![Shadows](pics/shadow.png)

## Extras

There's an optional toggle for multibounce, which seems to work:

![Multibounce](pics/multibounce.png)

The discontinuities from slerping become significantly more noticeable when
multibounce is enabled; presumably this is because the effect is cumulative. If
