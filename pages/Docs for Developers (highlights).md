title:: Docs for Developers (highlights)
author:: [[Jared Bhatti]]
full-title:: "Docs for Developers"
media:: #books
status:: #📥inbox

- Notes
	- How to write effective documentation?
		- Understand your your users
			- Have empathy for your users. You have to understand what your users wants from the software and where they need help along the way.
			- You need to understand who your users (customer segmentation) and what they want to achieve.
			- You need to keep in mind that your users have their own goals that may not match their leadership or organization.
	- You can understand your users better through user research.
		-
- Highlights first synced by [[Readwise]] [[2023-01-17]]
	- I’ve often joked that “Good developers copy; great developers paste.” To understand why, you have to dig into the workflow used by most software engineers when faced with a problem. Our usual workflow looks like this:
	  
	  1.  1.
	    
	    Attempt to understand the problem.
	    
	  2.  2.
	    
	    Search for an existing solution everywhere we can think to look.
	    
	  3.  3.
	    
	    If we’re lucky enough to find one, we prove to ourselves the solution works.
	    
	  4.  4.
	    
	    We push the solution we found to production.
	    
	  
	  This is what we call the “developer loop,” and the most successful projects have documentation to guide developers through each of these steps. It’s because documentation is a feature. In fact, it’s the first feature of your project most users interact with, because it’s the first thing we look for when trying to solve a problem. ([View Highlight](https://read.readwise.io/read/01gpz0ynw04ygn7pq05c392fzh))
	- You might have heard the often-misquoted saying that *good code documents itself*. It’s true that good naming, types, design, and patterns make code easier to understand. But projects with sufficient complexity and scale (that is, most projects worth building) need human-readable documentation to help others quickly understand what you’re building and how to use it. ([View Highlight](https://read.readwise.io/read/01gpz11dbe90jxtnyenajejr3d))
	- 1. Understanding your audience ([View Highlight](https://read.readwise.io/read/01gpz134hvjm8x3665g5wykkec))
- New highlights added [[2023-01-17]] at 11:51 PM
	- So it begs the question, why is documentation often deprioritized or missing altogether?
	  
	  It’s not because we’re not invested in it, nor is it because we aren’t good writers. It’s because many of us don’t know how to do it. It’s because we, as developers, rarely understand that in addition to the developer loop, there’s an equally important “writer loop.” ([View Highlight](https://read.readwise.io/read/01gq1h29aja3pv8khcgc6hw9g5))
	- The writer loop is similar to how we write code. It requires you to understand the problem your users are trying to solve, create a plan for solving it, use common design patterns, and write the content that solves the issue. The developer loop and the writer loop are two sides of the same coin. During the writing loop, we’re creating information our users want during the developer loop. Knowing how to bring these two loops into alignment helps both your project and your users succeed. ([View Highlight](https://read.readwise.io/read/01gq1h39vey316pdqzt92qb39f))
	- In the late 1980s, a group of economists at Harvard determined that humans assume others have the same knowledge they do. They named this cognitive bias the “curse of knowledge.”[1](https://readwise.io/reader/document_raw_content/27434535#Fn1) ([View Highlight](https://read.readwise.io/read/01gq1heg25dp2bd51nsmrstw5z))
	- Breaking the curse, and writing effective documentation, requires empathy for your users. You have to understand what your users want from your software, and where they need help along the way. Through user research, you can understand your users’ needs well enough to predict what they need before they need it. By performing user research before you put pen to paper or hands to keyboard, you’ll set your users on the path to success. ([View Highlight](https://read.readwise.io/read/01gq1hfje3myjs3eqb3ehva326))
	- Creating an initial sketch of your users
	  
	  To write effectively for users, you need to understand who they are and what they want to achieve.
	  
	  Start by gathering and reviewing any existing materials you already have about your product or your users. These could include old emails, design documents, chat conversations, code comments, and commit messages. Reviewing these artifacts will help you build a clearer picture of how your software works and what you intend your users to do with it.
	  
	  Users also have their own goals that may or may not match those of your organization. An initial review can help identify any initial gaps or mismatches between these different sets of goals. ([View Highlight](https://read.readwise.io/read/01gq1jc2bqzp8w36kbh7jrmwb3))
	- Defining your users’ goals
	  
	  Once you review your existing knowledge, the next step is to understand what your users want to accomplish from reading your documentation. Knowing your users’ goals will guide your research and focus your efforts on documenting the most relevant information.
	  
	  Consider: why are you writing this documentation in the first place? You don’t just want your users to know something about your software; you want them to complete a set of tasks or change their behavior in some way. There is an engineering goal (for them) and a business goal (for you) that you want your users to reach. ([View Highlight](https://read.readwise.io/read/01gq1jch3se0q21558zxj25ftn))
	- At Corg.ly, Charlotte needs to onboard as many new users to Corg.ly as possible for the business to be a success. The goal of Corg.ly documentation can be summarized as
	  
	  > *Onboard new users to Corg.ly by helping them integrate with Corg.ly’s API.*
	  
	  By contrast, the most common goal of Corg.ly users is
	  
	  > Translate my dog’s barks into human speech.
	  
	  The goals of Corg.ly and Corg.ly users are different, but they can still align in a single documentation set. You probably have a goal for your users as well. Identifying how different goals can both differ and overlap helps you gain empathy and meet needs effectively. ([View Highlight](https://read.readwise.io/read/01gq1jdbhbnmgydp0jye8rthb9))
- New highlights added [[2023-01-18]] at 1:51 AM
	- Not every user is the same, and you can’t meet every user’s needs. Prioritize the users who are most important for your product or business.
	  
	  For example, if your software will primarily be used by developers, then focus on understanding *developers’* needs—as opposed to those of a product manager who may be evaluating your software for an engineering team. Consider what kind of developer your user is: an application developer using an API needs different things than a site reliability engineer (SRE) focused on security and reliability. ([View Highlight](https://read.readwise.io/read/01gq1kw5ybj03brhfqpkz2nfk1))
	- Outline your users’ needs
	  
	  Once you create a basic definition of who your users are and the overall goal you want them to accomplish, you can start outlining what your users need. The easiest approach is to list questions your users will have about your product that your documentation will need to answer.
	  
	  Some questions, in general, apply to all products. Questions like:
	  
	  •   What is this product?
	    
	  •   Will this product solve my problem?
	    
	  •   What features are available?
	    
	  •   How much does it cost?
	    
	  •   How do I get started?
	    
	  
	  Other questions are going to be very specific to your product, your users, and their goal:
	  
	  •   How do I authenticate against your API?
	    
	  •   How do I use a specific feature?
	    
	  •   How do I troubleshoot a specific problem?
	    
	  
	  You’ll identify some of these questions immediately through your experience with your own product, but remember your curse of knowledge. Your users don’t know as much about your product as you do, so they will likely have basic questions about your product that you’ll need to answer. As you do more research into your users and validate your understanding, you can add additional questions for which users need answers from your documentation. ([View Highlight](https://read.readwise.io/read/01gq1kwxwpdazhb67z0qpy50hw))
	- Validate your user understanding
	  
	  Once you have a definition of your users, their goals, and their needs, you should validate and build on your initial understanding. User research helps you confirm who your users are and what they need from your documentation.
	  
	  The quickest way to confirm or reject your assumptions about who your users are and what they need from your documentation is to talk to them directly. Interacting directly with users is a surefire way to help you understand what they’re trying to do with your software, how they’re currently using it, and any frustrations or concerns they have ([View Highlight](https://read.readwise.io/read/01gq1kyye0mx0xm2mwfcmwpfqx))
	- The focus here is on your users’ *needs*, which are different from user *wants* ([View Highlight](https://read.readwise.io/read/01gq1m6e3bcr7vwnsh1qbbs9a8))
	- Using existing data sources
	  
	  The easiest way to connect with your users is to find the places where communication channels already exist. If you’re part of a larger organization, you might have access to teams who are already having conversations with users whom you can reach out to. These teams include:
	  
	  •   Developer relations
	    
	  •   Product support
	    
	  •   User experience
	    
	  •   Marketing
	    
	  
	  These teams can help you validate your assumptions about your user and give you additional information, for example: What do we already know about our users’ experience with the software? What are their blockers or pain points? How long does it take for a user to complete a successful integration? ([View Highlight](https://read.readwise.io/read/01gq1m720sm91nb5deqx1ybcky))
	- Support tickets
	  
	  Support tickets are an existing data source and a gold mine for understanding your users. Nothing beats the content of a support request sent in the heat of the moment by a frustrated user for understanding what your users need most. In addition, you can follow up with the user who filed the support ticket and see if they would be willing to speak with you directly. ([View Highlight](https://read.readwise.io/read/01gq1m7nrq8zd9c8a7rqxt6406))
	- Collecting new data
	  
	  Sometimes, existing data sources aren’t available or aren’t enough to validate or refute the assumptions we have about our readers. This is a perfect opportunity for more in-depth research collection methods. However, it’s important to note that good research can be time consuming. Although the return on your time investment will be huge, it can be tricky to find the balance between the right amount of research and the need to get your documentation in front of your readers quickly. ([View Highlight](https://read.readwise.io/read/01gq1m8qw09bvb6m3qdvvfdqye))
	- Direct interviews
	  
	  Where themes overlap or requests seem the most pressing, interviews can help you dig a little deeper. Provided you are considerate of their time, most people like the chance to help shape a future product or documentation . ([View Highlight](https://read.readwise.io/read/01gq1m9snw8kw2rxn3xm8mxqkw))
	- Regardless of your interview source, pursue quality over quantity. Five potential readers who fit your target audience will offer much more valuable insight than fifty people who didn’t meet your criteria, but were easier to find—and if you can only find five participants, that’s okay, too. Advice varies, but around three to five people for one “round” of research is considered a robust enough sample on which to base future content decisions.[4](https://readwise.io/reader/document_raw_content/27434535#Fn4) ([View Highlight](https://read.readwise.io/read/01gq1mc6e1wqvrgaeaspwyavvx))
	- When performing the interviews, it’s important to prepare your topics in advance to keep the conversations focused and useful. Some high-level topics for the Corg.ly API could be:
	  
	  •   Previous experience using similar services and APIs
	    
	  •   Expectations while using the Corg.ly API ([View Highlight](https://read.readwise.io/read/01gq1mcp20pkh0n46q0b8xyh1x))
	- Break each topic down into specific, open questions. A specific question bounds the scope of possible answers in a helpful way. An open question is exploratory, usually answered with a story or longer explanation. By contrast, a closed question is limited and usually answered with a yes or a no. For example, “Have you used pet translation software before?” is a closed question. You can rephrase it as an open question by asking, “What’s your experience using translation software?” ([View Highlight](https://read.readwise.io/read/01gq1md0aazn8e3seb85tvkgnn))
	- To make a survey quick and painless, you need to create a small set of targeted questions. As with planning interviews, you’ll need to know what you want to find out—and asking fewer questions is more impactful than trying to cover everything.
	  
	  Good survey questions:
	  
	  •   Ask one thing per question
	    
	  •   Are closed (with limited answers)
	    
	  •   Optional to answer
	    
	  •   Are neutral ([View Highlight](https://read.readwise.io/read/01gq1mhpgdccat04r6nf6pajnj))
	- Even the most perfectly designed questions are only useful if people answer them. There are several tactics you can use to increase your response rate. Make it clear who you are, what data you’re collecting, and why. Write your questions carefully so they are easy to answer. If you demand too much from your responder, it’s likely they will not complete the survey or annoy them so much it skews their responses.[6](https://readwise.io/reader/document_raw_content/27434535#Fn6) ([View Highlight](https://read.readwise.io/read/01gq1mj4jvgr80ydxttyb5r7st))
	- Condensing user research findings
	  
	  Compiling your results and observations from research can feel unnecessary. You’ve probably gathered a lot of information about problems you want to immediately fix, but hold up! That rush of knowledge is easily lost, and it’s worth taking the time to condense your findings into tangible records you can refer to during later stages of writing documentation.
	  
	  Three useful ways of condensing your user research findings are:
	  
	  •   User personas
	    
	  •   User stories
	    
	  •   User journey maps ([View Highlight](https://read.readwise.io/read/01gq1mk0s4b7w36ny0han9ffkm))
	- User personas
	  
	  A *user persona* is a semi-fictional character created to represent your ideal reader or readers. This character can be based on a specific person or an amalgam of people you learned about in your research. A user persona usually includes a short description of the individual (real or imagined) and a list of their goals, skills, knowledge, and situation.
	  
	  To build a user persona, compile a list of the essential characteristics you’ve learned about your users through your research. For example, here’s a user persona for an advanced developer based on Mei, Corg.ly’s alpha customer:
	  
	  **Name:** Mei
	  
	  **Developer skill**
	  
	  Advanced
	  
	  **Languages**
	  
	  Python, Java
	  
	  **Developer environment**
	  
	  MacOS, Linux
	  
	  **Role**
	  
	  Lead developer ([View Highlight](https://read.readwise.io/read/01gq1mm1ey3mxxa27m7hkd26aq))
	- Once you create your personas, consider which persona you want to focus the rest of your research on ([View Highlight](https://read.readwise.io/read/01gq1mmzdp4qctgd1pvxnb6rfn))
	- User stories
	  
	  If you have more time, you may find it useful to write *user stories* alongside your personas. User stories are short written summaries of what a user is trying to achieve and are a nifty way to condense your users’ needs to keep them front of mind for the planning, writing, editing, publishing, and maintenance that comes next ([View Highlight](https://read.readwise.io/read/01gq1mpcvvdv46tr9d9n36876e))
	- User journey maps
	  
	  For meatier research projects with ample research notes and text, a visual illustration can be handy. A *user journey map* is a diagram showing the path a user takes through a product or website while trying to accomplish a particular task. The map usually covers all routes or “channels” a user may take when interacting with your software and documentation. The map is a timeline, tracking what a user does at each point in their journey and what they feel or experience at each step. Creating a user journey map can be a succinct way to condense your findings, highlighting where your users are happiest, and where you can improve.
	  
	  To create a user journey map:
	  
	  1.  1.
	    
	    Define the task the user is trying to accomplish.
	    
	  2.  2.
	    
	    List the channels a user may interact with (e.g., your website, docs, your code repository, or the app itself).
	    
	  3.  3.
	    
	    Piece together the steps a user takes through each channel (e.g., discover, sign up, install, configure, test, run, review).
	    
	  4.  4.
	    
	    List the user experience at each step (e.g., what they are doing, feeling, thinking).
	    
	  5.  5.
	    
	    Connect the channels, steps, and experiences in a flow. ([View Highlight](https://read.readwise.io/read/01gq1mppyzd3jt9g56pb6es8k5))
	- Figure [1-1](https://readwise.io/reader/document_raw_content/27434535#Fig1) shows an example map of a user journey where a user evaluates, signs up for, and connects to Corg.ly. The top row shows common user questions identified through Charlotte’s research. The middle row shows the user’s experience throughout the journey (where the current experience is meeting or not meeting their needs). The final row lists opportunities for Charlotte’s team to add or improve the documentation or product to provide a better experience .
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/27434535/Aimages_505277_1_En_1_Chapter_505277_1_En_1_Fig1__HXNODMg.jpg) ([View Highlight](https://read.readwise.io/read/01gq1mq2hfz7baasv80htkfp75))
	- Creating a friction log ([View Highlight](https://read.readwise.io/read/01gq1mssd2ex85v60qzzkv7zbh))
	- A *friction log* is a journal in which you try your software as a user would and record your experiences. To record your experience, log each step sequentially, noting the behavior you expect and the actual behavior of your software. The bigger the gap between expectation and reality, the bigger the opportunity to improve your docs or software.
	  
	  The best friction logs have a tight scope to prevent sprawl and keep results actionable. Pick a user and a scenario with a clear beginning and end, for example, a developer installing your software for the first time. Note the scenario and any other test information at the top of the page, such as the environment or version you’re using. ([View Highlight](https://read.readwise.io/read/01gq1mtahksw8ny2w9kyh1xvk7))
	- **Goal:** Start using Corg.ly API
	  
	  Tasks
	  
	  Friction log
	  
	    1. Sign up for a paid Corg.ly account.
	  
	    1. Opened Corg.ly website.
	  
	    2. Navigated to web form for sign-up. Had to scroll to the bottom of the page. Difficult to find. Maybe add to top of page?
	  
	    3. Completed form. Put in credit card information.
	  
	    4. Clicked submit button. Did not receive confirmation it had been submitted. No error generated.
	  
	    5. Noticed some form fields were blank. Did the empty fields stop the form from submitting?
	  
	    6. Filled in blank fields.
	  
	    7. Clicked submit button. Received confirmation message and reassuring information has been sent.
	  
	  ...
	  
	  You may find it useful to color code your friction log to indicate positive and negative user experiences. For example, green could indicate steps that were easy to complete, offered clear evidence of success, and guided you to the next step, or red for steps that were particularly frustrating or stopped you from progressing. ([View Highlight](https://read.readwise.io/read/01gq1mw9gpdgdsfmazdkws18t1))
	- Friction logs offer a chance to reflect on what steps could be improved by documentation and which by software changes. You may have identified issues that are fixable in the product (a missing error message, a typo in a command) rather than documentation. Consider creating a bug report or issue to capture these and free your time to focus on writing documentation for where it matters most. ([View Highlight](https://read.readwise.io/read/01gq1mx1nxkx55rmc5fdqayf0d))
	- You don’t need to restrict friction logging to the early stages of your documentation project. Rerunning or picking a new area to log is a great way to reconnect with your readers and remember what it feels like to experience your software as a newcomer, as well as find new improvements to make. In time, you can test the usability of your documentation itself alongside your software, which can be a handy means of measuring the effectiveness of your documentation. For more information on measuring the quality of your documentation, see Chapter [9](https://readwise.io/reader/document_raw_content/27434535#None). ([View Highlight](https://read.readwise.io/read/01gq1mx8at74vvvjj3jhn0nmsm))
	- Getting started documentation
	  
	  Guiding users through first impressions and first-time user experience is the critical role of *getting started documentation.* Getting started docs are your opportunity to help users get up and running and to build trust with your users that you will guide and support them with good resources. As you write a getting started document, some questions you should ask yourself are:
	  
	  •   What are the quickest explanations of what this service is and what its core features do?
	    
	  •   What are the simplest steps to install and use your product?
	    
	  •   What are the most important questions new users will have?
	    
	  •   What are the cool things they can do with your service?
	    
	  
	  Getting started documentation should translate your user’s interest into them actually developing with your product. If your product is fairly simple, you could show the steps of how to do a basic integration with your product and your user’s code. If your product is more complex, you could provide your users with an inline or downloadable code sample that just needs a few small tweaks to use. It’s better to show your users your product than to tell them about it.
	  
	  Getting started content also acts as a starting point for more advanced pieces of content. A common mistake organizations make is to only produce advanced documentation, like how-to guides. But you really want to make sure that all types of users are supported, whether they’re advanced or just evaluating your service. You need to help them quickly understand what your product does and what it can do for them. Getting started documentation helps with this problem ([View Highlight](https://read.readwise.io/read/01gq1npvfg2wpm68q5mfvzvmjf))
	- Conceptual documentation
	  
	  The next content type is *conceptual documentation* *.* Conceptual documentation helps users understand the concepts and ideas behind your service. It describes how your service works to your users. Conceptual content can be opinionated, but it should avoid implementation details. (Implementation details belong in procedural content, covered later in this chapter.)
	  
	  Meeting notes, design documents, whiteboard diagrams, and internal documentation are great source material for your service’s conceptual content.
	  
	  Keep conceptual documentation brief and concise, especially if you’re using conceptual information to set context for a procedure or tutorial. Focus on these sections:
	  
	  Conceptual guide
	  
	  The first paragraph, which introduces the concept explained in the document.
	  
	  **Overview**
	  
	  Give a technical overview of how the concept works. Describe any additional sub-components or related concepts in sub-sections.
	  
	  **Related Concept 1**
	  
	  **. . .**
	  
	  **Related Concept 2**
	  
	  **. . .**
	  
	  **Additional resources**
	  
	  List any related documentation, including tutorials and how-to guides that implement the concept.
	  
	  Limit the number of concepts explained in a single document. Readers are generally good at absorbing one core concept at a time. If you’re explaining several new concepts, things get complex very quickly and users may struggle. By keeping conceptual documentation simple for your readers, beginners will feel comfortable learning about your service, and advanced users will appreciate the efficiency it affords them.
	  
	  Note
	  
	  Conceptual documentation offers a good opportunity for simple user research. Ask a user to read a draft, and then ask them to explain what they read. Evaluate which concepts made sense to them and which ones did not. Improve your document based on this feedback and repeat the exercise as many times as needed.
	  
	  This user research exercise also shows you other content to include in your documentation plan. Not only does iterative user research improve your conceptual documentation, it helps you identify gaps that you can fill with other types of documentation ([View Highlight](https://read.readwise.io/read/01gq1nrnqcqb7mqxccvgm7jkef))
	- Procedural documentation
	  
	  The next type of user content is *procedural documentation* . Procedural content includes tutorials and how-to guides—anything from installation instructions to API integrations. A procedural document shows readers how to accomplish a specific goal by following a set of structured steps. A single step should describe a single action that a user takes.
	  
	  People read documentation to solve a problem or accomplish a task, and they want to do so as quickly and effectively as possible. These are some useful patterns for writing guides and tutorials:
	  
	  •   Make the guide stand on its own as much as possible with all the actions users need on a single page.
	    
	  •   Keep the number of steps limited to what’s necessary for your users. When a procedure contains many steps, the procedure looks overwhelming and complex to users. Longer procedures also create more opportunities for mistakes and tend to require more maintenance.
	    
	  •   Avoid lengthy explanations. A few sentences of explanation or a well-placed image is useful, but too much additional content within a procedure tends to overwhelm users. A good practice is to write procedures that allow a user to see two or more steps on a standard monitor screen. If you find your procedure contains many explanations, consider separating that information out into a conceptual guide. Note that this doesn’t apply to code examples ([View Highlight](https://read.readwise.io/read/01gq1ns8g8jfh4tdada8hzcvxa))
	- Tutorials
	  
	  A *tutorial* is a procedure that teaches users how to achieve a specific goal. Tutorials help users test an integration without implementing real code. Good tutorials provide users with an environment they can use for learning and may even offer test data or tools to use.
	  
	  If your tutorial includes more than ten steps, you’re trying to solve for a use case that’s too complex, or you’re combining too many actions in one document. Long, time-consuming tutorials make it less likely that a user will successfully finish.
	  
	  If you can’t condense a long tutorial—or any procedural content, for that matter—into fewer steps despite your best efforts, it could mean the service itself is too complex. There may be steps that should be combined, automated, or omitted from the service—and that’s a conversation you should have with the product developers . ([View Highlight](https://read.readwise.io/read/01gq1nsmb89zga6b32ew4pc26g))
	- How-to guides
	  
	  *How-to guides* are the core type of procedural content. A how-to guide shows how users can solve actual business problems by performing specific steps with your service.
	  
	  How-to guides are a true differentiator for your users: a single document that helps them build a solution to their problem. While tutorials focus on learning, a how-to guide is based on action with users implementing real code.
	  
	  How-To Guide
	  
	  The first paragraph, which introduces the core concepts and gives overview information required for this guide.
	  
	  **Prerequisites**
	  
	  List any steps your users should do before they follow the steps in this guide.
	  
	  **Steps**
	  
	  1.
	  
	  2.
	  
	  3.
	  
	  4.
	  
	  5.
	  
	  . . .
	  
	  **Next steps**
	  
	  Link to additional documentation the user should follow after doing the steps in this guide.
	  
	  When planning how-to guides, pay attention to your users’ needs and interpret your company’s strategy of what you want your users to do. Plan carefully and be selective, as how-to guides are labor-intensive to write and maintain. You could lead users astray by documenting edge cases at the outer boundaries of your service’s capability .
	  
	  A good pattern for writing how-to guides is to keep words simple, make actions clear, and continuously reinforce the problem the guide solves.
	  
	  Include prerequisites at the start of your guides. Prerequisites include any dependencies, such as installing a required version of your system or packages. If specialist skills and knowledge are truly required, list them as a prerequisite, but avoid this whenever possible. Assessments of knowledge or skills are often subjective and add unnecessary requirements. Prerequisites not only tell users what they need to accomplish a goal; they also provide users with an escape hatch. ([View Highlight](https://read.readwise.io/read/01gq1ntabn68f39jmb7wr40mf0))
	- Effective how-to guides keep users on a single page as much as possible. It’s tempting to use a link every time another page exists for a term or concept that you mention, but clicking too many links adds more distractions for users. As opposed to Wikipedia, which uses links liberally to teach you new things you didn’t know existed, you can help your users focus by creating a how-to guide on a single page. ([View Highlight](https://read.readwise.io/read/01gq1nv08r66phvvj33gfmxv1w))
	- Change documentation
	  
	  A *changelog* provides a helpful historical record for internal teams like support and engineering. Understanding when changes took place and when customers were impacted can be useful information when troubleshooting. Changelogs are most common in API documentation, where breaking changes or new versions can negatively impact a developer’s existing integration with your service.
	  
	  Whenever there’s a significant or breaking change, provide information for what, when, and why this occurred. Not only is it helpful in the moment when you’re letting users know that something changed, but if they’re looking backward and trying to troubleshoot an issue, they can see when a change took place that may have affected them .
	  
	  List changes in chronological order, including data like:
	  
	  •   Previously supported versions, integrations, or deprecated features
	    
	  •   Name changes of parameters or important fields
	    
	  •   An object or resource moved ([View Highlight](https://read.readwise.io/read/01gq1nwe99mrfzmcerng9dnqj9))
	- *Release notes* are another helpful type of documentation. Release notes provide rich context for the changes listed in a changelog. While a changelog can be automated or consist only of a bulleted list with little context, release notes speak directly to your users. *Here's the change that took place. Here's why. Here's how it used to be. Here's how it's going to be.* Release notes give users context to understand why a change took place. Example entries for release notes include:
	  
	  •   New features
	    
	  •   Bug fixes
	    
	  •   Known bugs or limitations
	    
	  •   Migrations
	    
	  
	  Release Notes
	  
	  **2020–03–18**
	  
	  Item one
	  
	  •   Summary
	    
	  •   Impact
	    
	  •   Reasoning
	    
	  •   Actions required
	    
	  
	  Item two
	  
	  . . .
	  
	  **2020–03–11**
	  
	  . . . ([View Highlight](https://read.readwise.io/read/01gq1nwqyxs74cmqsqqc3k8601))
		-
	- Planning your documentation
	  
	  Now that you understand the content types and patterns that best serve your users, you can create a documentation plan. A documentation plan functions as a flexible outline, making it easy to map out a user journey through the content you write.
	  
	  A good documentation plan allows you to:
	  
	  •   Anticipate and meet your user’s needs for information
	    
	  •   Get early feedback from users and internal stakeholders on your direction
	    
	  •   Identify gaps and shortcomings not just with your documentation, but the user journey for your service altogether
	    
	  •   Coordinate writing, organizing, and publishing your documentation with other stakeholders ([View Highlight](https://read.readwise.io/read/01gq1nx8fpc720bfhndw4vgenn))
- New highlights added [[2023-01-18]] at 2:51 PM
	- Creating a documentation plan is often straightforward, but easily overlooked. If you start writing documentation before creating a plan, you might miss critical information your users need or overlook problems they are trying to solve. Without a plan, it’s difficult to think about your user journeys holistically ([View Highlight](https://read.readwise.io/read/01gq3593bzcdtfs09n4jc2d30n))
	- To build your documentation plan, answer the following questions which will help you focus on the right information for your users. You already gathered some of this information in your user research (see Chapter [1](https://readwise.io/reader/document_raw_content/27434535#None)), but it’s useful to restate it at the top of your documentation plan to help you focus and keep the right information in scope.
	  
	  •   Who is your target audience? (You might already have a user persona for them.)
	    
	  •   What are the biggest takeaways you want them to have from your launch?
	    
	  •   In order of importance, what features are you releasing?
	    
	  •   What do users expect from your launch?
	    
	  •   Is there any knowledge users need before they start using your product or features?
	    
	  •   What are the use cases you’re supporting?
	    
	  •   Are there known issues or points of friction users could stumble upon? ([View Highlight](https://read.readwise.io/read/01gq359axsmqhvx4h2bp46ttr1))
	- Your content outline can be a list with a brief explanation of what’s in each document. A content outline for Corg.ly might look like Table [2-1](https://readwise.io/reader/document_raw_content/27434535#Tab1).
	  
	  Table 2-1
	  
	  Content outline
	  
	  Title
	  
	  Content type
	  
	  Brief description
	  
	  Getting Started with Corg.ly
	  
	  Getting started
	  
	  A very simple demo for using Corg.ly with links to other documentation
	  
	  Corg.ly: Dog Translation Explained
	  
	  Conceptual
	  
	  A technical explanation of how Corg.ly works
	  
	  Authenticating with Corg.ly’s API
	  
	  How-to
	  
	  A step-by-step procedure for authenticating with Corg.ly’s API
	  
	  Translating Dog Barks to English
	  
	  How-to
	  
	  A step-by-step procedure for translating dog barks into English
	  
	  Translating English into Dog Barks
	  
	  How-to
	  
	  A step-by-step procedure for translating English into dog barks
	  
	  Corg.ly API Reference
	  
	  API reference
	  
	  List of all API calls and their syntax
	  
	  Troubleshooting Audio Issues
	  
	  Troubleshooting
	  
	  Common issues with translating audio and managing audio files
	  
	  Release Notes
	  
	  Changelog
	  
	  Release notes for this Corg.ly release
	  
	  If your documentation plan reflects a coherent journey for your users, you’re probably in good shape. If your plan feels like a maze or it’s unclear what a user needs to do to accomplish a task or solve their problem, then go back and reshape the documentation plan. You may need to interview more users or internal stakeholders. If the problem isn’t with the documentation plan, then it may point to an overly complex service that needs improvement before a clear user journey can emerge. ([View Highlight](https://read.readwise.io/read/01gq35adw0mkxx6pqrmykte1h5))
	- Breaking through the blank page
	  
	  In previous chapters, you created an audience definition, researched existing content and code, and chose a documentation pattern to meet your needs.
	  
	  You can start your document by listing the information you’ve already gathered at the top:
	  
	  •   Audience
	    
	  •   Purpose
	    
	  •   Pattern
	    
	  
	  For example, let’s say you’re creating a document for a Corg.ly API that takes audio files of dog barks and translates them into strings of human language. You want to create a document that describes how to upload files to the Corg.ly service. Your initial information might look like:
	  
	  •   Audience: Developers using Corg.ly who know how to use REST APIs
	    
	  •   Purpose: Describe how to upload audio files to the Corg.ly service for analysis
	    
	  •   Content pattern: Procedural guide ([View Highlight](https://read.readwise.io/read/01gq35ggyd62dbtwjnsghbt0rm))
	- Defining your document’s title and goal
	  
	  You can define your document’s title based on the audience, purpose, and content pattern for the document. The title should be the shortest, clearest rephrasing of the document’s purpose from the user’s perspective.
	  
	  In the example of the Corg.ly service, the purpose of the document is: *Describe how to upload audio files to the Corg.ly service for analysis*. You can shorten this further for the reader into something like: “Uploading Audio Files to Corg.ly”.
	  
	  The title of the document should summarize the goal for reading the document. Anyone who clicks on your document title will know exactly what they’re getting. Here are a few examples of titles for additional documents:
	  
	  •   Translating dog barks to text
	    
	  •   Translating dog barks from streaming audio
	    
	  •   Audio encoding and sampling rates ([View Highlight](https://read.readwise.io/read/01gq35hjh6amrrvcjkkh02vwcm))
	- The goal of each of these documents is defined in the title. Limit your document to only one goal. If your document has several goals, you probably need multiple documents. ([View Highlight](https://read.readwise.io/read/01gq35n7dk8kwc1464mdr70yhv))
	- Meeting your reader’s expectations
	  
	  Once you create a title, goal, and outline for your document, it’s time to think about the *flow of information* . Consider what your reader needs to know and do to successfully complete the goal you stated in the title. Imagine their expectations and knowledge, drawing upon the research you’ve already done. The order of information in your outline should meet your user’s expectations and needs. The knowledge your reader has is different from yours, and their experience with what you’ve built won’t be as extensive. It’s up to you to provide the reader with the right information at the right time. This is what’s meant by the flow of information ([View Highlight](https://read.readwise.io/read/01gq35t0ybc0mhzec854qqyzdy))
	- Headers
	  
	  Headings are like signposts: they organize content within your document. Headings also serve as destinations in documentation, letting readers jump to exactly the information they need. Headings help structure content for the reader, but they’re also important for search engine optimization (SEO). Make sure to include headings in your document. ([View Highlight](https://read.readwise.io/read/01gq35xsp5f44vpfwmyb19axv5))
	- You can create document headings from your outline by making each of the high-level steps in your outline a header. When creating headers, keep the following tips in mind:
	  
	  •   **Be as brief, clear, and specific as possible.** Readers must be able to skim your headers quickly and understand your document at a high level.
	    
	  •   **Lead with the most important information.** Start with the most important information that readers need to know as close to the top of the page as possible.
	    
	  •   **Use unique headers for each section.** Unique headers help your reader find the right content quickly. For example, if there are multiple “testing” sections in the document, specify in the header what is being tested.
	    
	  •   **Be consistent.** Structure all of your headers similarly. If your document is a procedure for accomplishing a task, start every header with a verb. If you’re writing your document for a larger documentation set, match the style of headers in other documents. ([View Highlight](https://read.readwise.io/read/01gq35y8nvfbfz6a0y1r2rjj8w))
	- Procedures
	  
	  A procedure is a sequential set of actions a reader takes to achieve a desired result. Procedures should always use numbered lists to help readers understand the order of tasks they’re performing. Explain the desired goal at the start of the procedure so that users understand what they are doing. At the end of the procedure, add a way for the user to check that they performed it correctly. This serves as a kind of unit test for the documentation, and prevents users from compounding any errors they may make.
	  
	  For example, here’s a procedure to “Upload an audio file using Corg.ly’s UI”:
	  
	  1.  1.
	    
	    Open the Corg.ly app.
	    
	  2.  2.
	    
	    Select “Record” to record your dog barking.
	    
	  3.  3.
	    
	    Select “Upload” to upload your file for translation ([View Highlight](https://read.readwise.io/read/01gq364aebzzkyndhc4gv5teqp))
	- When you’re writing a procedure, identify the system’s starting state. Do you expect a reader to be logged in? Are they typing in a browser or a command line? Also, give readers the instructions they need to reach the desired state.
	  
	  Each step of the procedure should only cover one action. Your reader may be jumping between your documentation and your interface or the command line, and multiple actions in a single step can make it hard for your reader to follow along.
	  
	  Finally, give readers a way to verify they’ve completed the procedure properly. For example, at the end of the Corg.ly procedure, you could tell the reader they will receive a confirmation message if their upload has been successful. ([View Highlight](https://read.readwise.io/read/01gq364vaqcmg7d3603fxpvtky))
	- Lists are not in procedural order, but that doesn’t mean they are completely unordered. When creating a list, consider ordering it in a way that is most helpful to the user. For example, you could add a bulleted list to the audio file upload procedure:
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/27434535/Aimages_505277_1_En_3_Chapter_505277_1_En_3_Fig3__BHDOfz4.png)
	  
	  Figure 3-3
	  
	  Sample list of audio file types ([View Highlight](https://read.readwise.io/read/01gq365emveznmwwhpqw4vv6s6))
	- Callouts
	  
	  When writing your document, you might discover a piece of information that your reader needs to know at that moment, but that doesn’t fit with the flow of your content. It might be something absolutely critical that a reader needs to know in order to be safe, or it might be some useful, related information that you want to highlight at that point in the document. In these cases, you can use a *callout* .
	  
	  Here are some examples of callouts and when to use them:
	  
	  •   **Warning:** Don’t take this action! Readers might be in danger, personal data might be at stake, or the system may suffer irreversible damage or loss.
	    
	  •   **Caution:** Proceed carefully. An action might have unexpected consequences.
	    
	  •   **Note:** Related information or a tip about what you’re currently reading. ([View Highlight](https://read.readwise.io/read/01gq365z5cxgbp2fv4yb5abj0j))
	- For example, here’s a callout that you might find at the top of the doc for uploading an audio file to Corg.ly:
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/27434535/Aimages_505277_1_En_3_Chapter_505277_1_En_3_Fig4__z0vrMbB.jpg)
	  
	  Figure 3-4
	  
	  Example of a Caution callout ([View Highlight](https://read.readwise.io/read/01gq366xb4y8pjz9aeb6vj3vpt))
	- Writing for skimming
	  
	  There are two fundamental, paradoxical truths about readers of technical documentation:
	  
	  •   Readers come to your documentation looking for information.
	    
	  •   Readers read very little of what you write.
	    
	  
	  Think of how you read most content online: you probably search for something specific to catch your eye, quickly scanning the first few sections of multiple pages until you find what you’re looking for. Only when you’ve found what you’re looking for do you settle in and read content closely. You’ve moved through a number of pages while reading very little.
	  
	  Most people read in the same way: skimming titles and headings until they find the content that answers their question. In fact, based on the time readers spend on a page, they can read at most 28% of the words on a page (and that’s if they’re a very fast reader)[1](https://readwise.io/reader/document_raw_content/27434535#Fn1). This is true both for readers visually skimming through the document and for those using screen readers (tools that render content as speech or braille). ([View Highlight](https://read.readwise.io/read/01gq367j745nzyjpsemd8vpfs0))
- New highlights added [[2023-01-18]] at 4:51 PM
	- Completing your outline
	  
	  Review the outline for the document and consider your readers. Ask yourself the following questions:
	  
	  •   Is there additional introductory or setup information that readers need to know?
	    
	  •   Are there steps that you’re skipping or that aren’t fully explained?
	    
	  •   Do the steps make sense in consecutive order? ([View Highlight](https://read.readwise.io/read/01gq3cajvym8hvt6j2a3982b32))
	- Note
	  
	  When readers view a page of content, research shows they typically skim the content in an “F” pattern, scanning in two horizontal lines across the top of the document for the title and subtitle, and then scanning down the page. They do not read every word on the page.
	  
	  Write in a way that helps your reader skim your content to find the right piece of information. Helping your reader skim helps them find the content they’re looking for faster, and it leads to better, more direct content. There are a number of strategies you can use to make your content more skimmable and therefore more helpful to your readers. ([View Highlight](https://read.readwise.io/read/01gq3cbm0npq3rvw9fyhbyahxk))
	- State your most important information first
	  
	  If your reader is skimming your document they will, at most, get through the first few paragraphs of your document. In those first paragraphs, it’s important that you answer the question that’s burning in your reader’s mind: “Will this help me?”
	  
	  Your title should summarize the goal of the document. Include any critical information in the first three paragraphs. If you’re writing a procedure, let the reader know *what* they will accomplish by the end of the document. If you’re writing something more conceptual, explain the importance of the concept you’re describing, and *why* knowing more about it will help your reader. ([View Highlight](https://read.readwise.io/read/01gq3ccg0tb8wgjpbm7vtnahn2))
	- Break up large blocks of text
	  
	  Long paragraphs are difficult to skim. If most of your writing is for print publications or academic papers, you’re probably more familiar with writing long-form essays. Unfortunately, most of your readers will skip over your page if they see a wall of text.
	  
	  Instead, make long sets of paragraphs easier to scan by breaking them up with subheaders, lists, code samples, or graphics. Chapters [5](https://readwise.io/reader/document_raw_content/27434535#None) and [6](https://readwise.io/reader/document_raw_content/27434535#None) cover how to use code samples and visual content to break up your text. ([View Highlight](https://read.readwise.io/read/01gq3cd86rtwj9mvw4accvyjva))
	- Break up long documents
	  
	  It might be tempting to heap all of your content into a single document—but a single long document often tries to accomplish too many goals for too many different readers ([View Highlight](https://read.readwise.io/read/01gq3cem28m63p63824g9cmk78))
	- Strive for simplicity and clarity
	  
	  Short, concise documents are beautiful.
	  
	  As you draft a document, ask yourself: “Does this content satisfy my reader’s needs?” It might be tempting to add information like the history of a project or the design considerations you’ve made on a system, but they don’t belong in a procedural document. Put the history, design theory, and commentary for a document in a separate place and title and format it appropriately. ([View Highlight](https://read.readwise.io/read/01gq3cffy2jszz24sdc91f3krz))
	- Highlight missing content
	  
	  [TODO].
	  
	  We’ve all left TODO comments in code, and the same thing happens in documentation. As you’re writing, you may not have all the information you need to write a section, or you may realize there’s an essential part missing.
	  
	  When you notice a gap in content—that important information is missing—make a note of it and keep working on the parts you’re sure you can fill in. You can fill in the gap during a later round of revision or writing.
	  
	  Don’t get hung up on trying to write a document correctly and in order the first time through. Like code, writing is an iterative process. Write what you know, see what’s missing, research it, and write the new things you know. ([View Highlight](https://read.readwise.io/read/01gq3cgrh5ffzfey67hmsdry56))
- New highlights added [[2023-01-18]] at 10:51 PM
	- Write out of sequence
	  
	  You don’t have to write the first thing first. Sometimes, the first thing that people read—the introduction—is the last thing you write. Good introductions describe a document’s major themes, what readers will gain from reading the document, and why it matters. These topics aren’t always clear until you’re finished writing the steps or conceptual details that make up the body of the document. ([View Highlight](https://read.readwise.io/read/01gq40r654q4g9afhdnvht2jz9))
	- Working from templates
	  
	  If you’re making several similar documents that share the same document pattern, it’s worth creating a *template*. Templates provide reliable ways to create consistent documentation and simplify creating future documents.
	  
	  Templates create a consistent user experience. They make writing easier by letting you focus on content rather than structure. ([View Highlight](https://read.readwise.io/read/01gq40sb0w59jkcc627rqmzang))
	- Finishing your first draft
	  
	  Eventually, your draft document will be done: you’ve written down all the information your reader needs to reach your stated goal. To determine whether you’re done, ask yourself:
	  
	  •   Does the headline summarize the document’s goal?
	    
	  •   Do headings adequately summarize the document?
	    
	  •   Does your draft address your reader's needs from start to finish?
	    
	  •   Does the flow of information make sense to your reader?
	    
	  •   Does the draft address any issues you found in your friction log?
	    
	  •   Does your draft correctly follow any documentation patterns or a template?
	    
	  •   Have you tested and verified that any and all procedures work?
	    
	  
	  If you can answer yes to all of the questions above, then your first draft is done. Finishing a draft doesn’t mean that the content is ready to publish, but it does mean you’ve reached a major milestone in writing: you’ve conveyed all of the necessary information for your reader to succeed ([View Highlight](https://read.readwise.io/read/01gq40t4my7xgsqy6hyjabys2d))
	- Editing to meet your user’s needs
	  
	  The creative act of writing isn’t the same as the analytical act of reviewing and evaluating text. If drafting content is about getting all of your ideas down, editing is the process of looking at your documentation and making sure it’s meeting your users’ needs. Beyond grammar and readability, editing makes sure that text conveys information to your users in the clearest, fastest, and most helpful way possible. ([View Highlight](https://read.readwise.io/read/01gq40v99hx8az3mckpp9948dq))
	- Trying to write and edit at the same time is slower than doing each task separately ([View Highlight](https://read.readwise.io/read/01gq4143wvbxj47m5g5cdam187))
	- Like code reviews, editing is a collaborative process, where you share your content with others, test your assumptions, and gather feedback. This may feel vulnerable at first, but it’s also where the most learning happens. As you integrate the feedback you receive, you may see more elegant ways to approach the problem you’re documenting and write more effectively. ([View Highlight](https://read.readwise.io/read/01gq414qyg7g5eqe75sr01e34t))
	- Different approaches to editing
	  
	  When editing your work, it’s useful to focus on a single aspect of the document that you’re trying to improve. For example, “Is all of the technical information in this document correct?”, or “Is this document structured well?”. Trying to focus on all the factors of good documentation at once is both overwhelming and slow. It’s faster to break down the editing process into a series of *passes*, with each pass focused on one aspect of a well-edited document.
	  
	  Depending on your users and their needs, you may have different aspects that you focus on while editing your content. However, for most developer documentation, your editing passes should focus on:
	  
	  •   Technical accuracy
	    
	  •   Completeness
	    
	  •   Structure
	    
	  •   Clarity and brevity ([View Highlight](https://read.readwise.io/read/01gq415mf8qstq9pd2t92yttcq))
	- When editing for each of these qualities, read the document like someone encountering this information for the first time. When you know a product or technology well, it’s easy to make assumptions about familiar material, glossing over crucial introductory information that new readers need. The editing process is a great time to fill in these gaps and add information that helps users succeed ([View Highlight](https://read.readwise.io/read/01gq4169a0npwwec2kmmce8yr1))
	- Editing for technical accuracy
	  
	  When editing for technical accuracy, you’re editing for the correctness of your content. You should be able to answer the following questions:
	  
	  •   If someone follows these instructions, will they get the result you promised them?
	    
	  •   Is there any technical jargon or terms that might lead to confusion?
	    
	  •   Are code functions, parameters, and endpoints named and explained correctly? ([View Highlight](https://read.readwise.io/read/01gq416r0wfs5te8hj1zz3b4mr))
	- Editing for completeness
	  
	  When editing for completeness, you’re verifying that your content contains all of the necessary information for your user to be successful. It’s where you verify that there are no gaps in your content and that any [TODO] or [TBD] left in your draft is filled in.
	  
	  When editing for completeness, consider your user and how they might be using your software. If you’re developing on Linux, and they’re developing on a Mac, will your instructions still work? What if they’re not using the latest version of your software, but one that’s still supported—will there be any unexpected errors? ([View Highlight](https://read.readwise.io/read/01gq41ec5txstjyz5h8981ycbt))
	- Editing for structure
	  
	  The first thing a person sees when they open a document is the title, the headers, and the table of contents. These first few words are some of the most important parts of your document, giving your readers a set of signposts that point the way to the information they want. When you’re editing for structure, you’re verifying that these signposts are correct and that it’s clear to a reader what this document is about and how the topic is broken down.
	  
	  As you edit for structure, you’re trying to answer the following questions:
	  
	  •   Is it clear from the title and headers what the document is about?
	    
	  •   Is the document organized in a consistent and logical way?
	    
	  •   Are there sections in this document that should be put in another document?
	    
	  •   If a template exists, does the document follow it? ([View Highlight](https://read.readwise.io/read/01gq41snsf9mye9tg1ttxgmmd1))
	- Clearly state any prerequisite steps. For example, “You must be an administrator to complete these steps,” or “This document assumes you have finished configuring your API.”
	  
	  Likewise, if there are common next steps or additional information that a reader might need after reading your document, you should list those links. These signposts let your user know where they are on their journey ([View Highlight](https://read.readwise.io/read/01gq41x90aycx6ck3a2tp1txnk))
	- Editing for clarity and brevity
	  
	  When editing for clarity and brevity, you’re reviewing your document on a line-by-line basis for how easily understandable each sentence and paragraph is. Reword awkward phrases, remove any duplicate information, and cut unnecessary words. Think of editing for clarity and brevity as code refactoring for documentation.
	  
	  Editing at this stage includes all the classic elements of editing language, correcting for grammar, tone, and conciseness. Tools like spelling and grammar checkers can perform some of this work, but you should also review your document in its entirety. As you read each section of your document, ask yourself the following:
	  
	  •   Is this as clear as it can be?
	    
	  •   Are there terms used inconsistently that I should correct?
	    
	  •   Are there unnecessary words or phrases that I can cut?
	    
	  •   Are there any idioms, metaphors, or slang that could confuse readers?
	    
	  •   Am I using any biased language that should be avoided? ([View Highlight](https://read.readwise.io/read/01gq41y4nv5vyjcjdt8r33zxew))
	- Make your content as short and to the point as possible. While you’re editing, you might find yourself cutting a lot of content. This is a good thing! It means your reader will get to the right information quickly, without having to scan through your document ([View Highlight](https://read.readwise.io/read/01gq41ygqtaqjzd07tqj2wc0za))
	- Creating an editing process is similar to creating a code review process, and it has similar benefits. An editing process speeds up the length of time it takes to edit a document, allowing someone with a fresh perspective to give you objective feedback. It also helps share knowledge across reviewers and helps establish standards across documentation within your team.
	  
	  A typical editing process is shown in Figure [4-1](https://readwise.io/reader/document_raw_content/27434535#Fig1).
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/27434535/Aimages_505277_1_En_4_Chapter_505277_1_En_4_Fig1__66JKJ9h.jpg) ([View Highlight](https://read.readwise.io/read/01gq41za2gs6x64gmyvbe1nk0f))
	- One way to make reviewing your own content easier is to use an editing checklist. An editing checklist helps keep you on track, reviewing what’s important without getting bogged down in trying to create a perfect sentence. A checklist might look something like this:
	  
	  •   Title is short and specific
	    
	  •   Headers are logically ordered and consistent
	    
	  •   Purpose of document is explained in the first paragraph
	    
	  •   Procedures are tested and work
	    
	  •   Any technical concepts are explained or linked to
	    
	  •   Document follows structure from templates
	    
	  •   All links work
	    
	  •   Spelling and grammar checker has been run
	    
	  •   Graphics and images are clear and useful
	    
	  •   Any prerequisites and next steps are defined ([View Highlight](https://read.readwise.io/read/01gq41zya28fyvtjjcr7qw2w26))
	- Requesting a peer review
	  
	  Peer reviews for documentation are similar to code reviews for code. You’re requesting that someone review your content and make sure it’s useful and relevant for your audience. In the introduction to this chapter, peer review is exactly what Karthik is doing for Charlotte. ([View Highlight](https://read.readwise.io/read/01gq4285e2qa6hcytb2mbvr4t8))
	- In addition to requesting specific feedback from your review, it’s important to specify how you’d like to receive your feedback. Do you prefer to receive marked up paper, inline comments, or sidebar notes in a shared document? In peer reviews, the goal is to reduce friction, so your reviewer can comment efficiently and you can incorporate feedback easily. ([View Highlight](https://read.readwise.io/read/01gq428p97ehnqbt6mk9vye83g))
	- For a first draft review, you probably want a reviewer on your team who is familiar with the product or procedure you’re documenting, similar to how Karthik reviews Charlotte’s work. As you get closer to publication, you may want additional reviews from people who are more like your target audience, to make sure you’ve written what they need to understand ([View Highlight](https://read.readwise.io/read/01gq429gs8zmxznshf0v5mq24j))
- New highlights added [[2023-01-18]] at 11:51 PM
	- Technical reviews are a specific type of peer review to add or confirm details from a technical expert on a particular topic. Technical reviews are particularly important when you’re documenting an integration of two or more technologies, where you might be an expert on one but not the other. ([View Highlight](https://read.readwise.io/read/01gq42wv9vvrktxr7pmcv6cjjf))
	- Receiving and integrating feedback
	  
	  After you request and receive reviews, you’ll have a pile of scribbles, pull requests, and other notes on how people want your text changed. What’s next?
	  
	  First, take a deep breath. Feedback about writing can feel personal. Remember that reviews are intended to help you improve your content, not to pick on you as a person. The goal of your document is to communicate knowledge effectively to your readers. Ultimately, reviews help you help your readers and get you closer to your goal. ([View Highlight](https://read.readwise.io/read/01gq42xe324wt1vx3b4z76r8p9))
	- Next, go through each reviewer’s comments in turn. If you start with the person who sent in the most feedback, you’re likely to preemptively address feedback from subsequent reviews. If you try to incorporate all feedback simultaneously on a single item, you’re more likely to lose track of edits and progress while attempting to resolve contradictory advice ([View Highlight](https://read.readwise.io/read/01gq42ysmt7777wxvf31j4e2cg))
	- You should consider each piece of feedback you receive—but that doesn’t mean you have to accept it! Not all suggestions are helpful or necessary, even though your reviewer offered feedback with good intentions. Whether or not you accept their feedback, it’s important to acknowledge a reviewer’s help. Likewise, don’t reject feedback out of hand. It’s important to review all feedback to understand your reviewers’ concerns and maximize your document’s quality.
	  
	  If you do receive contradictory feedback, consider what helps your user the most. If you get a suggestion that you should have more technical details from one reviewer, while another reviewer argues for less, then consider this: what does a user using this doc need to know? ([View Highlight](https://read.readwise.io/read/01gq42z4r1npgdwvjpwx3rgd97))
	- Giving good feedback
	  
	  If you expect to get good feedback from your reviewers, it’s important to know how to give good feedback as well. Peer reviews work best when you approach them with a constructive mindset. You’re not fixing someone else’s mistakes; you’re adding to their understanding. ([View Highlight](https://read.readwise.io/read/01gq42zjrv3rbktngbcshgj5jm))
	- Consider the animation studio Pixar’s method of reviewing and critiquing work, where feedback on creative or technical work must follow a rule called *plussing* ,[1](https://readwise.io/reader/document_raw_content/27434535#Fn1) which is:
	  
	  > You may only criticize an idea if you also add a constructive suggestion.
	  
	  When using the plussing method of offering feedback, focus on the idea, not the person. For example, start by saying something like, “I found this part unclear,” rather than, “You got this wrong.”
	  
	  Follow your critique with specific suggestions for improvement. Constructive suggestions provide additional context for what you think would solve the problem. This “adding on” is why Pixar called the system “plussing.” For documentation, it’s helpful to suggest a specific way to rewrite an awkward sentence or a poorly defined concept. The more specific you make your constructive suggestion, the better your feedback becomes—and the more you help your users.
	  
	  If you’re adding a lot of constructive feedback, give the original writer time to consider your suggestions. People need time to receive, evaluate, and implement feedback. Don’t expect an immediate response, especially if there are multiple reviewers.
	  
	  In short, to provide good feedback:
	  
	  •   Focus on the idea, not the person
	    
	  •   Follow up with a constructive suggestion
	    
	  •   Allow the recipient time to react to your feedback ([View Highlight](https://read.readwise.io/read/01gq43c89frzhcdmp69pcb7gqx))
	- One more note about feedback: it’s okay to point out things you like! For example, an elegant explanation of a deeply technical concept is worth pointing out and celebrating. In addition, pointing out great writing makes it easier for others to emulate ([View Highlight](https://read.readwise.io/read/01gq43gyrvtzg6cgkwsj69w7cb))
	- Why visual content is hard to create
	  
	  Like written documentation, the most effective visual content is something the reader barely notices. It doesn’t require them to stop in order to think or be aware of the fact they are consuming anything at all. When visual content works, it conveys information so quickly that the reader sweeps through their task. In the words of Edward Tufte, statistician, pioneer of data visualization, and all-round visual content expert, “Graphical excellence is that which gives to the viewer the greatest numbers of ideas in the shortest time with the least ink in the smallest space.”[4](https://readwise.io/reader/document_raw_content/27434535#Fn4) ([View Highlight](https://read.readwise.io/read/01gq446p9ck04mm6ehh5tschy6))
	- In Chapter [3](https://readwise.io/reader/document_raw_content/27434535#None), we discussed how using a variety of paragraphs, bullets, and numbered steps helps break up walls of text. Visual content is another way to bring variety to documentation and with great effect. In one study, readers who followed instructions with illustrations were 323% better at completing those instructions than readers with no illustrations to help.[5](https://readwise.io/reader/document_raw_content/27434535#Fn5) ([View Highlight](https://read.readwise.io/read/01gq447wbrkjbpajyf62a6r71j))
	- Ineffective visual content interferes with the transfer of information, usually due to a lack of:
	  
	  •   Comprehension
	    
	  •   Accessibility
	    
	  •   Performance
	    
	  
	  It doesn’t matter whether you’re looking at screenshots, illustrations, graphs, videos, infographics, diagrams, or photographs. All visual content types, and all documentation including them, sometimes fail to help because of these issues. ([View Highlight](https://read.readwise.io/read/01gq448k6ch2ty3942yym6gw0v))
	- Comprehension
	  
	  Eye tracking studies by the Nielsen Norman Group show readers pay closer attention to images that contain information relevant to them. Other images, however beautifully designed, are ignored.[7](https://readwise.io/reader/document_raw_content/27434535#Fn7) ([View Highlight](https://read.readwise.io/read/01gq44909vdrfpnqy5z9qnm7q6))
	- Using screenshots
	  
	  Screenshots can be a useful addition to documentation, particularly to show a user interface (UI). If you think a screenshot would be useful to your readers, make sure they:
	  
	  •   Never appear without introduction or reference in the text.
	    
	  •   Appear close to the instructions or related text.
	    
	  •   Are clean and clutter free—do not include anything in your screenshot not part of your UI.
	    
	  •   Include all relevant parts of the UI with enough context to reassure the reader they’re on the right screen.
	    
	  •   Not too big—your readers need to be able to read all parts of the image.
	    
	  •   Not too small—your readers need to be able to correlate the screenshot to the UI they experience. ([View Highlight](https://read.readwise.io/read/01gq45cffsdhbrw0sggm949z3d))
	- Swimlanes
	  
	  Swimlane diagrams are particularly useful for situations with multiple contributors or acting parts. Much like a flowchart, they show a process from beginning to end. Each actor or contributor has its own lane, and each step of a process takes place in one of those lanes. In doing so, it’s easier to see at glance who or what is responsible for each step. ([View Highlight](https://read.readwise.io/read/01gq45e6gm7py6a4rkrktd66dk))
	- Building a content release process
	  
	  Just like your organization (hopefully!) has a software release process, you should also build a release process for your documentation. Your content release process is the plan for publishing your content. It contains the timeline for publishing, assigning responsibilities for final content review and publication, and designating where to publish content.
	  
	  Your content release process should answer the following questions:
	  
	  •   When are you going to publish your content?
	    
	  •   Who is responsible for final review and publication?
	    
	  •   Where are you going to publish your content?
	    
	  •   What additional software tools are needed to publish the content?
	    
	  •   How will you announce your new content to your users? ([View Highlight](https://read.readwise.io/read/01gq45fcwnjzkh1hwa0pmhggmq))
	- Creating a publishing timeline
	  
	  A publishing timeline is a way to make sure that all the essential tasks of publishing are included and that you have enough time to complete them. Doing user researching, creating a documentation plan, drafting documentation and getting reviews all takes time. A Gantt chart is a useful way to represent the planning that goes into a full release (Figure [7-1](https://readwise.io/reader/document_raw_content/27434535#Fig1)). For example, if you need three days for the web team to verify and upload something, two days to incorporate feedback, and one week to edit, you can see that you need to have the draft ready for editing two weeks before your publication target.
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/27434535/Aimages_505277_1_En_7_Chapter_505277_1_En_7_Fig1__h0ArABW.jpg)
	  
	  Figure 7-1
	  
	  A Gantt chart with a publishing timeline ([View Highlight](https://read.readwise.io/read/01gq45pwnma31c3xvst88yrvcw))
	- Finalize and approve publication
	  
	  You should assign a single, final approver who is responsible for allowing or halting a documentation release. This approver should be listed in the publishing timeline, and they should have final say in the amount of content and its level of quality before you launch. No document is ever going to be perfect, but no released document should be harmful. Be sure you have a responsible party for that decision. ([View Highlight](https://read.readwise.io/read/01gq45qrb3byhd46mbhysyf262))
	- If your organization wouldn’t release code without a peer review and some automated testing, you shouldn’t release your documents that way, either. The simplest way to ensure parity would be to use your code review process for documentation. If it’s going to be part of your codebase, it certainly needs to pass all the integration tests that your code does. If you have a culture of peer review or QA, your docs should be held to the same standard. ([View Highlight](https://read.readwise.io/read/01gq45qgr0zw3a15tb2kr2x5y8))
- New highlights added [[2023-01-19]] at 12:51 AM
	- Planning for the future
	  
	  Your documents are living documents, just like your code. You need to have some plans for what will happen to them ([View Highlight](https://read.readwise.io/read/01gq45y21artq7mp8ecxt02bax))
	- Listening to your users
	  
	  Documentation is one of the primary ways you communicate with your users, and users expect to be able to communicate back. Collecting user feedback can help you learn where your product and documentation succeed and where you need to make improvements. It also helps you validate (or correct) all the assumptions you’ve made about your users in your initial user assessment (see Chapter [1](https://readwise.io/reader/document_raw_content/27434535#None)) ([View Highlight](https://read.readwise.io/read/01gq45ysznc381ydrgw0vdy9mh))
- New highlights added [[2023-01-19]] at 1:56 PM
	- Collect document sentiment
	  
	  *Document sentiment* is how readers feel about your documentation. You can discover and measure document sentiment through a simple survey or by using embedded code on a page that prompts a user to indicate by clicking a simple yes or no whether the page was helpful (Figure [8-1](https://readwise.io/reader/document_raw_content/27434535#Fig1)).
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/27434535/Aimages_505277_1_En_8_Chapter_505277_1_En_8_Fig1__iqeLpLO.jpg)
	  
	  Figure 8-1
	  
	  A document sentiment tool on a Google page ([View Highlight](https://read.readwise.io/read/01gq58mz1zaqwq8x0m2zzzy5bc))
	- There are significant limitations to measuring sentiment. You need to collect a large number of responses from a yes/no sentiment survey in order for data to be useful. The more responses you get, the more confident you can be that the data actually represents your users. You also have to wait after making changes before collecting more responses to measure whether changes had an effect. ([View Highlight](https://read.readwise.io/read/01gq58nqdvxrpb80y523q00awh))
- New highlights added [[2023-01-19]] at 10:49 PM
	- Create user surveys
	  
	  Customer surveys let you ask users specific questions about your product and documentation in an automated way that’s easy to aggregate. You can embed shorter surveys in your documentation, either as a link or as a popup. Longer surveys can be emailed to your customers. ([View Highlight](https://read.readwise.io/read/01gq6k8090bmc2rn3ak1qftvtw))
	- Regardless of how you reach your users with a survey, it’s important to keep your survey focused on a specific set of questions with measurable results. For example, if Karthik wanted to understand user satisfaction with Corg.ly’s documentation, he might create a survey that asked the following questions:
	  
	  1.  1.
	    
	    How satisfied are you with Corg.ly’s documentation?
	    
	  2.  2.
	    
	    Are you able to find the information you were looking for?
	    
	  3.  3.
	    
	    How much time did it take you to find this information?
	    
	  4.  4.
	    
	    Did this effort match your expectations?
	    
	  5.  5.
	    
	    What can we do to improve our documentation? ([View Highlight](https://read.readwise.io/read/01gq6k87ed958q7kqccv9e0vhh))
	- Converting feedback into action
	  
	  When you gather data from the various feedback channels you create, you’re amassing information on the changes your users want. Some feedback will be concrete and easily actionable, like, “This particular code sample in this particular document needs an update.” Other feedback will be more complicated or require you to consider whether you need to improve your code or revise your information architecture.
	  
	  You need a process to convert user feedback into action, one that allows you to prioritize issues that are most important to your users, and backlog the issues you can ignore or defer to another time.
	  
	  The name for this process—of sorting and prioritizing feedback—is *triage*. Not all opinions deserve consideration, and not every great idea deserves immediate action. Triage helps you choose the most valuable improvements to make with limited resources ([View Highlight](https://read.readwise.io/read/01gq6kcc2cpajqwt8npj19wpg3))
	- Triaging feedback
	  
	  As in healthcare settings that evaluate patients upon arrival to make sure each patient receives an appropriate level of care, user feedback requires similar triage . Each feedback issue should be quickly evaluated to see if you can answer the following questions:
	  
	  1.  1.
	    
	    Is the issue valid?
	    
	  2.  2.
	    
	    Can it be fixed?
	    
	  3.  3.
	    
	    How important is the issue?
	    
	  
	  The following sections dive into each of these questions, defining specific requirements for answers at each step. Answering these questions helps you separate actionable user feedback from feedback that needs more information and feedback that can be ignored. Applying a standard triage process is critical because it:[3](https://readwise.io/reader/document_raw_content/27434535#Fn3)
	  
	  •   Speeds up the response times to user issues
	    
	  •   Prevents requested work from lingering endlessly
	    
	  •   Builds a standard set of priorities for issues
	    
	  •   Directs limited resources toward the most necessary and impactful changes
	    
	  
	  Triaging feedback for documentation is no different from triaging code or product issues. If you already have a system for managing issues, you should apply that system to managing your user feedback as well. ([View Highlight](https://read.readwise.io/read/01gq6kd68rsxx2v1h99b8fqbsy))
- New highlights added [[2023-01-19]] at 11:51 PM
	- Step one: Is the issue valid?
	  
	  It’s important to take a “trust but verify” approach when evaluating user feedback issues. Users have good intentions when submitting feedback, but sometimes their feedback isn’t relevant to documentation, or the issue they’re describing has already been fixed.
	  
	  The first step to triaging user feedback is to determine whether it’s *valid*. In this case, validity means the issue is relevant to documentation ([View Highlight](https://read.readwise.io/read/01gq6mrbs6rw5fd76whtky6xq7))
	- Step two: Can the issue be fixed?
	  
	  Once you’ve determined that the feedback is applicable to documentation, the next step is to determine whether the feedback is *actionable—*that is, whether you can act to change the documentation for the better.
	  
	  For a documentation issue to be actionable, it must be:
	  
	  •   Original
	    
	  •   Reproducible
	    
	  •   Scoped ([View Highlight](https://read.readwise.io/read/01gq6mz71hy1r7cb478zvbr8p1))
	- Finally, scope the issue to something that’s possible to fix. Feedback that’s too general in scope (e.g., “These docs didn’t help”) isn’t feedback on which you can act. The same is true for feedback that’s too large in scope (e.g., “Rewrite the entire security section”).
	  
	  Narrow the scope of an issue to something you can fix. For example, “The setup section for audio translation is difficult to follow and should be rewritten.” Limit the scope of each issue to a specific documentation fix that directly improves the user experience. Break down any required changes into smaller steps until you’ve created a well-bounded set of actions to take ([View Highlight](https://read.readwise.io/read/01gq6mzz2wxffahjw4gx9agprn))
	- Step three: How important is the issue?
	  
	  The last step of triage is to assign a priority to the issue. An issue’s priority encapsulates how important the issue is and how quickly it needs to be fixed.
	  
	  Most projects have a standard set of priorities for issues. For example, Table [8-1](https://readwise.io/reader/document_raw_content/27434535#Tab1) lists a set of issue priorities for the Chromium project.[4](https://readwise.io/reader/document_raw_content/27434535#Fn4)
	  
	  Table 8-1
	  
	  Issue priorities
	  
	  Priority
	  
	  What it means
	  
	  **P0**
	  
	  Emergency: requires immediate resolution
	  
	  **P1**
	  
	  Needed for upcoming release
	  
	  **P2**
	  
	  Wanted for upcoming release (but not required)
	  
	  **P3**
	  
	  Not time sensitive ([View Highlight](https://read.readwise.io/read/01gq6n1phdwcqr8k6m79hk93rf))
	- Following up with users
	  
	  As stated at the beginning of the chapter, feedback is how you have a conversation with your users. It’s important to communicate with users about how you’re taking action on the issues they raised.
	  
	  For example, if a user reports an issue that you can’t reproduce, the quickest way to address the issue is to ask for more specifics, including any code the user can provide you to help diagnose the issue and any information about their specific environment that might not be covered by your documentation. Asking users for more information about their feedback is quicker than trying to figure out the reported issue on your own.
	  
	  It’s also important to follow up with users when you fix the issue they reported. Some issue trackers let you follow up with the user who submitted the issue. Otherwise, you can reach out to them directly and thank them for their feedback. If a user goes above and beyond in their feedback, you can praise them in release notes or blog posts after you fix the issue.
	  
	  Let your users know that you’ve listened to their feedback. It takes time for users to submit feedback, so it builds trust when you let your users know they’ve been heard ([View Highlight](https://read.readwise.io/read/01gq6n2v6xaya14exjcfn55xt6))
	- Understanding documentation quality
	  
	  Before you can measure document quality, you must first define “quality.” Luckily, a group of writers and engineers at Google worked on this very question: they evaluated documentation quality with similar methods for evaluating code quality.[1](https://readwise.io/reader/document_raw_content/27434535#Fn1) The definition for documentation quality they created is very simple:
	  
	  > *A document is good when it fulfills its purpose.*
	  
	  If a document is good when it fulfills its purpose, then *what is its purpose*? The purpose of your documentation should align with the purpose of your code: to drive specific user behavior and accomplish the goals of your organization. Lifting vocabulary directly from the field of software testing, the group broke down documentation quality into two fundamental categories:
	  
	  •   **Functional quality**, which describes whether or not a document accomplishes its purpose or goal
	    
	  •   **Structural quality**, which describes whether a document is well written and well structured ([View Highlight](https://read.readwise.io/read/01gq6n7wvv40wxacfbp12r42en))
	- Functional quality
	  
	  The functional quality of a document describes whether or not the document accomplishes the goal it sets out to achieve. It examines at a fundamental level whether or not the document *works.*
	  
	  Functional quality is difficult to measure holistically, but it’s the more important metric because it more closely aligns with the document’s purpose. The functional quality of documentation can be broken down into the following categories:[2](https://readwise.io/reader/document_raw_content/27434535#Fn2)
	  
	  •   Accessible
	    
	  •   Purposeful
	    
	  •   Findable
	    
	  •   Accurate
	    
	  •   Complete ([View Highlight](https://read.readwise.io/read/01gq6n9vv73evq03cdhgfdtx95))
	- Accessible
	  
	  Accessibility is the most essential aspect of functional quality. If your readers can’t access and understand your content on a fundamental level, they won’t be able to accomplish their goals.
	  
	  For documentation, accessibility includes language, reading level, and screen reader access.
	  
	  One of the most important parts of accessibility is writing in the language of your readers. In the United States, for example, census records show that more than 300 languages are spoken within the country, and 8% of the population has limited English proficiency.[3](https://readwise.io/reader/document_raw_content/27434535#Fn3) ([View Highlight](https://read.readwise.io/read/01gq6nqv5z9cbsztnz10y0729s))
	- Reading level is another way to measure the accessibility of your documentation. In general, technical documentation should be written to a tenth grade level, including titles, headers, and paragraphs. This helps your readers understand your content quickly and pushes you, the writer, to use clear language and avoid complex technical jargon ([View Highlight](https://read.readwise.io/read/01gq6nrj7q8g0g8w0xepcxz6zd))
	- Purposeful
	  
	  For a document to be useful, it must clearly state its purpose or goal and then work to fulfill it. Your document should, in both its title and first paragraph, state the purpose of the document and what it will help your reader accomplish. These goals should align with both the goals of your organization and the goals of your reader. ([View Highlight](https://read.readwise.io/read/01gq6pcveahx829p502txbp0a5))
	- For example, let’s say Charlotte is creating a document to help developers get started with the Corg.ly API. First, the document title should explicitly be the goal of the document for the reader, something like “Getting started with the Corg.ly API.” Next, the document should explicitly state at the beginning what the document covers, such as “Authenticating with the Corg.ly API” and “Making your first Corg.ly API call.” ([View Highlight](https://read.readwise.io/read/01gq6phegqe3nknshzqzyxydp6))
	- Findable
	  
	  Findability is the measure of how easily your readers navigate to and through your content.
	  
	  You might think of findability as something that exists outside of your documentation, something that can be fixed with a good site architecture and a good search engine. Although good site architecture helps (see Chapter [10](https://readwise.io/reader/document_raw_content/27434535#None)), search engines can direct users to the wrong page within your site or miss your site entirely. Readers searching for the right content can be stymied if your content doesn’t have the keywords they expect or if there are many similar sites with similar content. Understanding what your users are searching for, standardizing on search keywords, and monitoring how users find and enter your site all help increase findability ([View Highlight](https://read.readwise.io/read/01gq6pjbqvw6fkt177s9523tq6))
	- Accurate
	  
	  Accuracy is the measure of how correct and credible the content is in a document. A document with high accuracy has correct and up-to-date technical explanations of the code it’s describing, along with working code samples and command line examples. A document with low accuracy might have several issues filed against it (see Chapter [9](https://readwise.io/reader/document_raw_content/27434535#None)) and might contain code samples that are broken or superseded by new versions of your product.
	  
	  Low-accuracy documentation leads to user frustration, as well as a loss of trust in both your documentation and product. How often have you searched for an answer to a problem and found a promising document, only to find out that the solution didn’t work? ([View Highlight](https://read.readwise.io/read/01gq6qyyve062dphsjv4thcf87))
	- Complete
	  
	  A document is complete if it contains all of the information necessary for the reader to succeed. For a task-driven document, completeness means:
	  
	  1.  1.
	    
	    Listing all prerequisites that readers should follow.
	    
	  2.  2.
	    
	    Documenting all tasks required to finish the task.
	    
	  3.  3.
	    
	    Defining next steps the reader should take ([View Highlight](https://read.readwise.io/read/01gq6qzrv84zeqgyn4emw06d1e))
	- Structural quality
	  
	  The structural quality of a document describes how well it’s written. This includes sentence, paragraph, and header structure, quality of language, and accuracy of grammar. Structural quality encapsulates how easy a document is to read.
	  
	  This book uses the “three Cs” of good writing to define structural quality:
	  
	  •   Clear
	    
	  •   Concise
	    
	  •   Consistent ([View Highlight](https://read.readwise.io/read/01gq6r0dj2pw7y9dttpdd5bg2w))
	- Clear
	  
	  Clarity is the measure of how easy your document is to understand. For documentation, clarity refers to how easily your reader can take in the information you’ve provided them and how confident they are that they will succeed.
	  
	  At a holistic level, clear documentation has:
	  
	  •   Well-defined and well-ordered headers that break down a topic into logical sections
	    
	  •   Headers ordered chronologically for tasks and each step indicating the desired outcome
	    
	  •   Unambiguous results for each step in a process
	    
	  •   Steps organized in a way your readers understand
	    
	  •   Content that calls out any places where a reader might get stuck
	    
	  •   Definitions of any errors that users may encounter
	    
	  
	  On a sentence-by-sentence level, clear documentation avoids unnecessarily long words or jargon that your reader might not understand. If you have to use unfamiliar words, define them for your readers ([View Highlight](https://read.readwise.io/read/01gq6r3rdctkd4bc9xdtz7h8gc))
	- Concise
	  
	  A good definition of concision (or conciseness) is *brief but comprehensive*. At a holistic level, a concise document contains only information that’s relevant to a reader and their goals. Remove anything that gets in the way of a reader’s understanding, and link to anything that is relevant but not immediately necessary ([View Highlight](https://read.readwise.io/read/01gq6r50w9sjb4k81cs5zda45z))
	- Consistent
	  
	  Document consistency means that the structure of your content, the concepts that you introduce, and your word choice are the same throughout your documentation. At a holistic level, consistent documentation has consistent titles, headers, paragraph structures, and lists. The content uses patterns that a reader can easily follow and use to skim documentation and quickly find what they need. ([View Highlight](https://read.readwise.io/read/01gq6r67mdtmjk46vgzhabk7j1))
- New highlights added [[2023-01-20]] at 12:51 AM
	- How functional and structural quality relate
	  
	  Ideally, your documentation should have both high structural quality and high functional quality. However, functional quality is more important. A well-structured, well-written document that doesn’t accomplish its goal is a poor piece of documentation. A document with structural issues that still accomplishes its goal is a good document.
	  
	  Here’s a good way to think about it:
	  
	  •   Low functional quality + high structural quality = poor overall quality
	    
	  •   High functional quality + okay structural quality = good overall quality ([View Highlight](https://read.readwise.io/read/01gq6rdm9m91z2r93f5b7t9ane))
	- Creating a strategy for analytics
	  
	  For documentation to be effective, it must align your technical and business goals with the goals of your reader. As stated at the beginning of the chapter, “*A document is good when it fulfills its purpose.”*
	  
	  An analytics strategy helps you recognize how your documentation goals align with the larger goals of your readers and your organization. A strategy allows you to focus on the metrics that are important to what you want to improve while ignoring the rest.
	  
	  To create an effective analytics strategy, clearly define the following:
	  
	  •   Your organization’s goals and how they’re measured
	    
	  •   Your reader’s goals and how they’re measured
	    
	  •   Your documentation goals and how they’re measured
	    
	  
	  Your documentation should help readers accomplish their goals, which in turn help your larger organization accomplish its goals. These metrics should all align with one another, so it’s useful to look at all of these together.
	  
	  Organizational goals and reader goals are covered in Chapter [1](https://readwise.io/reader/document_raw_content/27434535#None), but as your set of documentation grows, and your documentation becomes more specialized, it’s useful to revisit these goals before starting to measure quality. ([View Highlight](https://read.readwise.io/read/01gq6rejyd7hsddsskhr66zc8k))
	- Organizational goals and metrics
	  
	  Organizational goals are specific behaviors the organization wants from its users. These goals are usually tied to revenue. They focus on increasing revenue through adding users, engagement, and retention. They can also focus on reducing costs by addressing support needs and customer questions at scale. These goals include things like:
	  
	  •   Recruiting and onboarding new users
	    
	  •   Encouraging existing users to adopt new features
	    
	  •   Getting users to complete a specific task
	    
	  •   Retaining existing users
	    
	  •   Addressing users’ support needs and product questions ([View Highlight](https://read.readwise.io/read/01gq6sk2nh51yrft76wbhrzsc5))
	- User goals and metrics
	  
	  While the business goals of your organization are focused on revenue and adoption, your readers’ goals are focused on completing specific tasks. You already outlined these goals in Chapter [1](https://readwise.io/reader/document_raw_content/27434535#None), when you were researching your readers’ needs. It’s useful to highlight them again as you’re considering documentation quality.
	  
	  Your readers’ goals are smaller and more specific than your organizational goals. They can include things like “Downloading the SDK,” “Authenticating with your service,” or “Troubleshooting an Error.” They’re also more subjective in measurement. ([View Highlight](https://read.readwise.io/read/01gq6sn6hqnpmn4xh5fg6kmjr6))
	- Defining how you organize your content helps you grow your documentation in a structured and sustainable way. How you organize content conveys meaning and purpose to your readers. The organizational structure you apply to your documentation is called its *information architecture* ([View Highlight](https://read.readwise.io/read/01gq6sqcw1eezft8xfzmx91gk6))
	- A clearly defined information architecture helps you and your fellow developers add pages to your site and scale up the number of documents you publish without confusing your readers or making your site difficult to navigate ([View Highlight](https://read.readwise.io/read/01gq6sv6z1hkb83vfqkwhvvev2))
	- You can help your users navigate your site faster and more intuitively by organizing information into a meaningful structure, intentionally surfacing your pattern of organizing content, and highlighting information that is most relevant to your users. Doing this helps your readers build a map in their mind, or a *mental model* , of how your content is organized.
	  
	  Planning your information architecture, and helping your readers build a mental model of your content means incorporating new elements into your set of documentation, including:
	  
	  •   Site navigation and organization
	    
	  •   Landing pages
	    
	  •   Navigation cues ([View Highlight](https://read.readwise.io/read/01gq6sxaamcrka21bdjk25szdb))
	- Site navigation and organization
	  
	  Your site navigation is both a map for your existing content and your blueprint for where to publish additional content. It’s the most important part of your information architecture, so it’s important to build it thoughtfully.
	  
	  There are three basic ways to organize your content: sequences, hierarchies, and webs.[2](https://readwise.io/reader/document_raw_content/27434535#Fn2) These architectures govern the possible ways for you to create a consistent model for users to navigate your site, and for you to add additional pages.
	  
	  Sequences
	  
	  Sequential structures are the most familiar to any reader (Figure [10-1](https://readwise.io/reader/document_raw_content/27434535#Fig1)). Any book you read is organized in sequential order—one page after another. Sequential ordering may be chronological, like the steps required to use an API, or may be alphabetical, like an index or glossary. Sequential order requires you, the writer, to put the pages in the most effective order for your reader.
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/27434535/Aimages_505277_1_En_10_Chapter_505277_1_En_10_Fig_Ruew7fC.jpg)
	  
	  Figure 10-1
	  
	  Sequential structure ([View Highlight](https://read.readwise.io/read/01gq6sxwv6sg1r99f3r3chvfps))
	- Hierarchies
	  
	  Hierarchical structure is similar to a family tree or an organizational chart (Figure [10-2](https://readwise.io/reader/document_raw_content/27434535#Fig2)). Like a family tree, content has a parent/child relationship between pages. In a hierarchical structure, you start from one broad idea and narrow down into more detailed and increasingly specific information. One main topic is supported by multiple related subtopics beneath it.
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/27434535/Aimages_505277_1_En_10_Chapter_505277_1_En_10_Fig_qxPxDS1.jpg)
	  
	  Figure 10-2
	  
	  Hierarchical structure ([View Highlight](https://read.readwise.io/read/01gq6sy6rz2ygysqpsycy13n2g))
	- Webs
	  
	  Webs are interconnected, non-hierarchical patterns of pages where each page links to one or more pages (Figure [10-3](https://readwise.io/reader/document_raw_content/27434535#Fig3)). This allows your user to decide how to view and organize your content. Wikipedia, for example, has a web organization. Each page is at the same level in the hierarchy, and is linked to one or more pages in the set, allowing you to seamlessly read from one topic to the next, traversing any linked order you choose.
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/27434535/Aimages_505277_1_En_10_Chapter_505277_1_En_10_Fig_NQ6HDFW.jpg)
	  
	  Figure 10-3
	  
	  Web structure ([View Highlight](https://read.readwise.io/read/01gq6synzqzbqvysb8nacewa7d))
	- Although there are many different ways to categorize information, your information architecture should always feel consistent and familiar for a reader to navigate. For example, if Corg.ly had two services, one that translates dog barks through an app on phones carried by humans, and one for translation collars worn by dogs, it might make sense to have a document structure and navigation that looks like Figure [10-5](https://readwise.io/reader/document_raw_content/27434535#Fig5).
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/27434535/Aimages_505277_1_En_10_Chapter_505277_1_En_10_Fig_OGheZeP.png)
	  
	  Figure 10-5
	  
	  Sample architecture ([View Highlight](https://read.readwise.io/read/01gq6szdtd89z6h97bsy1emv6p))
	- Landing pages
	  
	  *Landing pages* are pages that route users to the right content with minimal reading required, building trust with users by saving them time. A landing page should be short, easy to scan, devoid of jargon, and surface useful information for your reader. Landing pages are equivalent to a huge signpost in the road that points to the possible directions your users can go.
	  
	  To make a good landing page, you must prioritize your users’ needs first. Your landing page should highlight the most important and relevant information for your users. Create guardrails to guide your users down the right path, and hide complexity that most users don’t need right away. Your user research (from Chapter [1](https://readwise.io/reader/document_raw_content/27434535#None)) and your company’s strategic goals can help define the top-level categories on your landing page ([View Highlight](https://read.readwise.io/read/01gq6t04wmdqte07wqvhx5s30t))
	- For example, the main landing page for Corg.ly documentation might have three major sections on the main page, each targeted at the most common user tasks (Figure [10-6](https://readwise.io/reader/document_raw_content/27434535#Fig6)):
	  
	  •   A Getting Started section that includes an overview of the Corg.ly service and a quick tutorial.
	    
	  •   Two of the most used how-to guides for what users want to accomplish with Corg.ly: “Translating barks to English”, and “Translating English to barks”.
	    
	  
	  ![](https://readwise-assets.s3.amazonaws.com/media/reader/parsed_document_assets/27434535/Aimages_505277_1_En_10_Chapter_505277_1_En_10_Fig_5X14SOA.png)
	  
	  Figure 10-6
	  
	  Example landing page ([View Highlight](https://read.readwise.io/read/01gq6t45g95rebyt6qxjvsc52s))
	- Navigation cues
	  
	  Most users will arrive at your documentation through search, by putting terms in a search engine and clicking on the first, most relevant result. This might get them to the right piece of information, but more likely than not, it will simply get them close.
	  
	  Unfortunately, close isn’t helpful if users don’t know how close they are, or how to navigate from a page that’s close to the actual page they’re looking for. This is where *navigation cues* can help.
	  
	  Navigation cues surface your information architecture to your readers, helping them understand where they are in relation to the rest of your content, and where to go next. It's the red dot on a map that says “You are here”.
	  
	  Navigation cues include elements like:
	  
	  •   **Breadcrumbs** that show where a particular page sits in a content hierarchy by displaying its parent pages
	    
	  •   **Side navigation** that shows the content hierarchy for the entire site, or a large portion of the site
	    
	  •   **Labels and metadata** that contain information relevant to the document, typically machine readable for help with search indexing
	    
	  •   **Prerequisites, next steps, and additional information sections** that are succinct and informative, directing users where to go next, or what they should have read before arriving at a page
	    
	  •   **Escape hatches**, often in the form of callouts, that offer recommendations for alternative pages if a reader ends up on the wrong page ([View Highlight](https://read.readwise.io/read/01gq6t5d9z219f0f0472ck85n5))
	- Organizing your documentation
	  
	  Organizing your documentation means assessing your existing content, planning and building an information architecture, and migrating content into this new organizational scheme. The goal is to create the best organizational structure for your content that helps your users find what they need *and* that you can maintain and scale over time. ([View Highlight](https://read.readwise.io/read/01gq6v18e97c8an0de981qpzj3))
	- Assess your existing content
	  
	  The first step to organizing your documentation and building an information architecture is to create an assessment of your existing content. The goal is to create a list of all the content you currently have and understand how well its location is serving your users.
	  
	  Think of assessment as a flow chart that starts at the top of your site and goes through each page in your documentation. To start, list each page of documentation in your site in a spreadsheet, including the page title and URL. Next, evaluate each page in the list, using what you know about your users to determine how well each page is working. Ask yourself the following questions:
	  
	  •   Is this page useful?
	    
	  •   Is this page up to date?
	    
	  •   Is this page in the right place?
	    
	  
	  As you evaluate each page, label it with what work needs to be done. Example labels include:
	  
	  •   Keep
	    
	  •   Remove
	    
	  •   Review for accuracy
	    
	  •   Merge with another document
	    
	  •   Split into multiple documents ([View Highlight](https://read.readwise.io/read/01gq6v2a329c3c5nmtxn0tgmy5))
	- After assessing your existing content, ask yourself, is there missing information that your users have been requesting? This missing content is called a *content gap* . Make a list of all the content gaps you find and add them to your assessment.
	  
	  From this exercise, you now have a list of all the content that *should* be in your new information architecture. You also have a list of new content to create, edit, or remove to improve your set of documentation. ([View Highlight](https://read.readwise.io/read/01gq6v2rp39s5f0379c8dvk16r))
	- Outline your new information architecture
	  
	  After assessing your existing content, consider what an ideal map of your content would look like. This is your chance to map out how your content should be organized to best support your users. ([View Highlight](https://read.readwise.io/read/01gq6v349b7hgbss1n4v1k3888))
	- Ultimately, users expect your content to be:
	  
	  •   **Consistent:** Your content is organized with familiar structure and patterns. Users always know where they are.
	    
	  •   **Relevant:** The most important content that addresses the most common user needs is the easiest to find.
	    
	  •   **Findable:** Your content is easily accessed from any homepage or landing pages, and through search ([View Highlight](https://read.readwise.io/read/01gq6vk6q0jcdpby1hhyksgcsp))
	- With these principles in mind, make sure your map includes consistent patterns for your content. For example, if you have a list of procedures documented, you probably want to list them in chronological order. If you have a list of conceptual information, you might want to organize it based on what’s most important to your users first ([View Highlight](https://read.readwise.io/read/01gq6vm3ecs0jabg18rnmsjhfy))
	- Aim for an information architecture that’s neither too deep nor too shallow. If one section of the site is too deep, consider ways of dividing that content into different groups. Likewise, if you have a section with only one page in it, consider whether to merge the page into another.[4](https://readwise.io/reader/document_raw_content/27434535#Fn4)
	  
	  As you settle on an outline for your content, verify your new information architecture serves the needs of your users. Consider the common tasks that your users perform with your documentation, and ask yourself:
	  
	  •   Does each common task have a clear starting point?
	    
	  •   Is the next step for each task clearly defined?
	    
	  •   Are there any missing steps (content gaps) that need to be added? ([View Highlight](https://read.readwise.io/read/01gq6vn5k8gt9b7net09931739))
- New highlights added [[2023-01-20]] at 2:50 AM
	- Migrate to your new information architecture
	  
	  Once you’re happy with your information architecture and you’ve gotten enough user feedback and validation, it’s time to migrate to your new organizational structure. As you move the pages around, use this validation checklist as an auditing mechanism:
	  
	  •   **Landing pages**: created sparingly and guiding users to the most important documents
	    
	  •   **Content types**: consistently implemented and suitable for your users
	    
	  •   **Page data**: descriptive and consistent titles, headers, prerequisites, and next steps
	    
	  •   **Navigation cues**: breadcrumbs, side navigation, and escape hatches to help orient users
	    
	  •   **Labels and metadata**: display relevant data for users and search index
	    
	  •   **Redirects:** users are redirected from previous locations to new URLs after you move pages ([View Highlight](https://read.readwise.io/read/01gq6vpzyxhxx58yqca8r67p9v))
	- Align documentation with release processes
	  
	  Once you’ve budgeted time in your planning process for updating documentation, you should also integrate documentation into your release process. Updated documentation and code should be released at the same time, guaranteeing that they both stay in sync.
	  
	  There are many ways you can align docs with a release. One way is to create tracking issues or bugs for each documentation update required for a release. Another way is to track documentation needs in a spreadsheet along with feature requests.
	  
	  For example, Kubernetes (Kubernetes.io) tracks its feature release process using a spreadsheet. Kubernetes is an open source project for automating container deployment and management with over 43,000 contributors.[1](https://readwise.io/reader/document_raw_content/27434535#Fn1) Despite its large size and rotating group of contributors, Kubernetes aligns new feature releases (called “enhancements”) and documentation updates with the following release process:[2](https://readwise.io/reader/document_raw_content/27434535#Fn2)
	  
	  1.  1.
	    
	    A tracking spreadsheet lists all proposed enhancements for the upcoming release.
	    
	  2.  2.
	    
	    Each proposed enhancement is documented in a Github Issue, and is required to have a design doc, feature owner, unit tests, and an assessment of whether or not documentation is necessary.
	    
	  3.  3.
	    
	    If the enhancement needs documentation, the feature owner must open a Pull Request for documentation and receive approval before the enhancement is approved for release.
	    
	  4.  4.
	    
	    Once the code, unit tests, and documentation are all approved for the enhancement, the enhancement is approved for launch.
	    
	  5.  5.
	    
	    On the release date, all approved enhancements are pushed with the new release.
	    
	  
	  In the case of Kubernetes, the process for releasing code enhancements is tightly coupled with the documentation process. This effort keeps the documentation up to date, preventing the documentation from diverging from the code. ([View Highlight](https://read.readwise.io/read/01gq6vsa63631vtbwbsh5gs35p))
	- Assign document owners
	  
	  Documentation often seems like a task that everyone is responsible for—and therefore *no one* is responsible for. Make responsibility clear with explicit assignments to owners who are responsible for responding to documentation issues, reviewing documentation changes, and updating documentation when needed. Clear, unambiguous responsibility helps prevent documentation from going out of date. ([View Highlight](https://read.readwise.io/read/01gq6vsnzn922g6axjhr45v9rh))
- New highlights added [[2023-01-20]] at 3:45 PM
	- Content freshness checks
	  
	  With a large enough documentation set, some documents eventually become stale and out of date. One way to avoid staleness is to show the “last modified” dates for your content on the rendered page. Last modified dates denote the last time that the document was reviewed or updated. If your documentation is stored in a source code repository, you can pull this information directly from your repo. Otherwise you can embed metadata in the document to store this information.
	  
	  In addition to last modified dates, you can set times in the future to verify the contents of your document. ([View Highlight](https://read.readwise.io/read/01gq84h28xgrnwv0axx9q3644g))
	- Link checkers
	  
	  Links in your documentation can break when the link target is moved, archived, or deleted. As your documentation grows, verifying that all of your links work can be a frustrating, time consuming process. Link checkers relieve toil by verifying all the links in your site, flagging links that generate 404 errors for updates.
	  
	  Link checkers work in one of two ways:
	  
	  •   By running against your documentation prior to publication as part of your CI/CD toolchain
	    
	  •   By running against the documentation after it’s published by crawling your document like a web page
	    
	  
	  How you integrate a link checker into your documentation depends on the tools you’re using for publishing and hosting your documentation. There are multiple tools available for both approaches. ([View Highlight](https://read.readwise.io/read/01gq84hn5cpm9d9g84s4mpktfc))
	- Deleting documentation
	  
	  As a rule, documentation should be deleted when it’s no longer useful to your users. There are a few common reasons this might happen. One is when all the users of a deprecated feature have successfully migrated away from it, the feature is being removed, and the documentation is no longer needed. Another reason to delete is when a piece of documentation is outdated or irrelevant and it’s not worth the time to fix it. ([View Highlight](https://read.readwise.io/read/01gq84jywcpxvs1nqv231avjh3))