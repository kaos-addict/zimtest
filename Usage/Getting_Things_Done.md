# Getting Things Done
The **GTD** methodology basically calls for maintaining lists of all loose ends that need be taken care of. The idea is that when all things that need to be done are recorded on a list it will give you peace because you do not have to keep them in your mind all the time. However it is essential that you can access the lists and sort through them so you always know what the next thing is that you can do given the time and tools available at a certain moment.

For those not familiar with the book either read it or check any of the numerous websites discussing it. The book follows a flowchart of the life of a task, which looks more or less like this:


![](./GTD_flowchart.png)


As the book only describes the methodology it leaves room to the user how to implement it and what tools to use. You can do it using some software task manager but also just using paper and pencil. There are many software tools designed specifically for the GTD workflow, but zim is not one of them. However the advantage of using a more generic editor like zim is that it is easier to adapt to how you want to do things. The downside can be that you need a bit more discipline compared to using a tool that enforces the GTD way of working. Anyway, this is how I use it, your mileage may vary.


### How I implement GTD in Zim

#### Notebook Layout
First create a new notebook to be used specific as a task tracker. Create pages for the various categories. I use "Projects", "SomeDay" and "Trash" for current, incubating and dormant projects respectively. There are two special pages, one called "INBOX" which is a generic dump for incoming stuff and one called "Chores" (which is a sub-page of "Projects"), which is a generic list of tasks that do not belong to any particular project.


	  INBOX
	+ Projects
	  |-- Chores
	  |-- Current project 1
	  `-- Current project 2
	+ SomeDay
	  |-- Idea 1
	  `-- Idea 2
	+ Trash
	  |-- Old project 1
	  `-- Old project 2
	

I also have several pages living in the top level of the notebook with various tickler lists. These do not contain tasks, examples are a list with loaned books or a  list birthday present ideas. If you have many of these lists consider putting them in a separate "Lists"section. Important is that the lists do not contain tasks.

In addition I find it useful to keep a section with notes as well. These are bits of information I encounter and may be useful in multiple projects. You can also choose to use an entirely different notebook for this and keep it separate from your task tracker.

#### Defining Tasks
As I already mentioned, small single tasks go into the "Projects:Chores" list. But tasks that are more complex or have multiple sub-tasks become projects and these get their own page as sub-page in the "Projects" section. These project pages can in turn have child pages for example with related information, minutes of meeting etc..  

One of the advantages of free-form editing is that you do not need to know what is going to happen with a task right from the start. Some projects start out as a project with a well defined goal, others first live on the "Chores" page as a bunch of related tasks until they take up too much room and get moved out to their own page.

To define individual tasks I use [checkboxes](../Help/Check_Boxes.markdown). This forces the main description to be a single line, which is good to make sure each task clearly states a physical action. Of course just below the checkbox their can be a whole paragraph or even many sub-pages with all the details. If the description sounds more like a topic than like an action probably it should be divided in smaller items that actually are actions. You should only define tasks within the "Projects" section, but you can put them anywhere on the pages. For example if you use a child page of a project page to take minutes of meeting and you get some action item, just put a checkbox for the task right there -- there is no need to first navigate to a main task list.

Now to get an overview of all the tasks the [Task List plugin](../Plugins/Task_List.markdown) and check the "include all open checkboxes" option. This will show a flat list of the tasks defined throughout the notebook and sorts by priority. In addition tasks can have tags to filter then. Tags look like "@work" or "@home" and appear on the same line as the checkbox in the task description. You can use the tag "@waiting" for tasks that you need to check on but are now waiting on someone else to take action.

Also task line items can have a due date, which will show up in the task list. But I do not use this - timing changes all the time anyway. Priority can still be assigned using "!", but don't over-use it, prios are shifting all the time anyway as well. Only use it for things that need to be done ASAP to feel comfortable again.

Finally I like to add a time estimate to a task description. This both forces you to think whether the task is really a physical task with a set effort or not. Also it can work motivating to see a task will only take you about half an hour and then you go home.

#### SomeDay and Trash
Projects that are still under incubation, are defined as sub-pages in the "SomeDay" section. These are project for which I'm collecting ideas, but require no action yet. These do not contain any tasks - remember that only the "Projects" section should contain tasks. As soon as they require tasks they should be moved to the "Projects" section.

Projects that are finished, abandoned or on hold should go under the "Trash" section (or "Archive" if you like). These should not contain any open tasks anymore. If there are still remaining open tasks in a project when I move it to "Trash" I check them off with the [x] checkbox to show they will not be done.

Of course you are perfectly free to move projects back from "Trash" to "Projects" when an abandoned project suddenly gets new interest.

The main point in separating active projects in "Projects" from non-active projects in the other two sections is that at any time you know exactly what are the things you are working on by looking at the "Projects" folder. This also helps with the regular reviews recommended in GTD.

#### Extensions
As an extension I also use the [Journal plugin](../Plugins/Journal.markdown) to have a journal page for each day with notes from meetings etc. Action items from meetings may live there, but this usage is a bit at odds with the use of the INBOX page. At least I can reference discussion notes of a certain date from a project page etc.

#### Summary

* Each action belongs to an open project - "Chores" is the collection bucket for small tasks
* Open projects go in the "Projects" section
* Open projects should have a clearly defined goal which can be evaluated and stamped "finished" at a certain point in time
* Otherwise they go in either "SomeDay" or "Archive"
* Each action should have a checkbox - possible follow up actions can have normal bullets if they are not actionable yet
* Tags on action are used to generate lists
* Some tickler lists can have their own pages, like "Loans"



