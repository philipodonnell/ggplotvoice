# ggplotvoice
### A proposal to create and manipulate ggplot2 charts live with your voice

Much of the difficulty in making others comfortable with data is the barrier of entry to the tools that allow the creation of interesting and informative visualizations. This proposal attempts to make the process of building a visualization simple enough that a non-technical user can use simple, straightforward verbal commands to compose graphics and manipulate data live on a screen.

#### Why now?

To implement this in base graphics or by writing application code would have requires a startup's worth of effort until the appearence of the closest thing we have to a spoken graphics language, [ggplot2](http://ggplot2.org/).

Mostly the widespread availablility of R and the development of [ggplot2](http://ggplot2.org/). ggplot2 is based on the concept of a 'grammar of graphics' or the idea that it is possible to describe all of the parameters needed to create visualization in a semi-abstract topical grammar and have the specifics of the graph determined based on the interpretion/translation of the speech. The cummulative nature of the way it builds charts resembles the progressive nature of speech. The `geom_`-style layers seem similar to how we would discuss a chart by speaking, and the way the `group` and `color` parameters work are easy to speak aloud (beyond just what is on the x and y axis). 

It is not *quite* a spoken grammar, either, but it is conceptually close enough that filling in the gap should be attainable quickly. There are also some state-related tracking to deal with undo operations, or tracking which layer or part is currently being discussed.

#### Speaking to `ggplot2`

ggplot2 provides much of the rendering capability to actually produce a chart, so our work will focus mainly on defining the spoken grammar, mapping that to elements of the ggplot2 composition model, tracking scope and changes as the visualization evolves, and ultimately rendering the visualization.

The solution will need:

* The selection of a speech recognition engine to drive input
* A defined grammar that is acceptable to the recognizer

and a basic recognition loop:

* A way to update the grammar to add column and row names, distinct values, etc...
* The ability to translate the spoken grammar commands into the correct R/ggplot2 code
* Rendering of the ggplot2 code into an image
* Displaying that image to the user





