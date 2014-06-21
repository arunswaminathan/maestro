maestro
=======

Many computer science projects now involve runing programs on multiple machines, whether to collect data, run analysis, or parallelize computation. At a high level, an end-user operates on a pool of machines and allocates jobs, usually represented in a scripting language. Our purpose is to build a declarative programming language, named Maestro, for users to easily express units of computations (a.k.a. jobs) and their dependencies. The runtime then distributes the jobs and ensures an order that doesn’t conflict with expressed dependencies.

As an example, a researcher wants to run an experiment that is divided into 3 steps: populate a third party service, collect data from the service, and analyze the collected data. The data collection has to run an hour after population, but the analysis can start as soon as the data is collected. With Maestro, we can express this in just a few lines, as shown in 1.3.
Prior related work in this area includes the so-called infrastructure configuration management frameworks, some of the most popular being Puppet and Chef . Typical infrastructure configuration management allows system administrators to ex- press infrastructure configuration dependencies. Our approach differs in that it provides end-users the ability to express dependencies related to job work-flows.

Please refer to main.pdf for a detailed decription of the language whitepaper, the language reference manual, and a tutorial.
