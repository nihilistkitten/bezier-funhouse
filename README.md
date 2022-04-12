Slerping works:

![Slerping](pics/slerping.png)

There is still some significant issue with discontinuities. Either my slerping
is not accurate enough, or more subdivisions are needed. Here's a picture with a
more extreme curve which demonstrates this:

![Slerping Discontinuities](pics/slerping-discontinuities.png)

I think this is just an issue with the granularity of this subdivision scheme;
similar discontinuities (in particular slight square-ish-ness of reflections of
spheres) seem to exist in the example photo.

The mirror's shadow also works, though it's very binary, and so it doesn't look
great:

![Shadows](pics/shadow.png)
