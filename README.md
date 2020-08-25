# Using GitHub Classroom for UiT courses

Contacts:
- Lars Ailo Bongo (larsab@cs.uit.no)
- Radovan Bast (radovan.bast@uit.no)

Please help improving this guide by fixing mistakes, adding clarifications, and new tips.

This is the unofficial guide for using GitHub for UiT courses.

We recommend using GitHub for two reasons:
- We believe in open access publication and believe that it should apply for our courses as well as research results.
- We believe that our students should be trained to use professional collaboration and version management tools.

This guide consist of step-by-step instructions and tips for setting up a
GitHub organization and using a repository for publishing a course website. In
addition, we describe how to use [GitHub Classroom](https://classroom.github.com/)
for handing out and managing mandatory assignments.


## GitHub organization

First we need an organization that we will use to administer the content and
members of the course. You need to create a new organization each time the
course is given. The reason for this is that each course needs to be attached
to a GitHub organization and that GitHub Classroom requires course TAs to have *owner* access in the
corresponding organization.

1. Go to: https://github.com/organizations/new
2. Choose the *Free* plan (unlimited repositories, unlimited collaborators).
3. Give the organization a name using the following naming scheme: uit-(course
   code)-(f for fall or s for spring)(year). For example the name for the
   inf-2202 course given in the fall of 2016 is **uit-inf-2202-f16**
4. "This organization belongs to:" choose "A business or institution"
   and "UiT The Arctic University of Norway".
5. Invite the teach assistants to the organization as owners. You need to know
   their GitHub usernames.
6. Fill in organization details.
7. In your organizations members list, make at least yourself "public" such
   that your membership is visible to everyone and displayed on your public
   profile so that the organization has a contact point.
8. We recommend enabling two factor authentication for the organization.

Then students must be invited to join the organization. They can either be manually 
added, but to do this you need to know their GitHub username. Alternatively, students
can be automatically added to the organization by sending them the GitHub Classroom link
to the first assignment. But you still need to map the GitHub usersnames with their real names.

## Course website

You can create the course website from
[this template](https://github.com/uit-no/github-course-template)
by following the instructions at
https://github.com/uit-no/github-course-template/blob/master/README.md.


## Managing assignments

To manage mandatory assignments you should use GitHub Classroom as follows:

1. Create a [new classroom](https://classroom.github.com/classrooms/new) and
   link it to the GitHub organization which you just created (above). You may
   need to grant access to the course organization.
2. Give your TAs the link to the new classroom.

For each assignment:

1. Create a public repository in your organization where you put the assignment
   description, pre-code, etc.
2. In GitHub classroom create a new assignment. The assignment can be either
   individual or for a group.
3. Distribute the link for the assignment to the students.

For individual assignments GitHub will automatically create a new private
repository for the student in the course organization. Only the student and
thew owners team have access to this repository.

For group assignments GitHub will automatically create a new private repository
for the group. It will also give the students the opportunity to create and
join teams.

For hand-in. Simply pull the content of all repositories.


## Tips

- Turn of automatic watching of repositories at
  https://github.com/settings/notifications to avoid receiving an email each
  time a student commits to a repository.
- If you are using (an OAuth) Git client such as SmartGit you may need to grant
  access to the new organization.
- Create a Slack team for the course (free, unlimited users, but only 10K most
  recent messages are saved): https://slack.com/
- Add a GitHub bot to a Slack channel to automatically notify the team when the
  course website is changed.
