# Sample Product Feature

### Overview

This repo demonstrates how I would approach adding a new feature as a product manager: selecting a feature to add to an existing product and articulating why it needs to be enhanced, determining a solution and creating tasks for developers to make the idea a reality.

Detailed issues and wireframes outlining specifics of this feature enhancement can be found in [this project](https://github.com/eleanorstrib/sample_feature/projects/2).

The product I'll use for this demo is Github, which we're conveniently looking at right now.

### The problem

While GitHub has made a lot of significant improvements in project management features over the last few months (with more promised soon), it falls really short is a clean way to collect and tally engineering estimates on issues.  Even if you are using Github as a version control and tracking tool, this sort of information would be convenient for engineers to be able to enter and compare to the actual time between the creation of a pull request (PR) referencing an issue to when the PR is finally merged, and likely more accurate than relying on additional entries in project management software like JIRA or Trello.  However, there is no dedicated place to put that information, so estimates often get buried in the comments or clog up the titles or labels fields, and none are places where that information can be analyzed or summarized.

Overall, this feature update is targeted to users in small to midsize companies who are Github users and don't have the resources to maintain this information (which can change frequently) in two places.  Here are a couple of sample user stories, based on my experience. 

##### User story: Dwayne, Project Manager

Dwayne is a Project Manager in a 100 person tech company.  He wants to be able to easily summarize engineering estimates to plan sprints and reallocate work across the team. The company does planning meetings where they estimate time on issues, but discussion often happens on Github, and he needs to keep issues and estimates updated in JIRA, which is used for project planning.

##### User story: Aarti, Senior Software Engineer

Aarti works in a small tech startup and often needs to get updated engineering estimates in order to report back to management, but when engineers write (and sometimes update) their estimates in the comments, it's very time consuming for her to review comments and figure out what estimates everyone made, then tally them up for the project or remaining "TO DOs".    

### Business case and measurement

This feature is likely not a huge revenue driver in the near term, but it fulfills an important strategic objective: making Github a stickier platform with higher switching costs.  

Measurement would include:
- Feature use: Number of issues where at least one estimate is made, reviewing changes over a 3 month timeframe, looking at week over week growth
- Time in platform: Track time spent in-platform among users of the new feature over a 3 month timeframe, looking at week over week changes
- User feedback: Analyze sentiment of feedback on social media and support channels for this particular feature over a 3 month period, determine if trend is postive or flat
- Authorization revocation for alternative services(secondary metric): Number of accounts where alternative service auth is revoked over a 3 month period, compared to previous 3 months

More detailed reporting post-MVP a big value prop of other services (see "Alternatives" below), could be added for a nominal fee, while eliminating the need to use multiple services and simplifying the workflow for users.  The reporting might also drive more non-developer users onto Github and require organizations to purchase more expensive plans.

### Alternatives

There are a couple of alternative services that do offer a way to enter an estimate:

##### _Waffle.io_

Users connect Waffle to their Github account and can see their issues displayed on a board.  The main advantage to Waffle is that it enables you to aggregate issues across projects, but it also includes a field where you can add a "size" to each issue, although there is no attribution to an indvidual for this or range of estimates.

##### _ZenHub_

Zenhub is a similar product that, like Waffle, incorporates better planning tools, as well as enabling users to add estimates, in a similar way.

### Proposed solution

Based on these use cases, the MVP functionality will include:
- Dedicated field for developers (all people with access to the repo) to enter an estimate for the issue 
- Attribution of each estimate to a developer
- High, low and average estimate data for each issue and the project
- Basic roll-up of average estimates in the project view (could be released after the above)

### Future enhancements

- Functionality to enable a product or engineering manager to see all estimates but not expose team estimates to individual developers to get less biased estimates
- Reporting tools to compare estimates to actual dev times (based on PR opening, self-reported time to complete before PR created)
- Speed/accuracy analysis by participant
- Reporting on estimates across multiple projects and time to complete for each participant
- Addition of this information to the Github API

Detailed issues corresponding to this functionality can be found in [this project](https://github.com/eleanorstrib/sample_feature/projects/2).


