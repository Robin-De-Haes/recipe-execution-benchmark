# A Benchmark for Recipe Understanding in Autonomous Agents

## Contact Information

| Name                      | Email address                                                       |
| :---                      | :---                                                                |
| Robin De Haes             | [robindehaes@msn.com](mailto:robindehaes@msn.com)                   |

## Abstract

Procedural text is composed of instructions on how to perform a specific task. Understanding such text requires insight into the impact of events on the world, which is a major component of intelligence. Benchmarks that support the development of artificial intelligence approaches towards achieving this capability often use recipes as a source of procedural text, because recipes are abundantly available and involve consistent tasks and tools. Moreover, deep recipe understanding could lead to many practical applications, such as the robotisation of everyday cooking.

Despite the existence of recipe benchmarks, the performance of robots is still limited when it comes to understanding an arbitrary recipe well enough to execute it. Current recipe understanding benchmarks have failed to achieve widespread adoption and lack important benchmark properties, which can slow down progress. They lack clear evaluation methods that could transfer results to the real world, overly promote specific types of models, and miss transparency regarding benchmark applicability and design.

In this thesis, we developed a new benchmark called the MUHAI Recipe Execution Benchmark, with all choices, properties, and general usage being transparently analyzed and documented. Specifically, we created the MUHAI Cooking Language, a graph-based, machine-readable representation language for recipe execution. A test set with gold standard recipe annotations in this language was then obtained through a data curation process. To avoid overfitting and overpromotion of a particular approach, only test data is curated to separate model development from model evaluation.

To perform model evaluation, we developed a symbolic simulator that measures performance using both simulation-based and non-simulation-based metrics. This combination allows for multiperspective performance estimates, optimizing transferability to real-world utility. Smatch, a commonly used semantic graph comparison tool, is included because of its high adoption rate, while simulation-based metrics are included due to their specificity in gauging recipe execution abilities. The developed simulation-based metrics include:

- **Goal-condition success**: Measures how many required goal-conditions have been traversed during recipe execution.
- **Dish approximation score**: Estimates the similarity between two prepared food products.
- **Recipe execution time**: Measures efficiency.

Whether the developed benchmark will achieve community-wide adoption and lead to significant advances in natural language understanding can only be determined in the future. Nevertheless, its transparent design makes it useful for developing recipe understanding approaches and could even serve as inspiration for new benchmarks.
