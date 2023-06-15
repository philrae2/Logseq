title:: Regression Testing in Agile: Concepts, Challenges and Strategies. (highlights)
author:: [[Sealights]]
full-title:: "Regression Testing in Agile: Concepts, Challenges and Strategies."
media:: #articles
url:: https://www.sealights.io/regression-testing/regression-testing-in-agile-concepts-challenges-and-strategies/
tags:: #[[regression testing]]

- Highlights first synced by [[Readwise]] [[2023-05-16]]
	- Regression testing in agile helps development teams concentrate on new functionality, while maintaining stability with every new product increment. Teams use regression testing to make sure that tested software continues to perform after every modification. Regression testing is the “stepchild” of agile testing, loved by few, but is essential to enable the high velocity that agile teams strive to achieve. ([View Highlight](https://read.readwise.io/read/01h0k1rbkd4s6hr7cc3p1dv2mr))
	- In agile, testing needs to develop with each sprint and testers must make sure that new changes do not affect existing functionality of the application. This is known as regression testing. ([View Highlight](https://read.readwise.io/read/01h0k1rnfrs38bb5fjf30az0ek))
	- There are three ways to undertake regression testing. The approach you select will vary according to your circumstances, the size of your codebase, the number of testers on your team, and your available resources.
	  
	  •   **Re-test everything**—involves rerunning all existing tests on the new codebase. If the tests were well designed, this will isolate regressions. However, this method is resource intensive and may not be feasible for a large codebase.
	  •   **Selective re-testing**—it is sometimes possible to identify a subset of your existing tests that can address all or almost all of the “moving parts” of your codebase. It is then sufficient to re-run that selective set to discover regressions across the codebase.
	  •   **Prioritized re-testing**—used on large codebases. The priority tests address code paths, user actions and areas of functionality expected to contain bugs. Once these tests have run you can complete the remaining tests. ([View Highlight](https://read.readwise.io/read/01h0k1sb3jmrna8wejdb55g71g))
	- **Is automation suitable for your project size?**
	  
	  Automated testing is efficient for large and medium-scale projects, especially when testing software with multiple sub-systems, for example web applications or multiuser games. For a small or short-term project, automation will not have a high return on investment and may not be worthwhile. ([View Highlight](https://read.readwise.io/read/01h0k1tcd2a8chzywvpt6wdmqs))
	- **Manual tests are a starting point**
	  
	  If you try to write automated regression tests against a feature in development, you could waste time writing against a volatile feature. Thus, you should only conduct regression testings once you have run and passed a test manually at least once. Only then can you compare the results of the manual run and the automated test. ([View Highlight](https://read.readwise.io/read/01h0k1tx62242bhcqf9chchma7))
	- **Don’t aim for 100% coverage**
	  
	  Regression testing scripts should cover 70-90% of manual tests which are effective and repeatable. 10-30% of test cases only isolate bugs once, or continuously report false negatives or positives, so they are inappropriate for regression testing. Achieving 100% regression test coverage is actually less effective and can waste test resources. ([View Highlight](https://read.readwise.io/read/01h0k1v8kt2jwymv16s0pkh7ch))
	- Smoke and sanity testing come before regression tests and can save time for testing teams. Sanity testing is a run-through of the basic functionality of an application, prior to the additional testing of a new release, which informally confirms that functionality works as planned.
	  
	  To conduct smoke testing you need a subset of test cases which test primary and core product workflows, such as startup and login, and can run very quickly. ([View Highlight](https://read.readwise.io/read/01h0k1ybb8eqyjhwrh4jcdccdw))
	- You can use sanity tests and smoke tests to quickly assess if an application is too flawed to warrant any further testing, such as regression testing. ([View Highlight](https://read.readwise.io/read/01h0k1ypg8qkyvnzkvgnnspbpf))
	- In a risk-based approach, a testing team selects test cases that cover the application areas most affected by changes in the project. They also rank them according to priority. Regression tests focus on product areas with the greatest perceived risk of quality issues. ([View Highlight](https://read.readwise.io/read/01h0k3haa8r076nj302bp0y46t))
	- Prioritize the test cases according to critical and frequently used functionalities. When you select test cases based on their priority you can reduce the regression test suite, save maintenance time and make it possible to run regression takes faster and more frequently. ([View Highlight](https://read.readwise.io/read/01h0k3hjmq1pb3nejx7xdxyxdd))