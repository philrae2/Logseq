title:: My Zettelkasten workflow from start to finish (highlights)
author:: [[jay l. colbert]]
full-title:: "My Zettelkasten workflow from start to finish"
media:: #articles
status:: #📥inbox 
tags:: #zettelkasten #pkm 
url:: https://wilde\-at\-heart.garden/pages/my\-zettelkasten\-workflow\-from\-start\-to\-finish/

- Highlights first synced by [[Readwise]] [[2023\-06\-16]]
	- A person takes whatever “fleeting” notes made through the day (more on those in a second) and writes “permanent” notes from them. A person will also create reference notes for sources (like books, articles, movies, and conversations), and they will make notes inspired by/in response to those sources. It’s important to connect notes together. ([View Highlight](https://read.readwise.io/read/01h3187xymnbv82vvxq72ejjzw))
	- Fleeting Notes
		- Fleeting notes make up most of the notes we take during the day. These are our tasks, random lists, thoughts, and ideas. They are not necessarily meant to be permanent; instead, you review them and see what you can bring into your Zettelkasten. ([View Highlight](https://read.readwise.io/read/01h318917zwf8tnfpkctqd744d))
	- Permanent Notes
		- Permanent notes are the notes that make it into the Zettelkasten. At least in the way Ahrens uses the term, a permanent note is not synonymous with a “main” note. All “main” notes (or Zettels as some of us call them) are permanent notes, but so are literature notes.
		  
		  **Permanent means it stays in your Zettelkasten.** ([View Highlight](https://read.readwise.io/read/01h3189e0k79eq83z3fn586qgh))
	- Reference Notes
	  
	  I think Ahrens calls these literature notes. I follow Luhmann’s method and reason for making these notes, so at their simplest, they are bibliographic entries in my Zotero database and nothing more. If I’m going to take notes on them, I will make highlights, but instead of necessarily rewriting anything in my own words or summarizing what I’m reading, I make a simple index. I note the page something is on, I give a brief hint as to what it’s about, and then I tag it with a topic I’m focused on. ([View Highlight](https://read.readwise.io/read/01h318a4maxgafrpeh2s4aw773))
	- Zettels
	  
	  Zettels are the main part of the Zettelkasten. For me, these are not about rewriting something I’ve learned in my own words. Rather, they are for responding to, building on, or otherwise interacting with a source or idea. ([View Highlight](https://read.readwise.io/read/01h318ackf9mqw6egd96ancbds))
	- My digital Zettelkasten
	  
	  ![](https://wilde\-at\-heart.garden/assets/screen_shot_2022\-07\-16_at_4.05.27_pm_1658001986452_0.png) ([View Highlight](https://read.readwise.io/read/01h318aybgrh5ffqbsk0z54x1z))
	- How does this fit into PARA?
		- Remember how I did that whole Building a Second Brain thing?[2](https://wilde\-at\-heart.garden/pages/my\-zettelkasten\-workflow\-from\-start\-to\-finish/#fn:2) The organization framework taught in that is called PARA: Projects, Areas, Resources, and Archives.[3](https://wilde\-at\-heart.garden/pages/my\-zettelkasten\-workflow\-from\-start\-to\-finish/#fn:3) Because some folks view the Zettelkasten as another “second brain” system, they try to “PARA” their Zettelkasten.
		  
		  However, while a Zettelkasten can be part of a “second brain,” it in and of itself is not the same thing, at least not in the way Tiago Forte teaches the second brain. **I include my Zettelkasten in the Areas section of my second brain organization because it’s something I need to maintain.** ([View Highlight](https://read.readwise.io/read/01h318d9jrhj9ze1dvm8nskr5e))
	- Step 1: Fleeting Notes
	  
	  The first step in my Zettelkasten workflow is taking fleeting notes. As defined above, they’re basically any notes I take during the day. Like I said, reminders and tasks are technically fleeting notes.
	  
	  In Logseq, I have a template for the fleeting notes I know will feed into my Zettelkasten. Usually, these are ideas for Zettels.
	  
	    \- TODO **Note goes here**
	      date::
	      tags:: 
	      type::
		- [[fleeting]]"
		- I work from my daily journal page. I create a block and use the above template. In practice, it looks like this: ([View Highlight](https://read.readwise.io/read/01h318emc512ky6p4aetkbhwnm))
- New highlights added [[2023\-06\-22]] at 12:20 AM
	- Then, for resources I know I’m going to make notes from or cite, I create a page for it using Logseq’s Zotero integration. ([View Highlight](https://read.readwise.io/read/01h3gj9ajhv2vb8qcwmd6dhf37))
	- {:title "💡 FLEETING" :query (and (property type fleeting) (not (property template)) (not (task done))) :collapsed? true :breadcrumb\-show? false :result\-transform (fn [result] (sort\-by (fn [h] (get\-in h [:block/properties :date])) > result))} ([View Highlight](https://read.readwise.io/read/01h3ghvkb6tzm3fyed4vm3dwkt))
	- Instead of taking lengthy notes and summaries, I create an index when I read. That index is guided by what I’m actively interested in at the moment. I’m not creating a general index of the resource. When I take a highlight, I can actually change the text in the block that’s created. I mention briefly what the highlight is about, and I tag it with a topic. The text is usually themed around that topic. If I were reading with a different topic in mind, what I write for that highlight might be different. ([View Highlight](https://read.readwise.io/read/01h3gjksc954rhmgqsshm4szhc))
	- I embed the highlights page under a Notes block in my reference note. ([View Highlight](https://read.readwise.io/read/01h3gjkyk7y5rdyxam13c1nqkh))
	- I create all reference notes from the daily journal page. I technically have a template for it, but really, all I do is give it a block property of `type:: [[reference]]` and the date, like I did for fleeting notes. Sometimes, I’ll assign tags.
	  
	    \- insert reference here
	      date::
	      tags::
	      type:: [[reference]] ([View Highlight](https://read.readwise.io/read/01h3gjn4epajjfvzc12rqv8pef))
	- As with everything else, I create the permanent note from the daily journal page using the following template:
	  
	    \- LATER [[]]
	      date::
	      tags:: 
	      areas:: [[🍀 Digital Garden]], [[🗃 Zettelkasten]] 
	      type:: [[permanent]]
	      status:: draft ([View Highlight](https://read.readwise.io/read/01h3gjd85w2va8yhjeh1re1h4j))
	- Let’s break this down.
	  
	  I give it the task marker `LATER` so I can query it in my Newsletter workflow; the query for that will make the block disappear when I mark it `DONE`. My workflow and queries are inspired by Ramses Oudt: ([View Highlight](https://read.readwise.io/read/01h3gjf769y3m5vj17xwt5t69j))
- New highlights added [[2023\-06\-22]] at 1:20 AM
	- If it’s something like a journal article, a book, or any type of resource I want to dig deeper into, I take notes on this page. If there’s a PDF, I take notes by using Logseq’s PDF reader. When I highlight passages in the PDF, an annotations page is created with the text of each highlight; each block in that page is actually a block reference to the highlight in the PDF. ([View Highlight](https://read.readwise.io/read/01h3gnm603xkm9ecczf645z45y))
	- Then I create the page. I use an alphanumeric system at the beginning of my note titles because I’m following a Folgezettel structure.[5](https://wilde\-at\-heart.garden/pages/my\-zettelkasten\-workflow\-from\-start\-to\-finish/#fn:5) A Folgezettel is a “follow\-up note.” A Zettelkasten is [[rhizomatic]] and non\-hierarchical, but you can indicate trains of thought or a cluster about a topic by using Folgezettel. I’ll use some recent notes to demonstrate. ([View Highlight](https://read.readwise.io/read/01h3gnvdre4254xhx219e7kxhf))
		- **Note**: Context: When creating a zettel. A zettel is not synonymous with a permanent note.