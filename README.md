# Using GitHub Classroom for UiT Courses

Lars Ailo Bongo (larsab@cs.uit.no)

Please help improving this guide by fixing mistakes, adding clarifications, and new tips.

This is the unofficial guide for using GitHub for UiT courses. We recommend using GitHub instead of Fronter for three reasons. First, we believe in open access publication and believe that it should apply for our courses as well as research results. Second, we believe that our students should be trained to use professional collaboration and version management tools. Third, we really do not like Fronter.

This guide consist of step-by-step instructions and tips for setting up a GitHub organization and using a repository for publishing a course website. In addition, we describe how to use GitHub Classroom for handing out and managing mandatory assignments.

## GitHub Organization

First we need an organization that we will use to administer the content and members of the course. You need to create a new organization each time the course is given.

1. Go to: https://github.com/organizations/new
2. Give the organization a name using the following naming scheme: uit-(course code)-(f for fall or s for spring)(year). For example the name for the inf-2202 course given in the fall of 2016 is **uit-inf-2202-f16**
3. Choose a plan with unlimited members and public repositories for free. 
4. Invite the teach assistants to the organization. You need to know their GitHub usernames.
5. Fill in organization details.

Then:

6. Create a new Team called **Owners** with all teaching staff as members. This team will be given automatic access to the student repositories created as described below.
7. In your organizations members list, make at least yourself “public” such that your membership is visible to everyone and displayed on your public profile.

Then students must be invited to join the organization. To do this you need to know their GitHub username. You may want to put all students into a team named “Students”.

## Course Website

To create a website for the course that can be updated by pushing to a repository, do the following:

1. In your organization, create a new public repository named (organization name).github.io. For the uit-inf-2202-f16 organization the name is uit-inf-2202-f16.github.io.
2. Give the Owners time write access to the repository.
2. Clone and push the content of this repository, that contains a website with a UiT layout, to your repository. 
3. Modify the syllabus in the index.md Markdown file in your repository.
4. Modify the README.md file in your repository. You may for example say that “This is the syllabus for (your course)…”

The index.md will automatically be converted to an HTML file and shown at the address (repository name). For example, the uit-inf-2202-f16.github.io repository is at https://uit-inf-2202-f16.github.io/

You and the TA’s in the Owners team can now update the syllabus, add lecture notes, and so on by pushing to the repository.

If possible, creating a redirect in the UiT web server makes it easier to remember the course website address. The inf-2202 course is for example redirected from: http://www.cs.uit.no/kursinfo/inf2202

## Managing Assignments

To manage mandatory assignments you should use GitHub Classroom as follows:

1. Goto https://classroom.github.com/classrooms and create a new classroom that is linked to your course organization.
2. Apply for an education discount at https://education.github.com/discount_requests/new. This will give your organization private repositories needed for individual and group assignments. **Note** processing a request takes several days, so make sure that this is done weeks before you hand out the first assignment.

For each assignment:

1. Create a public repository in your organization where you put the assignment description, pre-code, etc
2. In GitHub classroom create a new assignment. The assignment can be either individual or for a group.
3. Distributed the link for the assignment to the students. 

For individual assignments GitHub will automatically create a new private repository for the student in the course organization. Only the student and the members in the Owners team have access to this repository.

For group assignments GitHub will automatically create a new private repository for the group. It will also give the students the opportunity to create and join teams.

For hand-in. Simply pull the content of all repositories.

## Useful tips

This is a list of useful tips for managing your course:
* Create a mailing list for the course at: https://list.uit.no/sympa
* Turn of automatic watching of repositories at https://github.com/settings/notifications to avoid receiving an email each time a student commits to a repository.
* If you are using (an OAuth) git client such as SmartGit you may need to grant access to the new repository.
* Create a Slack team for the course (free, unlimited users, but only 10K most recent messages are saved): https://slack.com/
* Add a GitHub boot to a slack room to automatically notify the team when the course website is changed.
