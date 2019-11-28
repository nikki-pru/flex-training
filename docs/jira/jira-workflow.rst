Ticket Types and Workflow
==========================

`JIRA`_ is the ticketing system we use here at Liferay. Different ticket types have their own workflow as determined by the teams that use them. The following are general pointers to keep in mind when working on tickets.

LRQA tickets
-------------
LRQA tickets are used to manage QA work. When working on an LRQA ticket:

1. Assign the task to yourself before working on the ticket. This informs others that the ticket is being worked on and helps us avoid doing double work.
2. Change the status from Open to In Progress before working on the ticket.
3. When done, either close the ticket with the appropriate resolution or send to your lead for review.

LPS Bugs/Regression Bugs tickets
---------------------------------
An LPS ticket that is ready to be closed should be in Resolved status. When closing a ticket that is in Resolved status:

1. Assign the ticket to yourself.
2. Test the ticket to find out if the issue is fixed.
  a. If the issue is still reproducible, add a comment that the issue is reproducible (including the environment that it is reproduced on), put it in FAILED QA status and reassign the ticket to the dev who resolved the issue (see History or Activity).
  b. If the issue is no longer reproducible, close the ticket and add a comment following JIRA standards.

Story Tickets
--------------
A story ticket that is ready for testing will be in the READY FOR QA status.

1. Assign the ticket to yourself.
2. Test the ticket according to the indicated acceptance criteria.
3. Close the ticket and add a comment following JIRA standards.

.. note::
  Before assigning yourself to a ticket that is In Progress or In QA, check with the current assignee if you can take the ticket. This is to avoid having to do double work.


.. _JIRA: http://issues.liferay.com
