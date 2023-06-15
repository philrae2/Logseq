title:: Scrum_and_XP_from_the_Trenches_How_We_Do_Scrum_Henrik_Kniberg_Z-Library (highlights)
author:: [[readwise.io]]
full-title:: "Scrum_and_XP_from_the_Trenches_How_We_Do_Scrum_Henrik_Kniberg_Z-Library"
media:: #articles
url:: https://readwise.io/reader/document_raw_content/53150715

- Highlights first synced by [[Readwise]] [[2023-05-24]]
	- There must be no one outside a team interfering with the team during a
	  sprint. ([View Highlight](https://read.readwise.io/read/01h17dcbcd7s20myx8xhbbmcaj))
	- Both Scrum and extreme programming (XP) ask teams to complete
	  some tangible piece of shippable work by the end of each iteration.
	  These iterations are designed to be short and time-boxed. This focus on
	  delivering working code in a short timeframe means that Scrum and XP
	  teams don’t have time for theories. They don’t pursue drawing the perfect
	  UML model in a case tool, writing the perfect requirements document,
	  or writing code that will be able to accommodate all imaginable future
	  changes. Instead, Scrum and XP teams focus on getting things done.
	  These teams accept that they may mistakes along the way, but they also
	  realize that the best way to find those mistakes is to stop thinking about
	  the software at the theoretical level of analysis and design and to dive in,
	  get their hands dirty, and start building the product. ([View Highlight](https://read.readwise.io/read/01h17ddg369f2z5342evcms84m))
	- Er, no, the product backlog isn’t the starting point. A good product starts
	  with a customer need and a vision for how to solve it. The product backlog
	  is the result of refining that vision into concrete deliverables. The journey
	  from vision to backlog can be quite complex, and lots of techniques have
	  popped up to fill that gap. Things like user-story mapping (read Jeff
	  Patton’s book, it’s great!), lean UX, impact mapping, and more. But don’t
	  use that as an excuse for big, up-front design though! Let the product
	  backlog emerge iteratively, like everything else. ([View Highlight](https://read.readwise.io/read/01h17efdc6jej689zrmbjt4kv3))
	- PRODUCT BACKLOG (example)
	  ID Name
	  Imp Est How to demo
	  1
	  Deposit
	  30
	  5
	  Log in, open deposit
	  page, deposit €10, go
	  to my balance page
	  and check that it has
	  increased by €10.
	  2
	  See your
	  own
	  transaction
	  history
	  10
	  8
	  Log in, click on
	  “transactions”. Do a
	  deposit. Go back to
	  transactions, check
	  that the new deposit
	  shows up.
	  Notes
	  Need a UML
	  sequence
	  diagram.
	  No need to
	  worry about
	  encryption for
	  now.
	  Use paging to
	  avoid large DB
	  queries. Design
	  similar to view
	  users page. ([View Highlight](https://read.readwise.io/read/01h17evky6ee9dwxenp0p2b79z))
		- **Note**: Screenshot
	- I would never consider using
	  Excel for backlog management today, unless it’s a cloudy version. The
	  product backlog needs to live in a shared online document that anyone
	  can access and edit easily and concurrently. Either one of the gazillion
	  backlog management tools available (Trello and LeanKit and Jira are
	  popular) or a Google Spreadsheet (very practical!). ([View Highlight](https://read.readwise.io/read/01h17f4mw5ykrvfvc2des77sak))
	- Additional story fields
	  Sometimes we use additional fields in the product backlog, mostly as a
	  convenience for the product owner to help him sort out his priorities: ([View Highlight](https://read.readwise.io/read/01h17f5h16w4bthpm60nfaz38r))
	- Components - Usually realized as “checkboxes” in the Excel
	  document, for example “database, server, client”. Here the team or
	  product owner can identify which technical components ([View Highlight](https://read.readwise.io/read/01h17f5tryrp5qmxyr4j08sf95))
	- The team is normally
	  better suited to figure out how to solve something, so the product owner
	  should focus on business goals.
	  When I see technically oriented stories like this, I normally ask the product
	  owner a series of “but why?” questions until we find the underlying goal.
	  Then we rephrase the story in terms of the underlying goal (“speed up the
	  search event form in the back office”). The original technical description
	  ends up as a note (“Indexing the event table might solve this”).
	  There’s an old and well-established template for this: “As X, I want Y, so
	  that Z.” For example “As buyer, I want to save my shopping cart, so that
	  I can continue shopping tomorrow.” I’m really surprised I hadn’t heard
	  of that in 2007! Would have been very convenient. Yes, there are more
	  elaborate templates available nowadays, but this simple one is a good
	  starting point, especially for teams that are new to the whole agile thing.
	  The template forces you to ask the right types of questions, and reduces
	  the risk of getting stuck in techy details. ([View Highlight](https://read.readwise.io/read/01h17fkwyyxcemng1h8zqqmgyh))
	- OK, sprint planning day is coming at us quickly. One lesson we learn
	  over and over is: Make sure the product backlog is in shipshape before the
	  sprint planning meeting.
	  Amen to that! I’ve seen lots of sprint planning meetings blow up because
	  the product backlog is a mess. You know the saying “shit in = shit out”?
	  Exactly.
	  And what does that mean? That all stories have to be perfectly well
	  defined? That all estimates have to be correct? That all priorities must be
	  fixed? No, no, and no! All it means is:
	  •   The product backlog should exist! (Imagine that?)
	  •   There should be one product backlog and one product owner (per
	  product that is).
	  •   All important items should have importance ratings assigned to
	  them, different importance ratings.
	  •   Actually, it is OK if lower-importance items all have the same
	  value, since they probably won’t be brought up during the sprint
	  planning meeting anyway.
	  •   Any story that the product owner believes has a remote
	  possibility of being included in the next sprint should have a
	  unique importance level.
	  •   The importance rating is only used to sort the items by
	  importance. So if Item A has importance 20 and Item B has
	  importance 100, that simply means B is more important than A.
	  It does not mean that B is five times more important than A. If B
	  had importance rating 21 it will still mean the exact same thing!
	  •  
	  It is useful to leave gaps in the number sequence in case an item
	  C comes up that is more important than A but less important
	  than B. Of course you could use an importance rating of 20.5 for
	  C, but that gets ugly, so we leave gaps instead!
	  Bah, just sort the list and you don’t need to fiddle with importance ratings.
	  •   The product owner should understand each story (normally he is
	  the author, but in some cases other people add requests, which the
	  product owner can prioritize). ([View Highlight](https://read.readwise.io/read/01h17fpqnf2d9k74h5jdwpzcmb))
	- Sprint planning is a critical meeting, probably the most important event
	  in Scrum (in my subjective opinion of course). A badly executed sprint
	  planning meeting can mess up a whole sprint.
	  Important? Yes. Most important event in Scrum? No! Retrospectives
	  are waaay more important! Because well-functioning retrospectives will
	  help fix other things that are broken. Sprint planning tends to be pretty
	  trivial as long as the other things are in place (a good product backlog,
	  an engaged product owner and team, etc.). Also, sprinting isn’t the
	  only way to be agile – a lot of teams use kanban instead. I even wrote
	  a mini-book about it: “Kanban and Scrum: Making the Most of Both”.
	  http://www.infoq.com/minibooks/kanban-scrum-minibook ([View Highlight](https://read.readwise.io/read/01h17gaa6dvankwnktjp746xz7))
	- The purpose of the sprint planning meeting is to give the team enough
	  information to be able to work in undisturbed peace for a few weeks, and
	  to give the product owner enough confidence to let them do so.
	  OK, that was fuzzy. The concrete output of the sprint planning meeting
	  is:
	  •   A sprint goal
	  •   A list of team members (and their commitment levels, if not 100%)
	  •   A sprint backlog (= a list of stories included in the sprint)
	  •   A defined sprint demo date
	  •   A defined time and place for the daily scrum ([View Highlight](https://read.readwise.io/read/01h17gb19ejm0nfj05nxaq8d3b))