---
title: 🧰 Chapter 10 | Schedule Management = Focus Management
---

- > Project managers help their team and themselves focus through schedule management tools, such as the following:
- Milestone chart
- Project calendar
- Gantt chart

Be mindful of choosing work cycles, keeping in mind project goals and the working styles of your teammates.
#.chapterdistillation

- The larger the project, the bigger is the threat of overwhelm. We solve this partially by breaking down the project (eg, with the WBS and the RBS) and programming our attention relative to the importance of their atomic components.
	 - As we execute the project over time, we also need to [program our attention](((5956e203-7944-46f2-ae4c-6616d68693db))) and our team's attention to what is important in each unit of time. This is project schedule management.
		 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FRoamfu%2FFA1mjRfafd.png?alt=media&token=d7c0f345-5584-4ff2-b15c-b26fe0bb71e8)

- In this chapter, we discuss these three commonly used tools for project schedule management:
	 - Milestone chart
id:: c2aa86ca-586c-4eee-8cc5-85798b013810

	 - Project calendar
id:: 5fbc9c4b-11ac-42f4-8e48-23afc59f57e6

	 - Gantt chart
id:: b4add9c1-5aef-42b5-883b-6370eb9db7f2

- Later in this chapter, we also explore the following:
	 - Meeting cadence and project work cycle
id:: 308ff91f-a123-40e6-96b9-ab8cdd18f089

	 - Choosing teamwork software for your project
id:: a61e24d4-9934-4abf-87f2-3f7a94393f6b

	 - Do you need a project schedule?
id:: 9f953813-f282-4d3a-b20e-4d1c1f3b740b

- ((c2aa86ca-586c-4eee-8cc5-85798b013810))
	 - A milestone chart is an executive summary of your project schedule. To create one, the project manager selects milestones—events or outputs that indicate project progress—and estimates a date for each.
		 - As a communications tool, the milestone chart is intended for project charters and presentations to stakeholders. You would want just enough milestones to give your stakeholders an idea of how the project will unfold over time. Too much will dilute your message.
id:: 97c081ca-8aca-4d1e-ace0-4c7c85436a8d
			 - Here's an example from [the first version](https://docs.google.com/document/d/1QY4h7TxQe60gLkTIfv3pM9A63iEgamMFlz59spPc3O4/edit#) of the [[Project Accessible Genomics]] grant proposal:
				 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FRoamfu%2FZcMzeevs2o.png?alt=media&token=c8cba2b6-2a68-4eb2-b474-c1f2a70a591d)

		 - As a planning tool, the milestone chart could be more detailed. Here is the milestone chart from the [project charter]([[[[P: Professional PM for Believers]] Project Charter]]) of the Zoom calls I organized for the Believers of this rBook. I made this purely for planning. I did not present this charter to anyone. It ended up being detailed enough, that I did not see the need to create a different project schedule.
			 - ((56152d41-5540-4ad7-a916-dff34f002fb9))
				 - The advantage of using Roam for planning with dates is that the block appears as a linked reference when the linked date arrives. This works best if you already have the habit of checking the day's linked references as messages from your past self.
id:: 8d18b0f8-34f8-4dd0-a8c6-745956ec8b08
					 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FRoamfu%2FAe8KRN9Rm8.png?alt=media&token=52499d94-12e1-4e2c-a3e6-867f4b179257)

- ((5fbc9c4b-11ac-42f4-8e48-23afc59f57e6))
	 - A calendar is a universal language for schedules. It can be used both for planning and communications.
		 - __Back in P&G, I worked with a project manager who always printed out the latest version of his project calendar. He would walk around the floors where his project teammates were located, bringing the printouts. Everyday, he did quick 1:1 meetings with his teammates in their workstations. They would talk about the week's priorities, obstacles and open issues while looking at the tasks in the calendar. This was his style of managing the focus of his project team.__

		 - Calendar views is a common feature in project management and [task collaboration software](((edda52b0-05fc-4cbd-9d74-518e9e209b54))).

	 - In Roam, there are multiple ways of using date links to create an equivalent to a calendar: a view that shows the focus for a timeframe.
		 - One way is to create a page with intervals of dates and indent work packages from your WBS as block references. You can have them in separate panes and option/alt-drag the work packages from the WBS to your calendar. Here's an example:
			 - {{embed  ((00a7b1d1-bae8-4ca3-ab72-9517592594e3))}}
				 - Similar to [our example above](((8d18b0f8-34f8-4dd0-a8c6-745956ec8b08))), the work packages would appear in the linked references of the dates under which they are indented. I do my weekly planning on Mondays, so all the dates I use are on Mondays.

		 - Another way is to tag the work packages in the WBS with their target dates, and use queries to create reports on which work packages should be the focus for the time period.
			 - For this example, I made [a copy](((db442bcd-6ab2-48bf-b0d4-d7afc52c0311))) of [the WBS of the crowdfunding project]([[[[P: RESOLVED Crowdfunding]] WBS]]) and made the same pairing of dates and work packages as above, but with the dates as linked references/tags beside the work packages. 
				 - The following queries would show us the same work packages per work week:
					 - {{[[query]]: {and: [[➕ Appendix 2 | Exercises]] {between: [[April 26th, 2021]] [[May 2nd, 2021]]}}}}
id:: e668d760-7980-4896-8e4a-e2c1de6eceb7

					 - {{[[query]]: {and: [[➕ Appendix 2 | Exercises]] {between: [[May 3rd, 2021]] [[May 9th, 2021]]}}}}
id:: 04b58d0c-8e79-449e-bf89-fa521239d01b

	 - [[Maximize your learning]]
		 - Tag some (or all) of the work packages in your WBS with dates ([[Tip for Roam beginners]]: use the date picker by typing "/date")
			 - {{embed  ((de4955b2-951b-476c-8b82-f69034814483))}}

		 - Replace the dates in these queries so that they show the work packages from your project instead of the crowdfunding project.
			 - {{embed  ((e668d760-7980-4896-8e4a-e2c1de6eceb7))}}

			 - {{embed  ((04b58d0c-8e79-449e-bf89-fa521239d01b))}}

- ((b4add9c1-5aef-42b5-883b-6370eb9db7f2))
	 - The Gantt chart is a useful visualization **for projects with a lot of dependencies**. Also, some project managers simply prefer this view more than a monthly or weekly calendar. Here is a Gantt chart from [that conference I organized in a university](((251f2934-7424-4f2d-aea0-8811114c86fc))).
		 - {{pdf  https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FRoamfu%2FjjKeA94Tx7.pdf?alt=media&token=6e774046-a9d3-487f-87f5-d57756d1a35a}}

	 - Most project management and project task collaboration software have a Gantt chart view. You can create a Gantt chart manually in Roam using `{{mermaid}}` but this is purely for presentation.

- ((308ff91f-a123-40e6-96b9-ab8cdd18f089))
	 - A work cycle in a project is the duration between your meetings with the team (individual or collective) to align on status of work packages and to start working on new ones.
id:: fe7598c1-0432-4678-ac68-291794c74169
		 - The meeting cadence could be monthly, every other week, weekly and even daily. It could change as the project progresses.
			 - For instance, in projects that prepare for events, the cadence could start monthly, then becomes weekly as the event nears, and might become daily the week before the event. During the event itself, the project manager might want to get updates every hour.

		 - You'd want work cycles to be long enough to get work packages done, and short enough to help avoid the negative impact of **Parkinson's Law**[*](https://en.wikipedia.org/wiki/Parkinson%27s_law) (work expands so as to fill the time available for its completion). This is also called the **College Student Syndrome**: tasks are done at the last possible time it could be done. This does not apply to everyone, of course, but you'd want to [[design for the extremes]].
			 - **Daily stand-up meetings**[*](https://en.wikipedia.org/wiki/Stand-up_meeting) is one way to mitigate these tendencies and to increase awareness of each member's progress and challenges across the project team. Stand-up meetings are different from the meeting between work cycles.

		 - These meetings between work cycles could be done [as a team](((b36234bb-a223-4c79-a77a-976161f1e088))), as a [1:1](((b769f0e9-3c42-4db8-ba7b-caf91a025d70))) or as smaller teams. The bigger the team, the better it is to do 1:1s or to have meetings with smaller teams.

	 - > Project managers need to be mindful in designing meetings schedules. The time our team spends in meetings is time away from getting work packages done.
id:: de924234-ee0c-4c63-aa30-73a91f76d275

- ((a61e24d4-9934-4abf-87f2-3f7a94393f6b))
id:: edda52b0-05fc-4cbd-9d74-518e9e209b54
	 - ((c8040632-2530-4f53-923a-ada3d3e79e3e))
		 - Visualize yourself leading a team meeting or doing a 1:1. Visualize your teammates starting their workday. What reports or views would help you and your team focus? You would want to consider these in your choice of software. Here is my top three:
			 - Tasks in a timeframe
id:: c6482f09-43a5-4dbb-894e-ef262f22b8b5

			 - Tasks per person
id:: 5803bd20-d26a-4de7-a853-2ddc847d2d04

			 - Tasks per person per timeframe
id:: 3dd137b3-ec3e-47dd-b00f-3ff412ecccf8

		 - Some projects have a lot of task dependencies (eg, construction). If your project is such, you would also want the following features:
			 - Automated sequencing visualization after the input of dependencies and task durations (usually presented as a Gantt chart).
				 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FRoamfu%2FADEF-fUK8s.png?alt=media&token=96324084-2ae3-4047-a4c2-ab2a960063d7)
					 - [Image source](https://www.wrike.com/blog/critical-path-is-easy-as-123/)

			 - Automated highlighting of the critical path (the red bars in the image above).
				 - __"In project management, the critical path is the longest sequence of tasks that must be completed to successfully conclude a project, from start to finish. The tasks on the critical path are known as critical activities because if they're delayed, the whole project will be delayed."__[*](https://www.projectmanager.com/critical-path-method)

	 - If your team is adept at using Roam, or if you opt to forego task collaboration software, these reports could be made with filters or queries:
		 - - ((c6482f09-43a5-4dbb-894e-ef262f22b8b5))
- ((5803bd20-d26a-4de7-a853-2ddc847d2d04))
- ((3dd137b3-ec3e-47dd-b00f-3ff412ecccf8))

		 - See [[🧰 Chapter 8 | How to Not Fail: The RBS and The Risk Register]] for an example of using queries.

	 - You could opt to forego task collaboration software
		 - Collaboration software requires some time to maintain. It could dissipate the focus of your team. You can run a project without it. In this case, you curate project information for your team: you tailor-make your communication on what tasks you should focus on per work cycle. You make use of whatever communication tool you and your team are used to.

	 - > Whether or not you use task collaboration software, you need to [tell the story](((371c4095-e3e7-41f1-9c6a-2eeae25b6b82))) of every work cycle: what victory means, what challenges await us, why this work is meaningful.

- ((9f953813-f282-4d3a-b20e-4d1c1f3b740b))
	 - To me, a WBS, an RBS and a risk register are required in all projects.[*](((a8f092ef-4ed1-44eb-8c34-8867b1a4bec1))) A project schedule, however, may be a waste of time for certain kinds of projects.
		 - Recall our table of relative flexibility among the triple constraints of a project:
			 - ((56c31dc8-7685-4151-b4c0-39710429aa60))

			 - If schedule is the most flexible aspect of the project, you don't want to add the artificial constraint of deadlines.
				 - After building the WBS of [[Project Accessible Genomics]], we knew what work was needed to get sequencing up and running in a lab. However, we did not know how long it would take to do them, particularly for fundraising and getting the equipment into the country. We focused on what could be done in each work cycle, instead of chasing arbitrary deadlines.

		 - For schedule-centric projects, like events and most projects under contract, the opposite is true: your project schedule should be the center of your focus.

	 - > Plan a project management schedule based not on convention, but on what the project needs, and what works best for your teammates.

- [[Maximize your learning]]
	 - What do you need to accomplish during your team meetings? What kind of meetings would help you accomplish these objectives? (What is the agenda, who needs to be there, what is the frequency.)
		 - 

	 - When deciding on meeting schedules, we should consider not only the needs of the project, but the culture of the team and individual work styles. Can you talk to each of your teammates to get an idea of their working styles, then adjust your meeting plan based on what you learn?
		 - 

	 - Choose a criteria for selecting which software you should use for project management and collaboration. What are the applications that fit the criteria best?
		 - 

	 - Do you need a project schedule for the project you are managing?
		 - 

- ---

- [[Next chapter]]
	 - The core of project management is to get the work packages in the WBS done. However, it your project team (sometimes this is just you) that gets work packages done. The next chapter is all about leading and motivating your project team. [[🧰 Chapter 11 | People Will Make or Break Your Project: Leading a Team]]

- ---

- {{embed  ((24ff1515-f632-42b9-91f3-b214f32d3e9b))}}
