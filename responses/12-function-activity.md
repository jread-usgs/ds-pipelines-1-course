We've introduced you to the various phases of pipeline projects. Now you will add a commit to your pull request that makes changes to the code too.

#### background

In addition to phases, it is important to decompose high-level concepts (or existing scripts) into thoughtful functions and "targets" that form the building blocks of data processing pipelines. A target is a noun we use to describe a tangible output of function, often a file or an R object, that we can use as a terminal product (like a summary map) or as input into another function. 

We strive to create functions that declare their clear purpose (good naming and thoughtful arguments/inputs is helpful for this) and are designed for re-use as appropriate. When writing pipelines functions, look for areas of re-usable operations or places where simple dividing lines can be drawn between different parts of data access, processing, modeling/analysis, and visualization. We use the high-level "phases" to divide the *major* concepts, but the way we scope functions is an additional subdivide. It is a best practice to have a function do a single thing, so instead of creating two plots and a table, it might be better to use one function to generate a table, which is then used as input to another function to create a plot. There are exceptions to this pattern (a 1:1 function-to-target pairing) that we'll get into later. It is harder for us to connect robot responses up to assignments related to writing good functions, so we're going to be tagging the humans too...


### :keyboard: Activity: modify existing code to create functions that generate plot, table, and log file outputs

We’ve given you an example script in the my_work_R folder that loads data and generates 3 plots, one table, and a log file. This script isn’t very good and includes some bad practices that need to be cleaned up. Additionally, we’re asking that you split this single script into several functions that can be used to build the same five things. When you are happy with your changes, delete the example script (and the my_work_R folder) and commit your new script into git source control. Use your same folder structure that was created for your open PR. Push your commit(s) to the open pull request and assign `aappling-usgs` for review. 

<hr><h3 align="center">A real live human will interact with your pull request when you've added them as a reviewer.</h3>
