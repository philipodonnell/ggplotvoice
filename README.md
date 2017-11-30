# ggplotvoice
### A proposal to create and manipulate ggplot2 charts live with your voice

Much of the difficulty in making others comfortable with data is the barrier of entry to the tools that allow the creation of interesting and informative visualizations. The idea of standing in front of a room and issuing commands like 

> Load this year's financials to date.

*a chart appears with the title '2016 Financials' and nothing else*

> Show me a line with revenue by month. 

*a `geom_line` appears with x=Month and y=Revenue*

> Split the line by division. 

*a `group` parameter is added by Division*

> Smooth the lines. 

*the `geom_line` is changed to a `geom_smooth`*

> Remove all the divisions except Operations. 

*filters the financials for only Division==Operations*

To implement this in base graphics or by writing application code would have requires a startup's worth of effort until the appearence of the closest thing we have to a spoken graphics language, [ggplot2](http://ggplot2.org/).

[ggplot2](http://ggplot2.org/) is based on the concept of a 'grammar of graphics' or the idea that it is possible to describe all of the parameters needed to create visualization in a semi-abstract topical grammar and have the specifics of the graph determined based on the interpretion/translation of the speech. The cumulative nature of the way it builds charts maps perfectly to the progressive nature of speech. The http://ggplot2.org/) is based on the concept of a 'grammar of graphics' or the idea that it is possible to describe all of the parameters needed to create visualization in a semi-abstract topical grammar and have the specifics of the graph determined based on the interpretion/translation of the speech. The cumulative nature of the way it builds charts maps perfectly to the progressive nature of speech. The `geom_`-style layers map well to how we would discuss a chart by speaking, and the way the `group` and `color` parameters are easy to speak to, beyond just what is on the x and y axis. 

But its not *quite* a spoken grammar, either, but it is conceptually close enough that filling in the gap should be attainable quickly.

## Speaking to `ggplot2`

This proposal is for a way of interpreting a spoken speech grammar into the neccessary ggplot2 grammar elements to render an arbitrary set of data into a useful visualization.



That leads to the natural question of, if its a grammar, why can't we speak  speak to it?

This proposal is an attempt to interpret human speech into a progressivly generated and automatically rendered plot.



