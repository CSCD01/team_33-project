# **Team 33 Deliverable 1**

## **Chosen Process**: Kanban Agile Process

## **Reasoning**:
1) Agile makes the most sense:

   The schedules of the team members is very volatile during the second half of the semester, so we need to be able to change requirements and expectations on the fly.

   Creating a plan for the next few days, up to a week, would not work well for us as it requires a level of dedication and time allocation that cannot be promised from university students in their last semester. So more flexibility is required.

   Reuse-oriented development processes also did not make much sense because the project is more or less done at this point, and is not created from existing components, and is not modularized itself. Using any process that is reuse-oriented would not work well at all really.

2) Kanban allows us to tailor the process to how we best operate:
   
   The practices of Kanban coincide well with how we usually work together as a group. The idea of visualizing the work is very helpful as most of are visually oriented, so being able to see what work is at what stage is a great boon to our productivity.
   
   Another practice is to limit the amount of work in progress, which is best for us, since everyone has a lot of work to do aside from this project, so limiting the amount of context switching we do, is best for the whole team.

   There is also a principle in Kanban to encourage leadership among everyone, which again works well for us, as we do not have defined roles for anyone in the group and it really is a collaborative effort with ideas welcome from everyone.

3) The down sides of agile do not really apply to us:
   
   * Difficult to keep the interest of customers: We have no customers
   * Team members may be unsuited to the intense involvement: This is where the kanban nature of our process comes into play, as people choose what they are most suited too, so we minimize how out-of-place people feel
   * Prioritising tasks is hard with multiple stakeholders: We don't really have any stakeholders other than the 4 members
   * Simplicity is hard to maintain: We are using kanban for this purpose, as with kanban it is very clean to begin with and you do not clutter things up.

## Tools Used:

1) Trello Board: This will help us visualize the workflow of the project, and we have added extensions that help us limit the work in progress to really uphold the principles of Kanban

2) Github: Where we keep all our code and things that we want to merge

3) Discord: We want to have daily meetings, and it is difficult with our schedules to be doing them in person, so sometimes we will use Discord


## The PDF.js code base
PDF.js is initially quite daunting of a codebase, with high level JavaScript spread across 75+ files, and quite little in-line documentation to help one trying to make sense of any of it. Many of these files are contain code for abstracting much more specific tasks like `jpg.js` which processes .jpg images more efficiently than other image file types. The code relevant to a developer trying to use PDF.js is in `pdf.js` which exports the actual funtionality of the API so a developer  can simply include this file in an HTML `<script>` tag and move forward with rendering PDFs. Other important files include `api.js` that facilitates high level interaction with PDFs to render them to the canvas. `document.pdf` interacts with lower level binary data and abstracts it in such a way for `api.js` to use. Rendering of the PDF file to HTML itself takes place inside `canvas.pdf`. The amount of abstraction and division of responsibilities amongst each file in the codebase is quite impressive, albeit a bit confusing to a developer learning the software.


