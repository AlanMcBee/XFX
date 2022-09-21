# Documents Index

This is *project* documentation, not documentation for the released product.

To start this off, there are scans (PDFs) of notes I wrote in the artifacts folder. I'll transcribe those with https://github.com/AlanMcBee/XFX/issues/2

## Transcribed thoughts from PDFs

### On the name XFX
XFX is a meant to be a temporary name, a sort of project code name.

XF is how I've been abbreviating "executive functions" whenever I write about ADHD.

XFX is, to my mind, an "executive function extension" or "executive function extender", by which I mean that it is meant to enhance executive function capabilities for those with reduced executive function capabilities (i.e. most people with ADHD).

### Background and reason for building this
There are many names and categories for the types of systems that assist us humans with doing things:
- Planners
- To-do lists
- Task lists
- Activity planners
- Project schedulers
- Reminders
... and even calendars can fall into this realm.

The one weakness I think most systems that I've ever tried to use in the past have is that they all act as though they are the primary or central point around which all planning and doing should take place. That is, while they may offer some kind of integration ability with external systems, the proposed value of these systems is only fully delivered if you engage primarily with that system, and limit interactions to other systems.

This does not work well for me. I have not found a system that adequately handles all of the reasons I depend upon various systems to help me prioritize my work and then do it. Some are better at planning, but fall short when I need to do things quickly and follow up. Others are great at working with individual tasks but make it difficult to get a whole-picture perspective. Others don't take into account the time or energy or mindset I have. Things that needs schedules might get placed on my calendar, but things on my calendar don't find their way back to my to-do planning.

Rather than build the system-to-end-all systems, I decided to abstract out the management of projects and tasks and schedules, and rely on other systems to do whatever it is they do best, while keeping each system synchronized with all of the other connected systems.

To do this, there must be one authoritative source of all of the connections, and one central master coordination service. But that service does not necessarily need the details of the tasks, projects, or events. It only needs the time-related and relative-prioritization information of various items.

Another shortcoming of many systems is that they fail to navigate the real-life situational needs of most people (well, me, more specifically, but I think I'm not alone). Most systems keep "work-life" separated strongly from "home-life" or other contexts. The reasons are legit: most employers regard the information and activities their workers perform as company intellectual property. Any worker who might use a personal device or connection to a network for work typically agrees to forfeit access to that information upon no longer having employment, and companies typically insist on the ability to forcibly remove that information from the devices at that time. Furthermore, some security-related scenarios require similar features (for example, having a device become lost or stolen).

### Fundamental design
Each human user will be expected to create a maximum of one account. This account would normally be associated with exactly one human for the lifetime of that person. I don't think I want to try to enforce these limits. If a person creates multiple accounts, it just means they lose valuable opportunities to manage everything in their lives. And if a person shares an account with someone (by sharing a password, etc.) it just means they lose privacy and have to deal with some confusion and ambiguity.

The account will be used to connect to different systems that the user wishes to synchronize with XFX. However, information that is proprietarily owned by those other systems will remain on those systems. The details of those projects, tasks, events, and so on will be shown to the users only at the endpoint where the user interacts with XFX. Those details will not be duplicated to a service or storage area that is owned by XFX unless the user explicitly agrees to do so and as long as the connected service permits XFX to do so.

### Fundamental features
There are two primary functions that I would like XFX to provide:

1. Prioritization of actions

I use David Allen's definition of actions (or "next actions") from his seminal book *Getting Things Done*. It is a discrete physical action that a person can perform, usually at one time. David does not directly guide readers to any particular approach to prioritizing the next actions. Rather, he advises that actions should be chosen based on situational context, on prior commitments, on available energy, and so on. He expects that any effort to prioritize a list of action is destined to be undone quickly as contexts, unexpected events, or energy changes throughout a day, and I agree.

XFX will assist with rapid and dynamic prioritization. I plan to offer several highly efficient user interface models that simplify the process of determining "what to do next."

2. Scheduling of actions

If all there were to do was merely to complete tasks on a list, adding new tasks to the list as the thoughts occur, and repeating this process to health, weealth, and wisdom, then I could stop with just the one function. Unfortunately (at least for me), people want to know when I will complete a task that I committed to doing. Another problem that tends to beset people with ADHD is so-called "time-blindness." This is sometimess expressed as that people with ADHD have only two time frames from which they work: now, and not now.

Scheduling is hard, because none of us always know what will be the unexpected events that knock us off our plans, or how much energy we think we'll need to start a challenging task at the time it should be done. Coordinating our actions with other people is yet another task that needs doing beyond the task that is to be done, which can be perceived as demanding more energy than the task alone.

XFX will assist with projecting the expected completion of tasks, by taking a comprehensive whole-life approach to applying a heuristic to when actions could or should be done. It includes the awareness that in our new normal (post COVID-19), many more people now work from home, which can be both liberating (no more daily commutes!) but also more demanding because you can't exactly "leave your work at work." XFX will try to help track, report, and appropriately plan tasks to fulfill objectives such as a minimum number of hours spent at work, and also at personal goals like getting enough sleep or personal projects.

### References
There are many other personal activity systems that I like, or at least that I like some aspects of those systems.

#### Microsoft To-Do
To-Do has a "My Day" feature. Add tasks to My Day, and then work just from that list. At the end of the day, everything is cleared out of the My Day list. It's motivational to get the work done so that you don't have to add it again the next day, but it's also a fresh start on the next day as you reconsider your priorities and goals.

To-Do also has a very powerfully intuitive UI for adding and managing basic actions. I find it not so wonderful for managing projects.

Even so, To-Do is fast and friendly. It would be my primary activity tracking tool, but I would not use it for my project planning or tracking with its current features.

#### Microsoft Outlook
Outlook has my favorite email and calendar tools. Emails can be flagged for followup, including sending an email to someone else that is pre-flagged so that you are notified when they mark it as complete. The calendars are fast and well done. Outlook tasks are sophisticated: you can create recurring tasks and provide considerable other details to them. Outlook tasks are used by Microsoft To-Do; a task created in To-Do will automatically appear in Outlook, and vice-versa.

Like To-Do, Outlook does not manage projects well. Outlook would be my primary communication and scheduling tool, where I would occasionally create or report on the status of assigned tasks or flagged emails.

#### Microsoft OneNote
OneNote is not ordinarily thought of as an activity system, but it does have to-do-style checkboxes, and it can also create Outlook tasks that are linked to paragraphs in OneNote. However, the main thing I like for OneNote is that is works great for project support. That is, for any given project that I'm doing, I nearly always want to have a section in OneNote that I use to track records, thoughts, and other notes about the project.

#### Microsoft Excel
Excel isn't an activity planner of any kind. But it is good at working with lists. There are times that I wish I could look at or edit details of projects in bulk. Excel is a great tool for that.

#### Microsoft Planner
Planner is good for team-based project management. Using a Kanban-style layout, it's easy to see a board of in-flight projects organized by priority order, and quickly update details. To-Do can show tasks from projects that are assigned to individuals, which is a nice way to bring all that together.

However, Planner is part of Microsoft 365 and not yet readily available to consumers. Even if it were availalbe, Planner does not easily aggregate all of the different Planners for teams in which a user might be a member. This makes it difficult to prioritize across multiple teams or groups of projects.

I would use Planner to plan the projects withing a team and to break down those projects into tasks. Sometimes I will update the tasks from Planner, but I would usually not have Planner open when I am considering which next actions I plan to do throughout the day.

#### Microsoft OneDrive
OneDrive is not an activity planner. It's a file storage service. This makes it a great place to store project support documents.

#### Azure DevOps
I'm a software engineer, and I can expect to spend considerable time using this product to complete my work at work. It includes Kanbans, backlog ordering, and project-to-task breakdown abilities, as well as some scheduling features.

While I very much appreciate Azure DevOps features, it doesn't update or interact with other systems. So tasks that I create in Azure DevOps will not automatically appear in To-Do or Outlook. Azure DevOps does not work as well for day-to-day projects and tasks.

#### Microsoft Project
Project is the industrial-strength project planning tool. It can handle the largest project you might want to throw into it. It is far too unwieldy to use as a personal task and activity planner. Even so, it can be used to assign tasks to individuals.

#### Microsoft Lists
Lists provides a simple interface for working with basic lists. It might be helpful to use it to show project or task status.

#### Many many others
- Asana
- Trello
- Monday
- Todoist
I am not going to compile an exhaustive list of all the planning and activity tools that are out there. Many are great tools, with great features. I'm not going to outdo any of them. I don't think I need to. None of them are going to traverse the work/life thresholds well. Or they focus too much on planning and not so much on doing.

## Solution Architecture
Even though XFX is not designed to be the end-all-and-be-all of project planning and activity tracking systems, it will need a custom user interface and some rudimentary features to enter and work with projects and tasks, not to mention other settings or configuration values.

### Smart Clients
I have choices to make, specifically for the client portions of the system.
- WPF
- MAUI
- Blazor
- WinForms
I am definitely going to stay away from Javascript-based platforms. And, even though I'm comfortable with HTML and CSS, I don't love those enough to feel that they are an easy choice over alternate client technologies.

The client portion of the system will be responsible for coordinating the interaction between sources that are held by or in systems that might not be under the direct control of the user. The client system might rely on a shared scheduling service, but any sensitive information about the data being processed (projects, activities, tasks, etc.) will be kept out of the shared services. Those services will work only with the necessary essential properties they need, which should not include titles, descriptions, PII, and so on. The client will be responsible for mapping operational data used by those shared systems back to the authoritative sources.

While I am planning a shared service that can support scheduling or other operations, I plan to include some or most of those operations as supplemental features in the client.

