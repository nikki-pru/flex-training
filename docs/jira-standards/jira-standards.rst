JIRA Ticket Standards
======================

`JIRA`_ is the ticketing system we use here at Liferay. Because it is used by most business functions, it is good to have some standards when interacting with others over JIRA tickets. These are not arbitrary standards but are best practices we’ve developed over the years to efficiently get information across to a developer, another viewer, or for reporting purposes. We work with developers and team members across different time zones and cultures and the more efficiently we get our point across the first time, the faster we get results.

Filing a bug ticket
--------------------
When filing bug tickets it is important to inform others on how the issue was reproduced and on what GIT IDs it was reproduced on. Attached GIFs or images are also helpful. Example, `LPS-103947`_.
::
    *Steps to Reproduce:*
    # Step 1
    # Step 2
      a. Step 2.1
      b. Step 2.2
    # Step 3

    *Expected Result:*
      What the expected behavior should be.

    *Actual Result:*
      What actually happened.

    *Reproduced on:*
      {appserver.version} + {db.version}
      Portal {version} GIT ID: #######################


Closing bug tickets
--------------------
There are multiple scenarios that can happen when closing a bug ticket. As in Filing a Bug Ticket, steps and GIT ID are important to document how or when the bug was closed in case the ticket needs to be referenced later on. The first thing to do is to Manually test the ticket to see if the issue is no longer reproducible

Fixed
^^^^^^
A bug ticket should be closed as fixed when there is a linked pull request. Example: `LPS-103737`_

*When steps are included in the description*
::
    *PASSED* Manual Testing following the steps in the description

    Fixed on:
    {appserver.version} + {db.version}
    Portal {version} GIT ID: #######################

    A short summary of observed behavior.

*When steps are not included in the description*
::
    *PASSED* Manual Testing using the following steps:

    #. Step 1
    #. Step 2
    #. Step 3

    Fixed on:
    {appserver.version} + {db.version}
    Portal {version} GIT ID: #######################

    A short summary of observed behavior.

No Longer Reproducible
^^^^^^^^^^^^^^^^^^^^^^^
A ticket is no longer reproducible when there is not linked pull request. The issue may have been fixed together with a fix for a different ticket. Example, `LPS-103861`_.

*When steps are included in the description*
::
    *No longer reproducible** following the steps in the description

    No longer reproducible on:
    {appserver.version} + {db.version}
    Portal {version} GIT ID: #######################

    A short summary of observed behavior.

*When steps are not included in the description*
::
    **No longer reproducible** using the following steps:
    # Step 1
    # Step 2
    # Step 3

    No longer reproducible on:
    {appserver.version} + {db.version}
    Portal {version} GIT ID: #######################

    A short summary of observed behavior.



.. _JIRA: http://issues.liferay.com
.. _LPS-103947: https://issues.liferay.com/browse/LPS-103947
.. _LPS-103737: https://issues.liferay.com/browse/LPS-103737
.. _LPS-103861: https://issues.liferay.com/browse/LPS-103861
