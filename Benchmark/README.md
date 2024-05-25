# Recipe Execution Benchmark

This benchmark for recipe understanding in autonomous agents aims to support progressing the domain of natural language understanding by providing a setting in which performance can be measured on the everyday human activity of cooking. Showing deep understanding of such an activity requires both linguistic and extralinguistic skills, including reasoning with domain knowledge. For this goal, the benchmark provides a number of recipes written in natural (human) English that should be converted to a procedural semantic network of cooking operations that can be interpreted and executed by autonomous agents. A system, which supports one-click installation and execution, is also included that can perform recipe execution tasks in simulation allowing both analysis and evaluation of predicted networks. The provided evaluation 
metrics are mostly simulation-based, because demonstrating deep understanding of recipes can be done by effectively taking all the appropriate actions required for cooking the intended dish.

## data 

The directory [data](data) contains the recipe texts which are meant to serve as test input for developed natural language understanding models and the gold standard solutions which are their ideal output. In addition to the ideal semantic network, gold standard files have also been included that specify which sentence has led to certain cooking operations being included in the network. This has mostly been added to provide further insight when analyzing test results after development. Some example recipe texts with annotations and comments are provided in the [documentation](documentation) directory for use during development.  

The directory [metadata](metadata) contains the online sources of all recipe data, including the date on which they were retrieved.

## executables

The directory [executables](executables) contains the standalone one-click executable, which will actually run the simulator and measure performance using the chosen metrics. More information about how to use this executable can be found in the [documentation](documentation) directory, including example scripts for running the simulator and example solution files with explained result interpretations.

The directory [libs](libs) contains the Python library Smatch, which is required in case the executable should compute Smatch Score during evaluation. The path to this Smatch library should be given as a parameter to the executable. Again, more information about this is given in the [documentation](documentation). 

## documentation

The directory [documentation](documentation) contains extensive documentation on the primitive cooking operations that are used to form the semantic networks, the metrics and their interpretations, the gold standard solutions and how they are formed as well as how to actually use and possibly even extend the provided simulator. 