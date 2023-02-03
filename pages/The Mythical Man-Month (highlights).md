title:: The Mythical Man-Month (highlights)
author:: [[Brooks, Jr. Frederick P.]]
full-title:: "The Mythical Man-Month"
media:: #books

- Highlights first synced by [[Readwise]] [[2023-01-15]]
	- Chapter 1: The Tar Pit ([View Highlight](https://read.readwise.io/read/01gpmsd2ern34qfjkhz96vhdax))
	- Chapter 1: The Tar ([View Highlight](https://read.readwise.io/read/01gpmsdmn2yn10zc2a20ce9qt4))
	- In the upper left of [Fig. 1.1](https://readwise.io/reader/document_raw_content/26202268#filepos18361) is a program. It is complete in itself, ready to be run by the author on the system on which it was developed. That is the thing commonly produced in garages, and that is the object the individual programmer uses in estimating productivity.
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id6-00004.jpg)
	  
	  Fig. 1.1 Evolution of the programming systems product
	  
	  There are two ways a program can be converted into a more useful, but more costly, object. These two ways are represented by the boundaries in the diagram.
	  
	  Moving down across the horizontal boundary, a program becomes a programming product. This is a program that can be run, tested, repaired, and extended by anybody. It is usable in many operating environments, for many sets of data. To become a generally usable programming product, a program must be written in a generalized fashion. In particular the range and form of inputs must be generalized as much as the basic algorithm will reasonably allow. Then the program must be thoroughly tested, so that it can be depended upon. This means that a substantial bank of test cases, exploring the input range and probing its boundaries, must be prepared, run, and recorded. Finally, promotion of a program to a programming product requires its thorough documentation, so that anyone may use it, fix it, and extend it. As a rule of thumb, I estimate that a programming product costs at least three times as much as a debugged program with the same function.
	  
	  Moving across the vertical boundary, a program becomes a component in a programming system. This is a collection of interacting programs, coordinated in function and disciplined in format, so that the assemblage constitutes an entire facility for large tasks.
	  
	  To become a programming system component, a program must be written so that every input and output conforms in syntax and semantics with precisely defined interfaces. The program must also be designed so that it uses only a prescribed budget of resources—memory space, input-output devices, computer time. Finally, the program must be tested with other system components, in all expected combinations. This testing must be extensive, for the number of cases grows combinatorially. It is time-consuming, for subtle bugs arise from unexpected interactions of debugged components. A programming system component costs at least three times as much as a stand-alone program of the same function. The cost may be greater if the system has many components.
	  
	  In the lower right-hand corner of Fig. 1.1 stands the programming systems product. This differs from the simple program in all of the above ways. It costs nine times as much. But it is the truly useful object, the intended product of most system programming efforts. ([View Highlight](https://read.readwise.io/read/01gpp3k22p010bmbv6g70k6h17))
	- More software projects have gone awry for lack of calendar time than for all other causes combined. Why is this cause of disaster so common?
	  
	  First, our techniques of estimating are poorly developed. More seriously, they reflect an unvoiced assumption which is quite untrue, i.e., that all will go well.
	  
	  Second, our estimating techniques fallaciously confuse effort with progress, hiding the assumption that men and months are interchangeable.
	  
	  Third, because we are uncertain of our estimates, software managers often lack the courteous stubbornness of Antoine's chef.
	  
	  Fourth, schedule progress is poorly monitored. Techniques proven and routine in other engineering disciplines are considered radical innovations in software engineering.
	  
	  Fifth, when schedule slippage is recognized, the natural (and traditional) response is to add manpower. Like dousing a fire with gasoline, this makes matters worse, much worse. More fire requires more gasoline, and thus begins a regenerative cycle which ends in disaster. ([View Highlight](https://read.readwise.io/read/01gpq4jkv35nzx88ayqfkbh625))
	- So the first false assumption that underlies the scheduling of systems programming is that all will go well, i.e., that each task willhike only as long as it "ought" to take. ([View Highlight](https://read.readwise.io/read/01gpq4mfzxasgy561ypvzchjq3))
	- In a single task, the assumption that all will go well has a probabilistic effect on the schedule. It might indeed go as planned, for there is a probability distribution for the delay that will be encountered, and "no delay" has a finite probability. A large programming effort, however, consists of many tasks, some chained end-to-end. The probability that each will go well becomes vanishingly small. ([View Highlight](https://read.readwise.io/read/01gpq4n75q9y0e3y3f9wsw4wty))
- New highlights added [[2023-01-15]] at 8:22 PM
	- Men and months are interchangeable commodities only when a task can be partitioned among many workers with no communication among them (Fig. 2.1). This is true of reaping wheat or picking cotton; it is not even approximately true of systems programming.
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id8-00006.jpg)
	  
	  Fig. 2.1 Time versus number of workers—perfectly partitionable task
	  
	  When a task cannot be partitioned because of sequential constraints, the application of more effort has no effect on the schedule (Fig. 2.2). The bearing of a child takes nine months, no matter how many women are assigned. Many software tasks have this characteristic because of the sequential nature of debugging. ([View Highlight](https://read.readwise.io/read/01gpvzczpwp6txbsytmsae940m))
	- In tasks that can be partitioned but which require communication among the subtasks, the effort of communication must be added to the amount of work to be done. Therefore the best that can be done is somewhat poorer than an even trade of men for months (Fig. 2.3). ([View Highlight](https://read.readwise.io/read/01gpvzdbvnjg6n7f4235qdst4m))
	- The added burden of communication is made up of two parts, training and intercommunication. Each worker must be trained in the technology, the goals of the effort, the overall strategy, and the plan of work. This training cannot be partitioned, so this part of the added effort varies linearly with the number of workers.[1](https://readwise.io/reader/document_raw_content/26202268#filepos441606)
	  
	  Intercommunication is worse. If each part of the task must be separately coordinated with each other part/ the effort increases as n(n-I)/2. Three workers require three times as much pairwise intercommunication as two; four require six times as much as two. If, moreover, there need to be conferences among three, four, etc., workers to resolve things jointly, matters get worse yet. The added effort of communicating may fully counteract the division of the original task and bring us to the situation of Fig. 2.4. ([View Highlight](https://read.readwise.io/read/01gpvze4thhjb07awp9dfzbfge))
	- Since software construction is inherently a systems effort—an exercise in complex interrelationships—communication effort is great, and it quickly dominates the decrease in individual task time brought about by partitioning. Adding more men then lengthens, not shortens, the schedule. ([View Highlight](https://read.readwise.io/read/01gpvzg2f8hrtmqnw341fq17zj))
	- Systems Test
	  
	  No parts of the schedule are so thoroughly affected by sequential constraints as component debugging and system test. Furthermore, the time required depends on the number and subtlety of the errors encountered. Theoretically this number should be zero. Because of optimism, we usually expect the number of bugs to be smaller than it turns out to be. Therefore testing is usually the most mis-scheduled part of programming.
	  
	  For some years I have been successfully using the following rule of thumb for scheduling a software task:
	  
	  > l/3 planning
	  > 
	  > l/6 coding
	  > 
	  > l/4 component test and early system test
	  > 
	  > l/4 system test, all components in hand.
	  
	  This differs from conventional scheduling in several important ways:
	  
	  1.  The fraction devoted to planning is larger than normal. Even so, it is barely enough to produce a detailed and solid specification, and not enough to include research or exploration of totally new techniques.
	  2.  The half of the schedule devoted to debugging of completed code is much larger than normal.
	  3.  The part that is easy to estimate, i.e., coding, is given only one-sixth of the schedule. ([View Highlight](https://read.readwise.io/read/01gpvzh2xrv2c9w3mzap693r5b))
	- Failure to allow enough time for system test, in particular, is peculiarly disastrous. Since the delay comes at the end of the schedule, no one is aware of schedule trouble until almost the delivery date. Bad news, late and without warning, is unsettling to customers and to managers ([View Highlight](https://read.readwise.io/read/01gpvzjjnczwkqesq5npsypx89))
	- Furthermore, delay at this point has unusually severe financial, as well as psychological, repercussions. The project is fully staffed, and cost-per-day is maximum. More seriously, the software is to support other business effort (shipping of computers, operation of new facilities, etc.) and the secondary costs of delaying these are very high, for it is almost time for software shipment. Indeed, these secondary costs may far outweigh all others. It is therefore very important to allow enough system test time in the original schedule. ([View Highlight](https://read.readwise.io/read/01gpvzks8z3npaa2r0fhmf2w7t))
	- Observe that for the programmer, as for the chef, the urgency of the patron may govern the scheduled completion of the task, but it cannot govern the actual completion. An omelette, promised in two minutes, may appear to be progressing nicely. But when it has not set in two minutes, the customer has two choices—wait or eat it raw. Software customers have had the same choices.
	  
	  The cook has another choice; he can turn up the heat. The result is often an omelette nothing can save—burned in one part, raw in another.
	  
	  Now I do not think software managers have less inherent courage and firmness than chefs, nor than other engineering managers. But false scheduling to match the patron's desired date is much more common in our discipline than elsewhere in engineering. It is very difficult to make a vigorous, plausible, and job-risking defense of an estimate that is derived by no quantitative method, supported by little data, and certified chiefly by the hunches of the managers. ([View Highlight](https://read.readwise.io/read/01gpvzn33saa53tm38nzgqdzck))
	- What does one do when an essential software project is behind schedule? Add manpower, naturally. As Figs. 2.1 through 2.4 suggest, this may or may not help.
	  
	  Let us consider an example[3](https://readwise.io/reader/document_raw_content/26202268#filepos442804). Suppose a task is estimated at 12 man-months and assigned to three men for four months, and that there are measurable mileposts A, B, C, D, which are scheduled to fall at the end of each month (Fig. 2.5).
	  
	  Now suppose the first milepost is not reached until two months have elapsed (Fig. 2.6). What are the alternatives facing the manager?
	  
	  1.  Assume that the task must be done on time. Assume that only the first part of the task was misestimated, so Fig. 2.6 tells the story accurately. Then 9 man-months of effort remain, and two months, so 4 1/2 men will be needed. Add 2 men to the 3 assigned.
	  2.  Assume that the task must be done on time. Assume that the whole estimate was uniformly low, so that Fig. 2.7 really describes the situation. Then 18 man-months of effort remain, and two months, so 9 men will be needed. Add 6 men to the 3 assigned.
	    
	    ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id12-00010.jpg)
	    
	    Figure 2.5
	    
	    ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id13-00011.jpg)
	    
	    Figure 2.6
	    
	    ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id14-00012.jpg)
	    
	    Figure 2.7
	    
	  3.  Reschedule. I like the advice given by P. Fagg, an experienced hardware engineer, "Take no small slips." That is, allow enough time in the new schedule to ensure that the work can be carefully and thoroughly done, and that rescheduling will not have to be done again.
	  4.  Trim the task. In practice this tends to happen anyway, once the team observes schedule slippage. Where the secondary costs of delay are very high, this is the only feasible action.
	    
	    The manager's only alternatives are to trim it formally and carefully, to reschedule, or to watch the task get silently trimmed by hasty design and incomplete testing.
	    
	  
	  In the first two cases, insisting that the unaltered task be completed in four months is disastrous. Consider the regenerative effects, for example, for the first alternative (Fig. 2.8). The two new men, however competent and however quickly recruited, will require training in the task by one of the experienced men. If this takes a month, 3 man-months will have been devoted to work not in theoriginal estimate. Furthermore, the task, originally partitioned three ways, must be repartitioned into five parts; hence some work already done will be lost, and system testing must be lengthened. So at the end of the third month, substantially more than 7 man-months of effort remain, and 5 trained people and one month are available. As Fig. 2.8 suggests, the product is just as late as if no one had been added (Fig. 2.6).
	  
	  To hope to get done in four months, considering only training time and not repartitioning and extra systems test, would require adding 4 men, not 2, at the end of the second month. To cover repartitioning and system test effects, one would have to add still other men. Now, however, one has at least a 7-man team, not a 3-man one; thus such aspects as team organization and task division are different in kind, not merely in degree.
	  
	  Notice that by the end of the third month things look very black. The March 1 milestone has not been reached in spite of all the managerial effort. The temptation is very strong to repeat the cycle, adding yet more manpower. Therein lies madness.
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id15-00013.jpg)
	  
	  Figure 2.8
	  
	  The foregoing assumed that only the first milestone was misestimated. If on March I one makes the conservative assumption that the whole schedule was optimistic, as Fig. 2.7 depicts, one wants to add 6 men just to the original task. Calculation of the training, repartitioning, system testing effects is left as an exercise for the reader. Without a doubt, the regenerative disaster will yield a poorer product, later, than would rescheduling with the original three men, unaugmented.
	  
	  Oversimplifying outrageously, we state Brooks's Law:
	  
	  > Adding manpower to a late software project makes it later.
	  
	  This then is the demythologizing of the man-month. The number of months of a project depends upon its sequential constraints. The maximum number of men depends upon the number of independent subtasks. From these two quantities one can derive schedules using fewer men and more months. (The only risk is product obsolescence.) One cannot, however, get workable schedules using more men and fewer months. More software projects have gone awry for lack of calendar time than for all other causes combined. ([View Highlight](https://read.readwise.io/read/01gpw26n3rpx23jy4sg12rj7zb))
- New highlights added [[2023-01-15]] at 9:22 PM
	- I have earlier argued that the sheer number of minds to be coordinated affects the cost of the effort, for a major part of the cost is communication and correcting the ill effects of miscom-munication (system debugging). This, too, suggests that one wants the system to be built by as few minds as possible. Indeed, most experience with large programming systems shows that the brute-force approach is costly, slow, inefficient, and produces systems that are not conceptually integrated. OS/360, Exec 8, Scope 6600, Multics, TSS, SAGE, etc.—the list goes on and on. ([View Highlight](https://read.readwise.io/read/01gpw2v8rt1s654x0vzwqhdsaa))
	- This then is the problem with the small, sharp team concept: it is too slow for really big systems. ([View Highlight](https://read.readwise.io/read/01gpw2xg3j0ekvp0bpejrnn24b))
	- The dilemma is a cruel one. For efficiency and conceptual integrity, one prefers a few good minds doing design and construction. Yet for large systems one wants a way to bring considerable manpower to bear, so that the product can make a timely appearance. How can these two needs be reconciled? ([View Highlight](https://read.readwise.io/read/01gpw2xktrx78d7wpp7dahnybw))
	- A proposal by Harlan Mills offers a fresh and creative solution.2'3 Mills proposes that each segment of a large job be tackled by a team, but that the team be organized like a surgical team rather than a hog-butchering team. That is, instead of each member cutting away on the problem, one does the cutting and the others give him every support that will enhance his effectiveness and productivity. ([View Highlight](https://read.readwise.io/read/01gpw2y68jcgynh366jwbzay9p))
	- A little thought shows that this concept meets the desiderata, if it can be made to work. Few minds are involved in design and construction, yet many hands are brought to bear. Can it work? Who are the anesthesiologists and nurses on a programming team, and how is the work divided? Let me freely mix metaphors to suggest how such a team might work if enlarged to include all conceivable support.
	  
	  The surgeon. Mills calls him a chief programmer. He personally defines the functional and performance specifications, designs the program, codes it, tests it, and writes its documentation. He writes in a structured programming language such as PL/I, and has effective access to a computing system which not only runs his tests but also stores the various versions of his programs, allows easy file updating, and provides text editing for his documentation. He needs great talent, ten years experience, and considerable systems and application knowledge, whether in applied mathematics, business data handling, or whatever.
	  
	  The copilot. He is the alter ego of the surgeon, able to do any part of the job, but is less experienced. His main function is to share in the design as a thinkerrdiscussant, and evaluator. The surgeon tries ideas on him, but is not bound by his advice. The copilot often represents his team in discussions of function and interface with other teams. He knows all the code intimately. He researches alternative design strategies. He obviously serves as insurance against disaster to the surgeon. He may even write code, but he is not responsible for any part of the code ([View Highlight](https://read.readwise.io/read/01gpw2z5jepedxacg8qbs81eb3))
	- The administrator. The surgeon is boss, and he must have the last word on personnel, raises, space, and so on, but he must spend almost none of his time on these matters. Thus he needs a professional administrator who handles money, people, space, and machines, and who interfaces with the administrative machinery of the rest of the organization. Baker suggests that the administrator has a full-time job only if the project has substantial legal, con-tractual, reporting, or financial requirements because of the user-producer relationship. Otherwise, one administrator can serve two teams.
	  
	  The editor. The surgeon is responsible for generating the documentation—for maximum clarity he must write it. This is true of both external and internal descriptions. The editor, however, takes the draft or dictated manuscript produced by the surgeon and criticizes it, reworks it, provides it with references and bibliogra-phy, nurses it through several versions, and oversees the mechanics of production.
	  
	  Two secretaries. The administrator and the editor will each need a secretary; the administrator's secretary will handle project correspondence and non-product files.
	  
	  The program clerk. He is responsible for maintaining all the technical records of the team in a programming-product library. The clerk is trained as a secretary and has responsibility for both machine-readable and human-readable files.
	  
	  All computer input goes to the clerk, who logs and keys it if required. The output listings go back to him to be filed and indexed. The most recent runs of any model are kept in a status notebook; all previous ones are filed in a chronological archive.
	  
	  Absolutely vital to Mills's concept is the transformation of programming "from private art to public practice" by making all the computer runs visible to all team members and identifying all programs and data as team property, not private property.
	  
	  The specialized function of the program clerk relieves programmers of clerical chores, systematizes and ensures proper performance of those oft-neglected chores, and enhances the team's most valuable asset—its work-product. Clearly the concept as set forth above assumes batch runs. When interactive terminals are used, particularly those with no hard-copy output, the program clerk's functions do not diminish, but they change. Now he logs all updates of team program copies from private working copies, still handles all batch runs, and uses his own interactive facility to control the integrity and availability of the growing product ([View Highlight](https://read.readwise.io/read/01gpw3wbpnm0x52t2ewet5abn7))
	- The team just defined meets the desiderata in several ways. Ten people, seven of them professionals, are at work on the problem, but the system is the product of one mind—or at most two, acting uno animo.
	  
	  Notice in particular the differences between a team of two programmers conventionally organized and the surgeon-copilot team. First, in the conventional team the partners divide the work, and each is responsible for design and implementation of part of the work. In the surgical team, the surgeon and copilot are each cognizant of all of the design and all of the code. This saves the labor of allocating space, disk accesses, etc. It also ensures the conceptual integrity of the work.
	  
	  Second, in the conventional team the partners are equal, and the inevitable differences of judgment must be talked out or compromised. Since the work and resources are divided, the differences in judgment are confined to overall strategy and interfacing, but they are compounded by differences of interest—e.g., whose space will be used for a buffer. In the surgical team, there are no differences of interest, and differences of judgment are settled by the surgeon unilaterally. These two differences—lack of division of the problem and the superior-subordinate relationship—make it possible for the surgical team to act uno animo.
	  
	  Yet the specialization of function of the remainder of the team is the key to its efficiency, for it permits a radically simpler communication pattern among the members, as Fig. 3.1 shows. ([View Highlight](https://read.readwise.io/read/01gpw4568sqa6tkj17b9wzbr1m))
	- Even though they have not taken centuries to build, most programming systems reflect conceptual disunity far worse than that of cathedrals. Usually this arises not from a serial succession of master designers, but from the separation of design into many tasks done by many men.
	  
	  I will contend that conceptual integrity is the most important consideration in system design. It is better to have a system omit certain anomalous features and improvements, but to reflect one set of design ideas, than to have one that contains many good but independent and uncoordinated ideas ([View Highlight](https://read.readwise.io/read/01gpw5a0fcd48hzphpc3qwm10s))
	- Ease of use is enhanced only if the time gained in functional specification exceeds the time lost in learning, remembering, and searching manuals. With modern programming systems this gain does exceed the cost, but in recent years the ratio of gain to cost seems to have fallen as more and more complex functions have been added. ([View Highlight](https://read.readwise.io/read/01gpw5be7w2127kz1xbnmtqme7))
	- For a given level of function, however, that system is best in which one can specify things with the most simplicity aiid straightforwardness. Simplicity is not enough ([View Highlight](https://read.readwise.io/read/01gpw5m04byyz6c4ahjnea1vnk))
	- Simplicity and straightforwardness proceed from conceptual integrity. Every part must reflect the same philosophies and the same balancing of desiderata. Every part must even use the same techniques in syntax and analogous notions in semantics. Ease of use, then, dictates unity of design, conceptual integrity. ([View Highlight](https://read.readwise.io/read/01gpw5ms5ftkvwqfv53pzfa6xf))
	- Conceptual integrity in turn dictates that the design must proceed from one mind, or from a very small number of agreeing resonant minds.
	  
	  Schedule pressures, however, dictate that system building needs many hands. Two techniques are available for resolving this dilemma. The first is a careful division of labor between architecture and implementation. The second is the new way of structuring programming implementation teams ([View Highlight](https://read.readwise.io/read/01gpw5nj2j3c6z9vfrhj7cmq4c))
- New highlights added [[2023-01-15]] at 10:22 PM
	- The separation of architectural effort from implementation is a very powerful way of getting conceptual integrity on very large projects ([View Highlight](https://read.readwise.io/read/01gpw7cz0pb9rq6hbs5x3kn2tm))
	- The architect of a system, like the architect of a building, is the user's agent. It is his job to bring professional and technical knowledge to bear in the unalloyed interest of the user, as opposed to the interests of the salesman, the fabricator, etc.8
	  
	  Architecture must be carefully distinguished from implementation. As Blaauw has said, "Where architecture tells what happens, implementation tells how it is made to happen."3 He gives as a simple example a clock, whose architecture consists of the face, the hands, and the winding knob. When a child has learned this architecture, he can tell time as easily from a wristwatch as from a church tower. The implementation, however, and its realization, describe what goes on inside the case—powering by any of many mechanisms and accuracy control by any of many. ([View Highlight](https://read.readwise.io/read/01gpw7e2q1w2mwpynqkgtnnr4b))
	- I will certainly not contend that only the architects will have good architectural ideas. Often the fresh concept does come from an implementer or from a user. However, all my own experience convinces me, and I have tried to show, that the conceptual integrity of a system determines its ease of use. Good features and ideas that do not integrate with a system's basic concepts are best left out. If there appear many such important but incompatible ideas, one scraps the whole system and starts again on an integrated system with different basic concepts. ([View Highlight](https://read.readwise.io/read/01gpw89pwgpj3a5b39bbf2asyn))
	- Yes, in the sense that there must be few architects, their product must endure longer than that of an implementer, and the architect sits at the focus of forces which he must ultimately resolve in the user's interest. If a system is to have conceptual integrity, someone must control the concepts. That is an aristocracy that needs no apology. ([View Highlight](https://read.readwise.io/read/01gpw8aw7pccdgs3k4yv69f5cn))
- New highlights added [[2023-01-16]] at 10:49 PM
	- Regenerative Schedule Disaster
	  
	  What does one do when an essential software project is behind schedule? Add manpower, naturally. As Figs. 2.1 through 2.4 suggest, this may or may not help.
	  
	  Let us consider an example[3](https://readwise.io/reader/document_raw_content/26202268#filepos442804). Suppose a task is estimated at 12 man-months and assigned to three men for four months, and that there are measurable mileposts A, B, C, D, which are scheduled to fall at the end of each month (Fig. 2.5).
	  
	  Now suppose the first milepost is not reached until two months have elapsed (Fig. 2.6). What are the alternatives facing the manager?
	  
	  1.  Assume that the task must be done on time. Assume that only the first part of the task was misestimated, so Fig. 2.6 tells the story accurately. Then 9 man-months of effort remain, and two months, so 4 1/2 men will be needed. Add 2 men to the 3 assigned.
	  2.  Assume that the task must be done on time. Assume that the whole estimate was uniformly low, so that Fig. 2.7 really describes the situation. Then 18 man-months of effort remain, and two months, so 9 men will be needed. Add 6 men to the 3 assigned.
	    
	    ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id12-00010.jpg) ([View Highlight](https://read.readwise.io/read/01gpwef813tprx4x3k6dake2xr))
	- Regenerative Schedule Disaster
	  
	  What does one do when an essential software project is behind schedule? Add manpower, naturally. As Figs. 2.1 through 2.4 suggest, this may or may not help.
	  
	  Let us consider an example[3](https://readwise.io/reader/document_raw_content/26202268#filepos442804). Suppose a task is estimated at 12 man-months and assigned to three men for four months, and that there are measurable mileposts A, B, C, D, which are scheduled to fall at the end of each month (Fig. 2.5).
	  
	  Now suppose the first milepost is not reached until two months have elapsed (Fig. 2.6). What are the alternatives facing the manager?
	  
	  1.  Assume that the task must be done on time. Assume that only the first part of the task was misestimated, so Fig. 2.6 tells the story accurately. Then 9 man-months of effort remain, and two months, so 4 1/2 men will be needed. Add 2 men to the 3 assigned.
	  2.  Assume that the task must be done on time. Assume that the whole estimate was uniformly low, so that Fig. 2.7 really describes the situation. Then 18 man-months of effort remain, and two months, so 9 men will be needed. Add 6 men to the 3 assigned.
	    
	    ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id12-00010.jpg)
	    
	    Figure 2.5
	    
	    ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id13-00011.jpg) ([View Highlight](https://read.readwise.io/read/01gpwefmefda0z8k01tbp1aq7b))
	- 1.  Figure 2.6
	    
	    ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id14-00012.jpg)
	    
	    Figure 2.7
	    
	  2.  Reschedule. I like the advice given by P. Fagg, an experienced hardware engineer, "Take no small slips." That is, allow enough time in the new schedule to ensure that the work can be carefully and thoroughly done, and that rescheduling will not have to be done again.
	  3.  Trim the task. In practice this tends to happen anyway, once the team observes schedule slippage. Where the secondary costs of delay are very high, this is the only feasible action.
	    
	    The manager's only alternatives are to trim it formally and carefully, to reschedule, or to watch the task get silently trimmed by hasty design and incomplete testing.
	    
	  
	  In the first two cases, insisting that the unaltered task be completed in four months is disastrous. Consider the regenerative effects, for example, for the first alternative (Fig. 2.8). The two new men, however competent and however quickly recruited, will require training in the task by one of the experienced men. If this takes a month, 3 man-months will have been devoted to work not in theoriginal estimate. Furthermore, the task, originally partitioned three ways, must be repartitioned into five parts; hence some work already done will be lost, and system testing must be lengthened. So at the end of the third month, substantially more than 7 man-months of effort remain, and 5 trained people and one month are available. As Fig. 2.8 suggests, the product is just as late as if no one had been added (Fig. 2.6).
	  
	  To hope to get done in four months, considering only training time and not repartitioning and extra systems test, would require adding 4 men, not 2, at the end of the second month. To cover repartitioning and system test effects, one would have to add still other men. Now, however, one has at least a 7-man team, not a 3-man one; thus such aspects as team organization and task division are different in kind, not merely in degree.
	  
	  Notice that by the end of the third month things look very black. The March 1 milestone has not been reached in spite of all the managerial effort. The temptation is very strong to repeat the cycle, adding yet more manpower. Therein lies madness.
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id15-00013.jpg)
	  
	  Figure 2.8
	  
	  The foregoing assumed that only the first milestone was misestimated. If on March I one makes the conservative assumption that the whole schedule was optimistic, as Fig. 2.7 depicts, one wants to add 6 men just to the original task. Calculation of the training, repartitioning, system testing effects is left as an exercise for the reader. Without a doubt, the regenerative disaster will yield a poorer product, later, than would rescheduling with the original three men, unaugmented.
	  
	  Oversimplifying outrageously, we state Brooks's Law:
	  
	  > Adding manpower to a late ([View Highlight](https://read.readwise.io/read/01gpweh6cwvjcmex5596tt0tet))
	- ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id14-00012.jpg) ([View Highlight](https://read.readwise.io/read/01gpwefs7fmf9r8h9exshqa8bx))
	- ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id14-00012.jpg) ([View Highlight](https://read.readwise.io/read/01gpwegtez5w6mbhp64xqgfs1q))
	- > software project makes it later.
	  
	  This then is the demythologizing of the man-month. The number of months of a project depends upon its sequential constraints. The maximum number of men depends upon the number of independent subtasks. From these two quantities one can derive schedules using fewer men and more months. (The only risk is product obsolescence.) One cannot, however, get workable schedules using more men and fewer months. More software projects have gone awry for lack of calendar time than for all other causes combined. ([View Highlight](https://read.readwise.io/read/01gpwehee5re9myk021ed1z9jn))
	- The Problem
	  
	  Programming managers have long recognized wide productivity variations between good programmers and poor ones. But the actual measured magnitudes have astounded all of us. In one of their studies, Sackman, Erikson, and Grant were measuring performances of a group of experienced programmers. Within just this group the ratios between best and worst performances averaged about 10:1 on productivity measurements and an amazing 5:1 on program speed and space measurements! In short the $20,000/year programmer may well be 10 times as productive as the $10,000/year one. The converse may be true, too. The data showed no correlation whatsoever between experience and performance. (I doubt if that is universally true.)
	  
	  I have earlier argued that the sheer number of minds to be coordinated affects the cost of the effort, for a major part of the cost is communication and correcting the ill effects of miscom-munication (system debugging). This, too, suggests that one wants the system to be built by as few minds as possible. Indeed, most experience with large programming systems shows that the brute-force approach is costly, slow, inefficient, and produces systems that are not conceptually integrated. OS/360, Exec 8, Scope 6600, Multics, TSS, SAGE, etc.—the list goes on and on. ([View Highlight](https://read.readwise.io/read/01gpwej7ghgccc37hhb9dx77yp))
	- This then is the problem with the small, sharp team concept: it is too slow for really big systems ([View Highlight](https://read.readwise.io/read/01gpwejrffxdrbfcnye1pte8ww))
	- For efficiency and conceptual integrity, one prefers a few good minds doing design and construction. Yet for large systems one wants a way to bring considerable manpower to bear, so that the product can make a timely appearance. How can these two needs be reconciled? ([View Highlight](https://read.readwise.io/read/01gpwek0ys6kdtrqnsbcrxm277))
	- Mills's Proposal
	  
	  A proposal by Harlan Mills offers a fresh and creative solution.2'3 Mills proposes that each segment of a large job be tackled by a team, but that the team be organized like a surgical team rather than a hog-butchering team. That is, instead of each member cutting away on the problem, one does the cutting and the others give him every support that will enhance his effectiveness and productivity.
	  
	  A little thought shows that this concept meets the desiderata, if it can be made to work. Few minds are involved in design and construction, yet many hands are brought to bear. Can it work? Who are the anesthesiologists and nurses on a programming team, and how is the work divided? Let me freely mix metaphors to suggest how such a team might work if enlarged to include all conceivable support.
	  
	  The surgeon. Mills calls him a chief programmer. He personally defines the functional and performance specifications, designs the program, codes it, tests it, and writes its documentation. He writes in a structured programming language such as PL/I, and has effective access to a computing system which not only runs his tests but also stores the various versions of his programs, allows easy file updating, and provides text editing for his documentation. He needs great talent, ten years experience, and considerable systems and application knowledge, whether in applied mathematics, business data handling, or whatever.
	  
	  The copilot. He is the alter ego of the surgeon, able to do any part of the job, but is less experienced. His main function is to share in the design as a thinkerrdiscussant, and evaluator. The surgeon tries ideas on him, but is not bound by his advice. The copilot often represents his team in discussions of function and interface with other teams. He knows all the code intimately. He researches alternative design strategies. He obviously serves as insurance against disaster to the surgeon. He may even write code, but he is not responsible for any part of the code.
	  
	  The administrator. The surgeon is boss, and he must have the last word on personnel, raises, space, and so on, but he must spend almost none of his time on these matters. Thus he needs a professional administrator who handles money, people, space, and machines, and who interfaces with the administrative machinery of the rest of the organization. Baker suggests that the administrator has a full-time job only if the project has substantial legal, con-tractual, reporting, or financial requirements because of the user-producer relationship. Otherwise, one administrator can serve two teams.
	  
	  The editor. The surgeon is responsible for generating the documentation—for maximum clarity he must write it. This is true of both external and internal descriptions. The editor, however, takes the draft or dictated manuscript produced by the surgeon and criticizes it, reworks it, provides it with references and bibliogra-phy, nurses it through several versions, and oversees the mechanics of production.
	  
	  Two secretaries. The administrator and the editor will each need a secretary; the administrator's secretary will handle project correspondence and non-product files.
	  
	  The program clerk. He is responsible for maintaining all the technical records of the team in a programming-product library. The clerk is trained as a secretary and has responsibility for both machine-readable and human-readable files.
	  
	  All computer input goes to the clerk, who logs and keys it if required. The output listings go back to him to be filed and indexed. The most recent runs of any model are kept in a status notebook; all previous ones are filed in a chronological archive.
	  
	  Absolutely vital to Mills's concept is the transformation of programming "from private art to public practice" by making all the computer runs visible to all team members and identifying all programs and data as team property, not private property.
	  
	  The specialized function of the program clerk relieves programmers of clerical chores, systematizes and ensures proper performance of those oft-neglected chores, and enhances the team's most valuable asset—its work-product. Clearly the concept as set forth above assumes batch runs. When interactive terminals are used, particularly those with no hard-copy output, the program clerk's functions do not diminish, but they change. Now he logs all updates of team program copies from private working copies, still handles all batch runs, and uses his own interactive facility to control the integrity and availability of the growing product.
	  
	  The toolsmith. File-editing, text-editing, and interactive debugging services are now readily available, so that a team will rarely need its own machine and machine-operating crew. But these services must be available with unquestionably satisfactory response and reliability; and the surgeon must be sole judge of the adequacy of the service available to him. He needs a toolsmith, responsible for ensuring this adequacy of the basic service and for constructing, maintaining, and upgrading special tools—mostly interactive computer services—needed by his team. Each team will need its own toolsmith, regardless of the excellence and reliability of any centrally provided service, for his job is to see to the tools needed or wanted by his surgeon, without regard to any other team's needs. The tool-builder will often construct specialized utilities, catalogued procedures, macro libraries.
	  
	  The tester. The surgeon will need a bank of suitable test cases for testing pieces of his work as he writes it, and then for testing the whole thing. The tester is therefore both an adversary who devises system test cases from the functional specs, and an assistant who devises test data for the day-by-day debugging. He would also plan testing sequences and set up the scaffolding required for component tests.
	  
	  The language lawyer. By the time Algol came along, people began to recognize that most computer installations have one or two people who delight in mastery of the intricacies of a programming language. And these experts turn out to be very useful and very widely consulted. The talent here is rather different from that of the surgeon, who is primarily a system designer and who thinks representations. The language lawyer can find a neat and efficient way to use the language to do difficult, obscure, or tricky things. Often he will need to do small studies (two or three days) on good technique. One language lawyer can service two or three surgeons.
	  
	  This, then, is how 10 people might contribute in well-differentiated and specialized roles on a programming team built on the surgical model. ([View Highlight](https://read.readwise.io/read/01gpwekscqvxg29p3jb4j7c0bn))
	- The team just defined meets the desiderata in several ways. Ten people, seven of them professionals, are at work on the problem, but the system is the product of one mind—or at most two, acting uno animo. ([View Highlight](https://read.readwise.io/read/01gpwemagq72ma0a90r5zwsxkf))
	- Even though they have not taken centuries to build, most programming systems reflect conceptual disunity far worse than that of cathedrals. Usually this arises not from a serial succession of master designers, but from the separation of design into many tasks done by many men ([View Highlight](https://read.readwise.io/read/01gpwesfvfq3w4r4t76bx9rfjj))
	- I will contend that conceptual integrity is the most important consideration in system design. It is better to have a system omit certain anomalous features and improvements, but to reflect one set of design ideas, than to have one that contains many good but independent and uncoordinated ideas. In this chapter and the next two, we will examine the consequences of this theme for programming system design:
	  
	  •   How is conceptual integrity to be achieved?
	  •   Does not this argument imply an elite, or aristocracy of architects, and a horde of plebeian implementers whose creative talents and ideas are suppressed?
	  •   How does one keep the architects from drifting off into the blue with unimplementable or costly specifications?
	  •   How does one ensure that every trifling detail of an architectural specification gets communicated to the implementer, properly understood by him, and accurately incorporated into the product? ([View Highlight](https://read.readwise.io/read/01gpwerzb894ngxy1z1w9wv10x))
	- The purpose of a programming system is to make a computer easy to use. To do this, it furnishes languages and various facilities that are in fact programs invoked and controlled by language features. But these facilities are bought at a price: the external description of a programming system is ten to twenty times as large as the external description of the computer system itself. The user finds it far easier to specify any particular function, but there are far more to choose from, and far more options and formats to remember ([View Highlight](https://read.readwise.io/read/01gpwestxr76ky84n0zmtyykhn))
	- Because ease of use is the purpose, this ratio of function to conceptual complexity is the ultimate test of system design. Neither function alone nor simplicity alone defines a good design. ([View Highlight](https://read.readwise.io/read/01gpwet2faf7rsps08kq5tv5nk))
	- Conceptual integrity in turn dictates that the design must proceed from one mind, or from a very small number of agreeing resonant minds.
	  
	  Schedule pressures, however, dictate that system building needs many hands. Two techniques are available for resolving this dilemma. The first is a careful division of labor between architecture and implementation. The second is the new way of structuring programming implementation ([View Highlight](https://read.readwise.io/read/01gpwf3jbgkmwk313f1zkhhmym))
	- The separation of architectural effort from implementation is a very powerful way of getting conceptual integrity on very large projects. I myself have seen it used with great success on IBM's Stretch computer and on the System/360 computer product line. I have seen it fail through lack of application on Operating System/360. ([View Highlight](https://read.readwise.io/read/01gpwf3w44a3kmxtcc36b8arf3))
	- By the architecture of a system, I mean the complete and detailed specification of the user interface. For a computer this is the programming manual. For a compiler it is the language manual. For a control program it is the manuals for the language or languages used to invoke its functions. For the entire system it is the union of the manuals the user must consult to do his entire job.
	  
	  The architect of a system, like the architect of a building, is the user's agent. It is his job to bring professional and technical knowledge to bear in the unalloyed interest of the user, as opposed to the interests of the salesman, the fabricator, etc.8
	  
	  Architecture must be carefully distinguished from implementation. As Blaauw has said, "Where architecture tells what happens, implementation tells how it is made to happen."3 He gives as a simple example a clock, whose architecture consists of the face, the hands, and the winding knob. When a child has learned this architecture, he can tell time as easily from a wristwatch as from a church tower. The implementation, however, and its realization, describe what goes on inside the case—powering by any of many mechanisms and accuracy control by any of many. ([View Highlight](https://read.readwise.io/read/01gpwf4xjws091920ncq8kx6c3))
	- In System/360, for example, a single computer architecture is implemented quite differently in each of some nine models. Conversely, a single implementation, the Model 30 data flow, memory, and microcode, serves at different times for four different architectures: a System/360 computer, a multiplex channel with up to 224 logically independent subchannels, a selector channel, and a 1401 computer.4 ([View Highlight](https://read.readwise.io/read/01gpwf57gbz7k1mtm7pzzfh9nh))
	- Often the fresh concept does come from an implementer or from a user. However, all my own experience convinces me, and I have tried to show, that the conceptual integrity of a system determines its ease of use. Good features and ideas that do not integrate with a system's basic concepts are best left out. If there appear many such important but incompatible ideas, one scraps the whole system and starts again on an integrated system with different basic concepts.
	  
	  As to the aristocracy charge, the answer must be yes and no. Yes, in the sense that there must be few architects, their product must endure longer than that of an implementer, and the architect sits at the focus of forces which he must ultimately resolve in the user's interest. If a system is to have conceptual integrity, someone must control the concepts. That is an aristocracy that needs no apology.
	  
	  No, because the setting of external specifications is not more creative work than the designing of implementations. It is just different creative work. The design of an implementation, given an architecture, requires and allows as much design creativity, as many new ideas, and as much technical brilliance as the design of the external specifications. Indeed, the cost-performance ratio of the product will depend most heavily on the implementer, just as ease of use depends most heavily on the architect ([View Highlight](https://read.readwise.io/read/01gpwf6gy17b5hcb71sn8vk77b))
	- There are many examples from other arts and crafts that lead one to believe that discipline is good for art. Indeed, an artist's aphorism asserts, "Form is liberating." The worst buildings are those whose budget was too great for the purposes to be served. Bach's creative output hardly seems to have been squelched by the necessity of producing a limited-form cantata each week. I am sure that the Stretch computer would have had a better architecture had it been more tightly constrained; the constraints imposed by the System/360 Model 30's budget were in my opinion entirely beneficial for the Model 75's architecture. ([View Highlight](https://read.readwise.io/read/01gpwf7jd1chyp7x0h76r8dsck))
	- Similarly, I observe that the external provision of an architecture enhances, not cramps, the creative style of an implementing group. They focus at once on the part of the problem no one has addressed, and inventions begin to flow ([View Highlight](https://read.readwise.io/read/01gpwf8d4g1dftjd3jp5k2bgmx))
	- Many factors, of course, entered into that mistaken decision; but the overwhelming one was schedule time and the appeal of putting all those 150 implementers to work. It is this siren song whose deadly hazards I would now make visible.
	  
	  When it is proposed that a small architecture team in fact write all the external specifications for a computer or a programming system, the implementers raise three objections:
	  
	  •   The specifications will be too rich in function and will not reflect practical cost considerations.
	  •   The architects will get all the creative fun and shut out the inventiveness of the implementers.
	  •   The many implementers will have to sit idly by while the specifications come through the narrow funnel that is the architecture team.
	  
	  The first of these is a real danger, and it will be treated in the [next chapter](https://readwise.io/reader/document_raw_content/26202268#filepos75990). The other two are illusions, pure and simple. As we have seen above, implementation is also a creative activity of the first order. The opportunity to be creative and inventive in implementation is not significantly diminished by working within a given external specification, and the order of creativity may even be enhanced by that discipline. The total product will surely be.
	  
	  The last objection is one of timing and phasing. A quick answer is to refrain from hiring implementers until the specifications are complete. This is what is done when a building is constructed.
	  
	  In the computer systems business, however, the pace is quicker, and one wants to compress the schedule as much as possible. How much can specification and building be overlapped?
	  
	  As Blaauw points out, the total creative effort involves three distinct phases: architecture, implementation, and realization. It turns out that these can in fact be begun in parallel and proceed simultaneously.
	  
	  In computer design, for example, the implementer can start as soon as he has relatively vague assumptions about the manual, somewhat clearer ideas about the technology, and well-defined cost and performance objectives. He can begin designing data flows, control sequences, gross packaging concepts, and so on. He devises or adapts the tools he will need, especially the record-keeping system, including the design automation system.
	  
	  Meanwhile, at the realization level, circuits, cards, cables, frames, power supplies, and memories must each be designed, refined, and documented. This work proceeds in parallel with architecture and implementation.
	  
	  The same thing is true in programming system design. Long before the external specifications are complete, the implementer has plenty to do. Given some rough approximations as to the function of the system that will be ultimately embodied in the external specifications, he can proceed. He must have well-defined space and time objectives. He must know the system configuration on which his product must run. Then he can begin designing module boundaries, table structures, pass or phase breakdowns, algorithms, and all kinds of tools. Some time, too, must be spent in communicating with the architect. ([View Highlight](https://read.readwise.io/read/01gpwffs1pc858jc5xyqq7b7m4))
	- Conceptual integrity does require that a system reflect a single philosophy and that the specification as seen by the user flow from a few minds. Because of the real division of labor into architecture, implementation, and realization, however, this does not imply that a system so designed will take longer to build. Experience shows the opposite, that the integral system goes together faster and takes less time to test. In effect, a widespread horizontal division of labor has been sharply reduced by a vertical division of labor, and the result is radically simplified communications and improved conceptual integrity. ([View Highlight](https://read.readwise.io/read/01gpwfja8tcmmwcfq878cb6sxw))
	- The architect has two possible answers when confronted with an estimate that is too high: cut the design or challenge the estimate by suggesting cheaper implementations. This latter is inherently an emotion-generating activity. The architect is now challenging the builder's way of doing the builder's job. For it to be successful, the architect must
	  
	  •   remember that the builder has the inventive and creative responsibility for the implementation; so the architect suggests, not dictates;
	  •   always be prepared to suggest a way of implementing anything he specifies, and be prepared to accept any other way that meets the objectives as well;
	  •   deal quietly and privately in such suggestions;
	  •   be ready to forego credit for suggested improvements.
	  
	  Normally the builder will counter by suggesting changes to the architecture. Often he is right—some minor feature may have unexpectedly large costs when the implementation is worked out. ([View Highlight](https://read.readwise.io/read/01gpwfm1fx5m5c8cxmnkt6tr58))
	- Self-Discipline—The Second-System Effect
	  
	  An architect's first work is apt to be spare and clean. He knows he doesn't know what he's doing, so he does it carefully and with great restraint.
	  
	  As he designs the first work, frill after frill and embellishment after embellishment occur to him. These get stored away to be used "next time." Sooner or later the first system is finished, and the architect, with firm, confidence and a demonstrated mastery of that class of systems, is ready to build a second system.
	  
	  This second is the most dangerous system a man ever designs. When he does his third and later ones, his prior experiences will confirm each other as to the general characteristics of such systems, and their differences will identify those parts of his experience that are particular and not generalizable.
	  
	  The general tendency is to over-design the second system, using all the ideas and frills that were cautiously sidetracked on the first one. The result, as Ovid says, is a "big pile." For example, consider the IBM 709 architecture, later embodied in the 7090. This is an upgrade, a second system for the very successful and clean 704. The operation set is so rich and profuse that only about half of it was regularly used ([View Highlight](https://read.readwise.io/read/01gpwfvdxcbpfsbnjazz32a03s))
	- The second-system effect has another manifestation somewhat different from pure functional embellishment. That is a tendency to refine techniques whose very existence has been made obsolete by changes in basic system assumptions. OS/360 has many examples of this. ([View Highlight](https://read.readwise.io/read/01gpwfvy2h8854hkh6e0c3b84j))
	- How does the architect avoid the second-system effect? Well, obviously he can't skip his second system. But he can be conscious of the peculiar hazards of that system, and exert extra self-discipline to avoid functional ornamentation and to avoid extrapolation of functions that are obviated by changes in assumptions and purposes.
	  
	  A discipline that will open an architect's eyes is to assign each little function a value: capability x is worth not more than m bytes of memory and n microseconds per invocation. These values will guide initial decisions and serve during implementation as a guide and warning to all.
	  
	  How does the project manager avoid the second-system effect? By insisting on a senior architect who has at least two systems under his belt. Too, by staying aware of the special temptations, he can ask the right questions to ensure that the philosophical concepts and objectives are fully reflected in the detailed design ([View Highlight](https://read.readwise.io/read/01gpwft9928gema1939nw943sb))
- New highlights added [[2023-01-16]] at 11:48 PM
	- Written Specifications—the Manual
	  
	  The manual, or written specification, is a necessary tool, though not a sufficient one. The manual is the external specification of the product. It describes and prescribes every detail of what the user sees. As such, it is the chief product of the architect. ([View Highlight](https://read.readwise.io/read/01gpy64t1bq80v3jeb195jtxd5))
	- For the sake of implementers it is important that the changes be quantized—that there be dated versions appearing on a schedule. ([View Highlight](https://read.readwise.io/read/01gpy6577gw2pajc61nw82a0r5))
	- The manual must not only describe everything the user does see, including all interfaces; it must also refrain from describing what the user does not see. That is the implementer's business, and there his design freedom must be unconstrained. The architect must always be prepared to show an implementation for any feature he describes, but he must not attempt to dictate the implementation.
	  
	  The style must be precise, full, and accurately detailed. A user will often refer to a single definition, so each one must repeat all the essentials and yet all must agree. This tends to make manuals dull reading, but precision is more important than liveliness. ([View Highlight](https://read.readwise.io/read/01gpy65ptr3mm8tvhp8g0zha18))
	- The unity of System/360's Principles of Operation springs from the fact that only two pens wrote it: Gerry Blaauw's and Andris Padegs'. The ideas are those of about ten men, but the casting of those decisions into prose specifications must be done by only one or two, if the consistency of prose and product is to be maintained. For the writing of a definition will necessitate a host of mini-decisions which are not of full-debate importance. An example in System/360 is the detail of how the Condition Code is set after each operation. Not trivial, however, is the principle that such mini-decisions be made consistently throughout ([View Highlight](https://read.readwise.io/read/01gpy66847mm4s2mn5thn2rsan))
	- Let us examine the merits and weaknesses of formal definitions. As noted, formal definitions are precise. They tend to be complete; gaps show more conspicuously, so they are filled sooner. What they lack is comprehensibility. With English prose one can show structural principles, delineate structure in stages or levels, and give examples. One can readily mark exceptions and emphasize contrasts. Most important, one can explain why. The formal definitions put forward so far have inspired wonder at their elegance and confidence in their precision. But they have demanded prose explanations to make their content easy to learn and teach. For these reasons, I think we will see future specifications to consist of both a formal definition and a prose definition.
	  
	  An ancient adage warns, "Never go to sea with two chronometers; take one or three." The same thing clearly applies to prose and formal definitions. If one has both, one must be the standard, and the other must be a derivative description, clearly labeled as such. Either can be the primary standard. Algol 68 has a formal definition as standard and a prose definition as descriptive. PL/I has the prose as standard and the formal description as derivative. System/360 also has prose as standard with a derived formal description. ([View Highlight](https://read.readwise.io/read/01gpy69zk7n9kenkdy5vnd9vhh))
	- Many tools are available for formal definition. The Backus-Naur Form is familiar for language definition, and it is amply discussed in the literature.2 The formal description of PL/I uses new notions of abstract syntax, and it is adequately described.3 Iverson's APL has been used to describe machines, most notably the IBM 70904 and System/360.5
	  
	  Bell and Newell have proposed new notations for describing both configurations and machine architectures, and they have illustrated these with several machines, including the DEC PDP-8,6 the 7090,6 and System/360.7 ([View Highlight](https://read.readwise.io/read/01gpy6ag64snm8pf90f0y3q6n9))
	- Needless to say, meetings are necessary. The hundreds of man-to-man consultations must be supplemented by larger and more formal gatherings. We found two levels of these to be useful. The first is a weekly half-day conference of all the architects, plus official representatives of the hardware and software implementers, and the market planners. The chief system architect presides.
	  
	  Anyone can propose problems or changes, but proposals are usually distributed in writing before the meeting. A new problem is usually discussed a while. The emphasis is on creativity, rather than merely decision. The group attempts to invent many solutions to problems, then a few solutions are passed to one or more of the architects for detailing into precisely worded manual change proposals.
	  
	  Detailed change proposals then come up for decisions. These have been circulated and carefully considered by implementers and users, and the pros and cons are well delineated. If a consensus emerges, well and good. If not, the chief architect decides. Minutes are kept and decisions are formally, promptly, and widely disseminated.
	  
	  Decisions from the weekly conferences give quick results and allow work to proceed. If anyone is too unhappy, instant appeals to the project manager are possible, but this happens very rarely.
	  
	  The fruitfulness of these meetings springs from several sources:
	  
	  1.  The same group—architects, users, and implementers—meets weekly for months. No time is needed for bringing people up to date.
	  2.  The group is bright, resourceful, well versed in the issues, and deeply involved in the outcome. No one has an "advisory" role. Everyone is authorized to make binding commitments.
	  3.  When problems are raised, solutions are sought both within and outside the obvious boundaries.
	  4.  The formality of written proposals focuses attention, forces decision, and avoids committee-drafted inconsistencies.
	  5.  The clear vesting of decision-making power in the chief architect avoids compromise and delay. ([View Highlight](https://read.readwise.io/read/01gpy6d4d1fre7b998hxtcpm50))
	- time goes by, some decisions don't wear well. Some minor matters have never been wholeheartedly accepted by one or another of the participants. Other decisions have developed unforeseen problems, and sometimes the weekly meeting didn't agree to reconsider these. So there builds up a backlog of minor appeals, open issues, or disgruntlements. To settle these we held annual supreme court sessions, lasting typically two weeks. (I would hold them every six months if I were doing it again.) ([View Highlight](https://read.readwise.io/read/01gpy6n6k4crj5q1e743vh4dm6))
	- These sessions were held just before major freeze dates for the manual. Those present included not only the architecture group and the programmers' and implementers' architectural representatives, but also the managers of programming, marketing, and implementation efforts. The System/360 project manager presided. The agenda typically consisted of about 200 items, mostly minor, which were enumerated in charts placarded around the room. All sides were heard and decisions made. By the miracle of computerized text editing (and lots of fine staff work), each participant found an updated manual, embodying yesterday's decisions, at his seat every morning ([View Highlight](https://read.readwise.io/read/01gpy6nk19dfc7xz6z5sf2ryd3))
	- Communication in the Large Programming Project
	  
	  So it is today. Schedule disaster, functional misfits, and system bugs all arise because the left hand doesn't know what the right hand is doing. As work proceeds, the several teams slowly change the functions, sizes, and speeds of their own programs, and they explicitly or implicitly change their assumptions about the inputs available and the uses to be made of the outputs.
	  
	  For example, the implementer of a program-overlaying function may run into problems and reduce speed relying on statistics that show how rarely this function will arise in application programs. Meanwhile, back at the ranch, his neighbor may be designing a major part of the supervisor so that it critically depends upon the speed of this function. This change in speed itself becomes a major specification change, and it needs to be proclaimed abroad and weighed from a system point of view.
	  
	  How, then, shall teams communicate with one another? In as many ways as possible.
	  
	  •   Informally. Good telephone service and a clear definition of intergroup dependencies will encourage the hundreds of calls upon which common interpretation of written documents depends.
	  •   Meetings. Regular project meetings, with one team after another giving technical briefings, are invaluable. Hundreds of minor misunderstandings get smoked out this way.
	  •   Workbook. A formal project workbook must be started at the beginning. This deserves a section by itself. ([View Highlight](https://read.readwise.io/read/01gpy6tjvzhydx0kjq8hfr2tw1))
	- The Project Workbook
	  
	  What. The project workbook is not so much a separate document as it is a structure imposed on the documents that the project will be producing anyway.
	  
	  All the documents of the project need to be part of this structure. This includes objectives, external specifications, interface specifications, technical standards, internal specifications, and administrative memoranda. ([View Highlight](https://read.readwise.io/read/01gpy6yz2af4rc5sdn4kpzyq5w))
	- Why. Technical prose is almost immortal. If one examines the genealogy of a customer manual for a piece of hardware or software, one can trace not only the ideas, but also many of the very sentences and paragraphs back to the first memoranda proposing the product or explaining the first design. For the technical writer, the paste-pot is as mighty as the pen.
	  
	  Since this is so, and since tomorrow's product-quality manuals will grow from today's memos, it is very important to get the structure of the documentation right. The early design of the project workbook ensures that the documentation structure itself is crafted, not haphazard. Moreover, the establishment of a structure molds later writing into segments that fit into that structure.
	  
	  The second reason for the project workbook is control of the distribution of information. The problem is not to restrict information, but to ensure that relevant information gets to all the people who need it. ([View Highlight](https://read.readwise.io/read/01gpy6zhf44bphk613an2sxegh))
	- The first step is to number all memoranda, so that ordered lists of titles are available and each worker can see if he has what he wants. The organization of the workbook goes well beyond this to establish a tree-structure of memoranda. The tree-structure allows distribution lists to be maintained by subtree, if that is desirable ([View Highlight](https://read.readwise.io/read/01gpy702xrgr5y822yf71733hz))
	- Of critical importance is timely updating. The workbook must be current. This is very difficult to do if whole documents must be retyped for changes. In a looseleaf book, however, only pages need to be changed. We had available a computer-driven text-editing system, and this proved invaluable for timely maintenance. Offset masters were prepared directly on the computer printer, and turnaround time was less than a day. The recipient of all these updated pages has an assimilation problem, however. When he first receives a changed page, he wants to know, "What has been changed?" When he later consults it, he wants to know, "What is the definition today?" ([View Highlight](https://read.readwise.io/read/01gpy73kg07q7x3nrm200xww6k))
	- The latter need is met by the continually maintained document. Highlighting of changes requires other steps. First, one must mark changed text on the page, e.g., by a vertical bar in the margin alongside every altered line. Second, one needs to distribute with the new pages a short, separately written change summary that lists the changes and remarks on their significance. ([View Highlight](https://read.readwise.io/read/01gpy76r6gjsgtsdp44x2qp80s))
	- Let us consider a tree-like programming organization, and examine the essentials which any subtree must have in order to be effective. They are:
	  
	  1.  a mission
	  2.  a producer
	  3.  a technical director or architect
	  4.  a schedule
	  5.  a division of labor
	  6.  interface definitions among the parts ([View Highlight](https://read.readwise.io/read/01gpy7a3gyhdx7twqqsq9g3yp5))
	- What is the role of the producer? He assembles the team, divides the work, and establishes the schedule. He acquires and keeps on acquiring the necessary resources. This means that a major part of his role is communication outside the team, upwards and sideways. He establishes the pattern of communication and reporting within the team. Finally, he ensures that the schedule is met, shifting resources and organization to respond to changing circumstances. ([View Highlight](https://read.readwise.io/read/01gpy7af4pwnryfhymzpa7r6bv))
	- How about the technical director? He conceives of the design to be built, identifies its subparts, specifies how it will look from outside, and sketches its internal structure. He provides unity and conceptual integrity to the whole design; thus he serves as a limit on system complexity. As individual technical problems arise, he invents solutions for them or shifts the system design as required. He is, in Al Capp's lovely phrase, "inside-man at the skunk works." His communications are chiefly within the team. His work is almost completely technical. ([View Highlight](https://read.readwise.io/read/01gpy7ajvycrx1tffps35r06x3))
	- Now it is clear that the talents required for these two roles are quite different. Talents come in many different combinations; and the particular combination embodied in the producer and the director must govern the relationship between them. Organizations must be designed around the people available; not people fitted into pure-theory organizations.
	  
	  Three relationships are possible, and all three are found in successful practice.
	  
	  The producer and the technical director may be the same man. This is readily workable on very small teams, perhaps three to six programmers. On larger projects it is very rarely workable, for two reasons. First, the man with strong management talent and strong technical talent is rarely found. Thinkers are rare; doers are rarer; and thinker-doers are rarest. ([View Highlight](https://read.readwise.io/read/01gpy7cejty2s04mb8jj1d88v5))
	- Second, on the larger project each of the roles is necessarily a full-time job, or more. It is hard for the producer to delegate enough of his duties to give him any technical time. It is impossible for the director to delegate his without compromising the conceptual integrity of the design. ([View Highlight](https://read.readwise.io/read/01gpy7cms032vm54fw1p7kc8w1))
	- Documents for a Computer Product
	  
	  Suppose one is building a machine. What are the critical documents?
	  
	  Objectives. This defines the need to be met and the goals, desiderata, constraints, and priorities.
	  
	  Specifications. This is a computer manual plus performance specifications. It is one of the first documents generated in proposing a new product, and the last document finished.
	  
	  Schedule
	  
	  Budget. Not merely a constraint, the budget is one of the manager's most useful documents. Existence of the budget forces technical decisions that otherwise would be avoided; and, more important, it forces and clarifies policy decisions.
	  
	  Organization chart
	  
	  Space allocations
	  
	  Estimate, forecast, prices. These three have cyclic Interlocking, which determines the success or failure of the project:
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id27-00025.jpg)
	  
	  To generate a market forecast, one needs performance specifications and postulated prices. The quantities from the forecast combine with component counts from the design to determine the manufacturing cost estimate, and they determine the per-unit share of development and fixed costs. These costs in turn determine prices.
	  
	  If the prices are below those postulated, a joyous success spiral begins. Forecasts rise, unit costs drop, and prices drop yet further.
	  
	  If the prices are above those postulated, a disastrous spiral begins, and all hands must struggle to break it. Performance must be squeezed up and new applications developed to support larger forecasts. Costs must be squeezed down to yield lower estimates. The stress of this cycle is a discipline that often evokes the best work of marketer and engineer.
	  
	  It can also bring about ridiculous vacillation. I recall a machine whose instruction counter popped in or out of memory every six months during a three-year development cycle. At one phase a little more performance would be wanted, so the instruction counter was implemented in transistors. At the next phase cost reduction was the theme, so the counter would be implemented as a memory location. On another project the best engineering manager I ever saw served often as a giant flywheel, his inertia damping the fluctuations that came from market and management people ([View Highlight](https://read.readwise.io/read/01gpy7x6gcagxydxwgfeczn7q7))
	- Why Have Formal Documents?
	  
	  First, writing the decisions down is essential. Only when one writes do the gaps appear and the inconsistencies protrude. The act of writing turns out to require hundreds of mini-decisions, and it is the existence of these that distinguishes clear, exact policies from fuzzy ones.
	  
	  Second, the documents will communicate the decisions to others. The manager will be continually amazed that policies he took for common knowledge are totally unknown by some member of his team. Since his fundamental job is to keep everybody going in the same direction, his chief daily task will be communication, not decision-making, and his documents will immensely lighten this load.
	  
	  Finally, a manager's documents give him a data base and checklist. By reviewing them periodically he sees where he is, and he sees what changes of emphasis or shifts in direction are needed ([View Highlight](https://read.readwise.io/read/01gpy7yj9s7b5havqbrc1337qx))
	- Chemical engineers learned long ago that a process that works in the laboratory cannot be implemented in a factory in only one step. An intermediate step called the pilot plant is necessary to give experience in scaling quantities up and in operating in nonprotective environments. For example, a laboratory process for desalting water will be tested in a pilot plant of 10,000 gallon/day capacity before being used for a 2,000,000 gallon/day community water system.
	  
	  Programming system builders have also been exposed to this lesson, but it seems to have not yet been learned. Project after project designs a set of algorithms and then plunges into construction of customer-deliverable software on a schedule that demands delivery of the first thing built. ([View Highlight](https://read.readwise.io/read/01gpy8b6fvjgfpfeced2rfamj9))
	- In most projects, the first system built is barely usable. It may be too slow, too big, awkward to use, or all three. There is no alternative but to start again, smarting but smarter, and build a redesigned version in which these problems are solved. The discard and redesign may be done in one lump, or it may be done piece-by-piece. But all large-system experience shows that it will be done.2 Where a new system concept or new technology is used, one has to build a system to throw away, for even the best planning is not so omniscient as to get it right the first time.
	  
	  The management question, therefore, is not whether to build a pilot system and throw it away. You will do that. The only question is whether to plan in advance to build a throwaway, or to promise to deliver the throwaway to customers. Seen this way, the answer is much clearer. Delivering that throwaway to customers buys time, but it does so only at the cost of agony for the user, distraction for the builders while they do the redesign, and a bad reputation for the product that the best redesign will find hard to live down.
	  
	  Hence plan to throw one away; you will, anyhow ([View Highlight](https://read.readwise.io/read/01gpy8arc82pmm29tf5zry6smv))
	- Once one recognizes that a pilot system must be built and discarded, and that a redesign with changed ideas is inevitable, it becomes useful to face the whole phenomenon of change. The first step is to accept the fact of change as a way of life, rather than an untoward and annoying exception. Cosgrove has perceptively pointed out that the programmer delivers satisfaction of a user need rather than any tangible product. And both the actual need and the user's perception of that need will change as programs are built, tested, and used.3 ([View Highlight](https://read.readwise.io/read/01gpy97np2b93eam3wbp0g3xsg))
	- Nevertheless, some changes in objectives are inevitable, and it is better to be prepared for them than to assume that they won't come. Not only are changes in objective inevitable, changes in development strategy and technique are also inevitable. The throw-one-away concept is itself just an acceptance of the fact that as one learns, he changes the design.4 ([View Highlight](https://read.readwise.io/read/01gpy98dkd5jwg7nczwpdtv9jb))
	- Plan the Organization for Change
	  
	  Cosgrove advocates treating all plans, milestones, and schedules as tentative, so as to facilitate change. This goes much too far—the common failing of programming groups today is too little management control, not too much. ([View Highlight](https://read.readwise.io/read/01gpy9979bkqdgcf66p2dh3r6j))
	- He observes that the reluctance to document designs is not due merely to laziness or time pressure. Instead it comes from the designer's reluctance to commit himself to the defense of decisions which he knows to be tentative. "By documenting a design, the designer exposes himself to the criticisms of everyone, and he must be able to defend everything he writes. If the organizational structure is threatening in any way, nothing is going to be documented until it is completely defensible."
	  
	  Structuring an organization for change is much harder than designing a system for change. Each man must be assigned to jobs that broaden him, so that the whole force is technically flexible. On a large project the manager needs to keep two or three top programmers as a technical cavalry that can gallop to the rescue wherever the battle is thickest. ([View Highlight](https://read.readwise.io/read/01gpy9bdyb0hjrf5rx86cxafv1))
	- Management structures also need to be changed as the system changes. This means that the boss must give a great deal of attention to keeping his managers and his technical people as interchangeable as their talents allow. ([View Highlight](https://read.readwise.io/read/01gpy9c2vk4qfy5dvxhvrzssbv))
	- Sharp Tools
	  
	  A good workman is known by his tools ([View Highlight](https://read.readwise.io/read/01gpy9hpqqq0kcyvr171gnv9b0))
	- Bug-proofing the definition. The most pernicious and subtle bugs are system bugs arising from mismatched assumptions made by the authors of various components. The approach to conceptual integrity discussed above in Chapters [4](https://readwise.io/reader/document_raw_content/26202268#filepos57546), [5](https://readwise.io/reader/document_raw_content/26202268#filepos75990), and [6](https://readwise.io/reader/document_raw_content/26202268#filepos86194) addresses these problems directly. In short, conceptual integrity of the product not only makes it easier to use, it also makes it easier to build and less subject to bugs.
	  
	  So does the detailed, painstaking architectural effort implied by that approach. V. A. Vyssotsky, of Bell Telephone Laboratories' Safeguard Project, says, "The crucial task is to get the product defined. Many, many failures concern exactly those aspects that were never quite specified."1 Careful function definition, careful specification, and the disciplined exorcism of frills of function and flights of technique all reduce the number of system bugs that have to be found. ([View Highlight](https://read.readwise.io/read/01gpy9qxzqwtcf8s85zddwmae7))
	- Testing the specification. Long before any code exists, the specification must be handed to an outside testing group to be scrutinized for completeness and clarity. As Vyssotsky says, the developers themselves cannot do this: "They won't tell you they don't understand it; they will happily invent their way through the gaps and obscurities."
	  
	  Top-down design. In a very clear 1971 paper, Niklaus Wirth formalized a design procedure which had been used for years by the best programmers.2 Furthermore, his notions, although stated for program design, apply completely to the design of complex systems of programs. The division of system building into architecture, implementation, and realization is an embodiment of these notions; furthermore, each of the architecture, implementation, and realization can be best done by top-down methods. ([View Highlight](https://read.readwise.io/read/01gpy9v1g0rftdqrwvf52j7n9s))
	- Briefly, Wirth's procedure is to identify design as a sequence of refinement steps. One sketches a rough task definition and a rough solution method that achieves the principal result. Then one examines the definition more closely to see how the result differs from what is wanted, and one takes the large steps of the solution and breaks them down into smaller steps. Each refinement in the definition of the task becomes a refinement in the algorithm for solution, and each may be accompanied by a refinement in the data representation.
	  
	  From this process one identifies modules of solution or of data whose further refinement can proceed independently of other work. The degree of this modularity determines the adaptability and changeability of the program.
	  
	  Wirth advocates using as high-level a notation as is possible at each step, exposing the concepts and concealing the details until further refinement becomes necessary.
	  
	  A good top-down design avoids bugs in several ways. First, the clarity of structure and representation makes the precise statement of requirements and functions of the modules easier. Second, the partitioning and independence of modules avoids system bugs. Third, the suppression of detail makes flaws in the structure more apparent. Fourth, the design can be tested at each of its refinement steps, so testing can start earlier and focus on the proper level of detail at each step.
	  
	  The process of step-wise refinement does not mean that one never has to go back, scrap the top level, and start the whole thing again as he encounters some unexpectedly knotty detail. Indeed, that happens often. But it is much easier to see exactly when and why one should throw away a gross design and start over. Many poor systems come from an attempt to salvage a bad basic design and patch it with all kinds of cosmetic relief. Top-down design reduces the temptation ([View Highlight](https://read.readwise.io/read/01gpy9x0addvk8bkt03hem4rq5))
	- How does one control a big project on a tight schedule? The first step is to have a schedule. Each of a list of events, called milestones, has a date. Picking the dates is an estimating problem, discussed already and crucially dependent on experience.
	  
	  For picking the milestones there is only one relevant rule. Milestones must be concrete, specific, measurable events, defined with knife-edge sharpness. Coding, for a counterexample, is "90 percent finished" for half of the total coding time. Debugging is "99 percent complete" most of the time. "Planning complete" is an event one can proclaim almost at will.1
	  
	  Concrete milestones, on the other hand, are 100-percent events. "Specifications signed by architects and implementers," "source coding 100 percent complete, keypunched, entered into disk library," "debugged version passes all test cases." These concrete milestones demark the vague phases of planning, coding, debugging.
	  
	  It is more important that milestones be sharp-edged and unambiguous than that they be easily verifiable by the boss. Rarely will a man lie about milestone progress, if the milestone is so sharp that he can't deceive himself. But if the milestone is fuzzy, the boss often understands a different report from that which the man gives. To supplement Sophocles, no one enjoys bearing bad news, either, so it gets softened without any real intent to deceive. ([View Highlight](https://read.readwise.io/read/01gpya9e8qsptp7cn50navqxnd))
	- How does one control a big project on a tight schedule? The first step is to have a schedule. Each of a list of events, called milestones, has a date. Picking the dates is an estimating problem, discussed already and crucially dependent on experience.
	  
	  For picking the milestones there is only one relevant rule. Milestones must be concrete, specific, measurable events, defined with knife-edge sharpness. Coding, for a counterexample, is "90 percent finished" for half of the total coding time. Debugging is "99 percent complete" most of the time. "Planning complete" is an event one can proclaim almost at will.1
	  
	  Concrete milestones, on the other hand, are 100-percent events. "Specifications signed by architects and implementers," "source coding 100 percent complete, keypunched, entered into disk library," "debugged version passes all test cases." These concrete milestones demark the vague phases of planning, coding, debugging.
	  
	  It is more important that milestones be sharp-edged and unambiguous than that they be easily verifiable by the boss. Rarely will a man lie about milestone progress, if the milestone is so sharp that he can't deceive himself. But if the milestone is fuzzy, the boss often understands a different report from that which the man gives. To supplement Sophocles, no one enjoys bearing bad news, either, so it gets softened without any real intent to deceive ([View Highlight](https://read.readwise.io/read/01gpyaahje6m2xmwkbs54yaj4j))
	- Two interesting studies of estimating behavior by government contractors on large-scale development projects show that:
	  
	  1.  Estimates of the length of an activity, made and revised carefully every two weeks before the activity starts, do not significantly change as the start time draws near, no matter how wrong they ultimately turn out to be.
	  2.  During the activity, overestimates of duration come steadily down as the activity proceeds.
	  3.  Underestimates do not change significantly during the activity until about three weeks before the scheduled completion.2 ([View Highlight](https://read.readwise.io/read/01gpyabvs2eex4g2tm8at08sfd))
	- But not all one-day slips are equally disastrous. So some calculation of response is necessary, though hustle be dampened. How does one tell which slips matter? There is no substitute for a PERT chart or a critical-path schedule. Such a network shows who waits for what. It shows who is on the critical path, where any slip moves the end date. It also shows how much an activity can slip before it moves into the critical path.
	  
	  The PERT technique, strictly speaking, is an elaboration of critical-path scheduling in which one estimates three times for every event, times corresponding to different probabilities of meeting the estimated dates. I do not find this refinement to be worth the extra effort, but for brevity I will call any critical path network a PERT chart.
	  
	  The preparation of a PERT chart is the most valuable part of its use. Laying out the network, identifying the dependencies, and estimating the legs all force a great deal of very specific planning very early in a project. The first chart is always terrible, and one invents and invents in making the second one.
	  
	  As the project proceeds, the PERT chart provides the answer to the demoralizing excuse, "The other piece is late anyhow." It shows how hustle is needed to keep one's own part off the critical path, and it suggests ways to make up the lost time in the other part ([View Highlight](https://read.readwise.io/read/01gpyaqms0x9s1r2v88yyy7pcs))
	- But every boss needs two kinds of information, exceptions to plan that require action and a status picture for education.3 For that purpose he needs to know the status of all his teams. Getting a true picture of that status is hard ([View Highlight](https://read.readwise.io/read/01gpyas87ff2hfg3cfwk40jp60))
	- The first-line manager's interests and those of the boss have an inherent conflict here. The first-line manager fears that if he reports his problem, the boss will act on it. Then his action will preempt the manager's function, diminish his authority, foul up his other plans. So as long as the manager thinks he can solve it alone, he doesn't tell the boss.
	  
	  Two rug-lifting techniques are open to the boss. Both must be used. The first is to reduce the role conflict and inspire sharing of status. The other is to yank the rug back.
	  
	  Reducing the role conflict. The boss must first distinguish between action information and status information. He must discipline himself not to act on problems his managers can solve, and never to act on problems when he is explicitly reviewing status. I once knew a boss who invariably picked up the phone to give orders before the end of the first paragraph in a status report. That response is guaranteed to squelch full disclosure. ([View Highlight](https://read.readwise.io/read/01gpyasy188kary6c4d966tces))
	- Conversely, when the manager knows his boss will accept status reports without panic or preemption, he comes to give honest appraisals.
	  
	  This whole process is helped if the boss labels meetings, reviews, conferences, as status-review meetings versus problem-action meetings, and controls himself accordingly. Obviously one may call a problem-action meeting as a consequence of a status meeting, if he believes a problem is out of hand. But at least everybody knows what the score is, and the boss thinks twice before grabbing the ball. ([View Highlight](https://read.readwise.io/read/01gpyawgz0sf7dcw5mz0577d74))
	- Yanking the rug off. Nevertheless, it is necessary to have review techniques by which the true status is made known, whether cooperatively or not. The PERT chart with its frequent sharp milestones is the basis for such review. On a large project one may want to review some part of it each week, making the rounds once a month or so.
	  
	  A report showing milestones and actual completions is the key document. Figure 14.1 shows an excerpt from such a report. This report shows some troubles. Specifications approval is overdue on several components. Manual (SLR) approval is overdue on another, and one is late getting out of the first state (Alpha) of the independently conducted product test. So such a report serves as an agenda for the meeting of 1 February. Everyone knows the questions, and the component manager should be prepared to explain why it's late, when it will be finished, what steps he's taking, and what help, if any, he needs from the boss or collateral groups ([View Highlight](https://read.readwise.io/read/01gpyb04fpw7v57tk17a23dhb1))
	- > I have found it handy to carry both "scheduled" and "estimated" dates in the milestone report. The scheduled dates are the property ofthe project manager and represent a consistent work plan for theproject as a whole, and one which is a priori a reasonable plan. Theestimated dates are the property of the lowest level manager who hascognizance over the piece of work in question, and represents his bestjudgment as to when it will actually happen, given the resources hehas available and when he received (or has commitments for deliveryof) his prerequisite inputs. The project manager has to keep his fingersoff the estimated dates, and put the emphasis on getting accurate,unbiased estimates rather than palatable optimistic estimates or self-protective conservative ones. Once this is clearly established in everyone 's mind, the project manager can see quite a ways into the futurewhere he is going to be in trouble if he doesn 't do something. *
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/26202268/id34-00032.jpg)
	  
	  Figure 14.1
	  
	  The preparation of the PERT chart is a function of the boss and the managers reporting to him. Its updating, revision, and reporting requires the attention of a small (one to three man) staff group which serves as an extension of the boss. Such a Plans andControls team is invaluable for a large project. It has no authority except to ask all the line managers when they will have set or changed milestones, and whether milestones have been met. Since the Plans and Controls group handles all the paperwork, the burden on the line managers is reduced to the essentials—making the decisions ([View Highlight](https://read.readwise.io/read/01gpyb0qskta6wzkynrxmecf4k))
	- For several years I diligently lectured my software engineering class on the necessity and propriety of good documentation, exhorting them ever more fervently and eloquently. It didn't work. I assumed they had learned how to document properly and were failing from lack of zeal. Then I tried loading some cash registers into the wagon; i.e., showing them how the job is done. This has been much more successful. So the remainder of this essay will downplay exhortation and concentrate on the "how" of good documentation. ([View Highlight](https://read.readwise.io/read/01gpynap5cwp8yyww4pvpw4rer))
	- What Documentation Is Required?
	  
	  Different levels of documentation are required for the casual user of a program, for the user who must depend upon a program, and for the user who must adapt a program for changes in circumstance or purpose.
	  
	  To use a program. Every user needs a prose description of the program. Most documentation fails in giving too little overview. The trees are described, the bark and leaves are commented, but there is no map of the forest. To write a useful prose description, stand way back and come in slowly:
	  
	  1.  Purpose. What is the main function, the reason for the program?
	  2.  Environment. On what machines, hardware configurations, and operating system configurations will it run?
	  3.  Domain and range. What domain of input is valid? What range of output can legitimately appear?
	  4.  Functions realized and algorithms used. Precisely what does it do?
	  5.  Input-output formats, precise and complete.
	  6.  Operating instructions, including normal and abnormal ending behavior, as seen at the console and on the outputs.
	  7.  Options. What choices does the user have about functions?
	  8.  Exactly how are those choices specified?
	  9.  Running time. How long does it take to do a problem of specified size on a specified configuration?
	  10.  Accuracy and checking. How precise are the answers expected to be? What means of checking accuracy are incorporated? ([View Highlight](https://read.readwise.io/read/01gpynb3hawe2tqt2ncyyjermm))
	- Often all this information can be set forth in three or four pages. That requires close attention to conciseness and precision. Most of this document needs to be drafted before the program is written, for it embodies basic planning decisions.
	  
	  To believe a program. The description of how it is used must be supplemented with some description of how one knows it is working. This means test cases.
	  
	  Every copy of a program shipped should include some small test cases that can be routinely used to reassure the user that he has a faithful copy, accurately loaded into the machine.
	  
	  Then one needs more thorough test cases, which are normally run only after a program is modified. These fall into three parts of the input data domain:
	  
	  1.  Mainline cases that test the program's chief functions for commonly encountered data.
	  2.  Barely legitimate cases that probe the edge of the input data domain, ensuring that largest possible values, smallest possible values, and all kinds of valid exceptions work.
	  3.  Barely illegitimate cases that probe the domain boundary from the other side, ensuring that invalid inputs raise proper diagnostic messages. ([View Highlight](https://read.readwise.io/read/01gpyncggw4q62e18z7z25k21f))
	- To modify a program. Adapting a program or fixing it requires considerably more information. Of course the full detail is required, and that is contained in a well-commented listing. For the modifier, as well as the more casual user, the crying need is for a clear, sharp overview, this time of the internal structure. What are the components of such an overview?
	  
	  1.  A flow chart or subprogram structure graph. More on this later.
	  2.  Complete descriptions of the algorithms used, or else references to such descriptions in the literature.
	  3.  An explanation of the layout of all files used.
	  4.  An overview of the pass structure—the sequence in which data or programs are brought from tape or disk—and what is accomplished on each pass.
	  5.  A discussion of modifications contemplated in the original design, the nature and location of hooks and exits, and discursive discussion of the ideas of the original author about what modifications might be desirable and how one might proceed. His observations on hidden pitfalls are also useful ([View Highlight](https://read.readwise.io/read/01gpyncz6272vy0v9t42xy9cbv))
	- The flow chart is a most thoroughly oversold piece of program documentation. Many programs don't need flow charts at all; few programs need more than a one-page flow chart. ([View Highlight](https://read.readwise.io/read/01gpynkwhh6w69kmgf4k7afxtd))
	- Flow charts show the decision structure of a program, which is only one aspect of its structure. They show decision structure rather elegantly when the flow chart is on one page, but the overview breaks down badly when one has multiple pages, sewed together with numbered exits and connectors.
	  
	  The one-page flow chart for a substantial program becomes essentially a diagram of program structure, and of phases or steps. As such it is very handy. Figure 15.1 shows such a subprogram structure graph.
	  
	  Of course such a structure graph neither follows nor needs the painfully wrought ANSI flow-charting standards. All the rules on box shapes, connectors, numbering, etc. are needed only to give intelligibility to detailed flow charts.
	  
	  The detailed blow-by-blow flow chart, however, is an obsolete nuisance, suitable only for initiating beginners into algorithmic thinking. When introduced by Goldstine and von Neumann,1 the little boxes and their contents served as a high-level language, grouping the inscrutable machine-language statements into clusters of significance. As Iverson early recognized,2 in a systematic high-level language the clustering is already done, and each box contains a statement (Fig. 15.2). Then the boxes themselves become no more than a tedious and space-hogging exercise in drafting; they might as well be eliminated. Then nothing is left but the arrows. The arrows joining a statement to its successor are redundant; erase them. That leaves only GO TO's. And if one follows good practice and uses block structure to minimize GO TO's, there aren't many arrows, but they aid comprehension immensely. One might as well draw them on the listing and eliminate the flow chart altogether.
	  
	  In fact, flow charting is more preached than practiced. I have never seen an experienced programmer who routinely made detailed flow charts before beginning to write programs. Where organization standards require flow charts, these are almost invariably done after the fact. Many shops proudly use machine programs to generate this "indispensable design tool" from the completed code. I think this universal experience is not an embarrassing and deplorable departure from good practice, to be acknowledged only with a nervous laugh. Instead it is the application of good judgment, and it teaches us something about the utility of flow charts. ([View Highlight](https://read.readwise.io/read/01gpynmefepdw3w54scp1cwz7h))
	- Self-Documenting Programs
	  
	  A basic principle of data processing teaches the folly of trying to maintain independent files in synchronism. It is far better to combine them into one file with each record containing all the information both files held concerning a given key.
	  
	  Yet our practice in programming documentation violates our own teaching. We typically attempt to maintain a machine-readable form of a program and an independent set of human-readable documentation, consisting of prose and flow charts.
	  
	  The results in fact confirm our teachings about the folly of separate files. Program documentation is notoriously poor, and its maintenance is worse. Changes made in the program do not promptly, accurately, and invariably appear in the paper.
	  
	  The solution, I think, is to merge the files, to incorporate the documentation in the source program. This is at once a powerful incentive toward proper maintenance, and an insurance that the documentation will always be handy to the program user. Such programs are called self-documenting. ([View Highlight](https://read.readwise.io/read/01gpynr25nexyk5gh73cp4m7w4))
		- **Note**: Document in code so there is less need to create a separate document
	- Many of the classical problems of developing software products derive from this essential complexity and its nonlinear increases with size. From the complexity comes the difficulty of communication among team members, which leads to product flaws, cost overruns, schedule delays. From the complexity comes the difficulty of enumerating, much less understanding, all the possible states of the program, and from that comes the unreliability. From the complexity of the functions comes the difficulty of invoking those functions, which makes programs hard to use. From complexity of structure comes the difficulty of extending programs to new functions without creating side effects. From complexity of structure comes the unvisualized states that constitute security trapdoors. ([View Highlight](https://read.readwise.io/read/01gpyp3tjs923mnhbwhsgwg56x))
	- Not only technical problems but management problems as well come from the complexity. This complexity makes overview hard, thus impeding conceptual integrity. It makes it hard to find and control all the loose ends. It creates the tremendous learning and understanding burden that makes personnel turnover a disaster ([View Highlight](https://read.readwise.io/read/01gpyp4tb3486p2tcxvab7xf2c))
	- All successful software gets changed. Two processes are at work. As a software product is found to be useful, people try it in new cases at the edge of, or beyond, the original domain. The pressures for extended function come chiefly from users who like the basic function and invent new uses for it.
	  
	  Second, successful software also survives beyond the normal life of the machine vehicle for which it is first written. If not new computers, then at least new disks, new displays, new printers come along; and the software must be conformed to its new vehicles of opportunity. ([View Highlight](https://read.readwise.io/read/01gpyp5qnfacchsz7k0eqxbffq))