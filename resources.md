# Resources

## GitHub + Rstudio

Posted below are a series of screencast videos to help get you set up with GitHub and RStudio.

1. [Linking GitHub to RStudio](https://www.dropbox.com/s/zxwz6mmlf5bs4du/github-rstudio-A.mov?dl=0)
2. [Submitting work by commit + push](https://www.dropbox.com/s/xgggdzwtoze3bi3/github-rstudio-B.mov?dl=0)
3. [Cleaning up with .gitignore](https://www.dropbox.com/s/4n629c1e9yy90bb/github-rstudio-C.mov?dl=0)
4. [Cacheing credentials](https://www.dropbox.com/s/07gkvhxzl7ju1bv/github-rstudio-D.mov?dl=0)

In case you missed it in video 4, the command that you paste into Tools > Shell is:

`git config --global credential.helper 'cache --timeout=10000000'`

## Homework workflow

### Creating, committing, pushing

Every time you're ready to work on an assignment, open up RStudio and be sure you're open to your named project (like "andrew_bray") indicated by the blue cube in the upper right hand corner. This is where you'll do the bulk of your coursework: it is a directory on your account on the RStudio server and a Git repo associated with repository on our class GitHub page.

To start an assignment, create a new R Markdown file and change its output format to `github_document`. As you save this file, you'll see it pop up in the Git pane in the upper right hand panel. Periodically, you may want to "knit" the file to see how the compiled version looks. 

Whenever you complete a good chunk of work on the assignment, click the boxes next to any changed files then click "commit", provide a commit message, and click "commit". This records how the file has changed. Close out of these windows and resume working on the assignment.

Once you're done with the assignment, commit any final changes to files and click the green "push" arrow in the Git pane. This will send all of your commits to Github.


### Submitting and Feedback

Homework is formally submitted by going to your repository on GitHub and creating a new issue (the issue tab is right under the repo name). The name of the issue should be "Review assignment X". The only text in the issue should be the name of your randomly assigned reviewer. When you click to create this issue, it will send an email to your reviewer letting them know it is ready. The reviewer will then access your repo on Github, read through the assignment file (the .md will be easiest to read), and provide written feedback in the issue.

## General homework rubric

The rubric below can used to review your own work (to be sure you have all the bases covered) and when providing feedback to others (for ideas on what to focus on).

Topic      |     Excellent      |        Satisfactory      |     Needs work      |  
|-----------| ------------------- |----------------------| -----------------|
|Coding style| Student has gone beyond what was expected and required, coding manual is followed, code is well commented | Coding style lacks refinement and has some errors, but code is readable and has some comments | Many errors in coding style, little attention paid to making the code human readable|
|Coding strategy| Complicated problem broken down into sub-problems that are individually much simpler. Code is efficient, correct, and minimal. Code uses appropriate data structure (list, data frame, vector/matrix/array). Code checks for common errors  | Code is correct, but could be edited down to leaner code. Some "hacking" instead of using suitable data structure. Some checks for errors. |   Code tackles complicated problem in one big chunk. Code is repetitive and could easily be functionalized. No anticipation of errors. |
|Presentation: graphs | Graph(s) carefully tuned for desired purpose. One graph illustrates one point | Graph(s) well chosen, but with a few minor problems: inappropriate aspect ratios, poor labels. | Graph(s) poorly chosen to support questions. |
|Presentation: tables | Table(s) carefully constructed to make it easy to perform important comparisons. Careful styling highlights important features. | Table(s) generally appropriate but possibly some minor formatting deficiencies.| Table(s) with too many, or inconsistent, decimal places. Table(s) not appropriate for questions and findings. Major display problems.|
|Achievement, mastery, cleverness, creativity|Student has gone beyond what was expected and required, e.g., extraordinary effort, additional tools not addressed by this course, unusually sophisticated application of tools from course.|Tools and techniques from the course are applied very competently and, perhaps,somewhat creatively. Chosen task was acceptable, but fairly conservative in ambition.|Student does not display the expected level of mastery of the tools and techniques in this course. Chosen task was too limited in scope.|
|Ease of access for instructor, compliance with course conventions for submitted work|Access as easy as possible, code runs! | Satisfactory | Not an earnest effort to reduce friction and comply with conventions  and/or code does not run|


## Guidelines for peer review of assignments

As part of this course you will be reviewing and providing feedback on other students' assignments. This is a serious responsibility: please put as much work into your feedback as you did into your original assignment.

### How to do peer review well

  * Give thoughtful, constructive and considerate comments. 
  * Be specific and concise.
  * Use the rubric above for ideas about criteria to evaluate and comment on (its not necessary to formalize a score (e.g. "excellent") for each component).
  * Try to learn something new and, if you succeed, point that out.
  * If you can't find anything to praise or that you found helpful, then at least offer some suggestions in a kind way.

### How to do peer review poorly

  * Your review is so generic that it's hard to determine which assignment you're reviewing.
  * Your review is mean.
  * You can't find anything to praise/learn and yet you don't offer any suggestions either.

### Additional resources:

Peer reviewing and critiquing others' work is a useful skill to develop during your studies. Although these links deal mainly with the peer review of academic papers, most of the key points are applicable to our peer review process.

* [Reviewing academic papers by Jeff Leek](https://github.com/jtleek/reviews/blob/master/README.md)

* [Edicts for peer reviewing (Ebb & Flow blog)](http://evol-eco.blogspot.ca/2014/09/edicts-for-peer-reviewing.html)

* [Faculty of 1000 Research: tips for peer reviewing](http://f1000research.com/peer-reviewing-tips)

* [The section entitled "How to perform the actual code review"](http://zonca.github.io/2014/08/code-review-for-scientific-computing.html)


* * *

These materials are adapted from those developed by Jenny Bryan at UBC.

