# Sample Product Feature

####Overview
This repo demonstrates how I would approach adding a new feature as a product manager: selecting a feature to add to an existing product and articulating why it needs to be enhanced, determining a solution and creating tasks for developers to make the idea a reality.

The product I'll use for this demo is Github, which we're conveniently looking at right now.

###The problem
While GitHub has made a lot of significant improvements in project management features over the last few months (with more promised soon), it falls really short is a clean way to collect and tally engineering estimates on issues.  Even if you are using Github as a version control and tracking tool, this sort of information would be convenient for engineers to be able to enter and compare to the actual time between the creation of a pull request (PR) referencing an issue to when the PR is finally merged, and likely more accurate than relying on additional entries in project management software like JIRA or Trello.  However, there is no dedicated place to put that information, so estimates often get buried in the comments or clog up the titles or labels fields, and none are places where that information can be analyzed or summarized.

Overall, this feature update is targeted to users in small to midsize companies who are Github users and don't have the resources to maintain this information (which can change frequently) in two places.  Here are a couple of sample user stories, based on my experience. 

#####User story: Dwayne, Project Manager
Dwayne is a Project Manager in a 100 person tech company.  They use JIRA, but Dwayne and the Product Manager are really the one maintaining it, and most discussion and happens on Github, which means issue descriptions are most current there.  He wants to be able to see summaries of engineering estimates so that he can plan sprints effectively by not over or underloading the dev team, and ensure that all developers have reviewed the issues and feel comfortable enough with scope and requirements to weigh in on timing.  

#####User story: Aarti, Senior Software Engineer
Aarti works in a small tech startup and often needs to step in to write issues, and keep the other three developers on track so that she can report back to the management team on their progress.  They can't really afford an enterprise solution like JIRA, and everyone loves Trello, but it's used more for roadmaps and longer term planning than for projects in flight, since most issue creation, version control and revisions are done by developers in Github.  



###Business case and measurement
This feature is likely not a huge revenue driver in the near term, but it fulfills an important strategic objective: making Github a stickier platform with higher switching costs.

###Alternatives
There are a couple of alternative services that do offer a way to enter an estimate:
_Waffle.io_
Users connect Waffle to their Github account and can see their issues displayed on a board.  The main advantage to Waffle is that it enables you to aggregate issues across projects, but it also includes a field where you can add a "size" to each issue, although there is no attribution to an indvidual for this or range of estimates.

_ZenHub_
Zenhub is a similar product that, like Waffle, incorporates better planning tools, as well as enabling users to add estimates, in a similar way.

###Proposed solution
Based on these use cases, the functionality will include:
- Dedicated field for developers (all people with access to the repo) to enter an estimate for the issue 
- Attribution of each estimate to a developer
- High, low and average estimate data for each issue and the project
- Ability of the github admin to set estimate values (story points, t-shirt sizes, etc) for the project as well as a repo default
- Basic reporting (for a small fee)


