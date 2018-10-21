.. include:: ../Includes.txt
.. highlight:: rst

.. _general-conventions-commit-messages:

===============
Commit messages
===============


Benefits of good commit messages
================================

There are several good reasons to have commit message rules or recommendations
and write good commit messages.

* The commit messages help to get an overview of the latest changes. This can
  be used to write news messages for the docs.typo3.org homepage. That way 
  we can inform people of important changes. If commits
  only consist of vague commit message, it is more tedious to find out 
  what was changed recently.
* The commit messages should be readable on the web (on the Github page),
  in the terminal (`git log`) or with a git UI tool. For this reason, it
  makes sense to stick to the max line length rules
* The commit message can be used to link to the issue.
* It is a good idea to have keywords, which distinguish bugfixing
  from new features.
  
Commit message recommendations
==============================

* Write commit messages that are **clear**, **concise** and **meaningful**
* Use imperative form: "Fix typo" (instead of "Fixed typo"). This is
  seen from the person, that is going to apply your patch: What will the patch do?
  Fix typo! See  `How to write a git commit message <https://chris.beams.io/posts/git-commit/>`__


A commit message for the docs should consists of a subject line. More lines
are optional. If you can find a meaningful subject line for your change, 
you do not necessarily need to elaborate this. If an issue exists, link to 
it. 

Example commit message:

.. code-block:: none

   [NEW] Add chapter for commit message rules

   Resolves: #4
   
This consists of the following parts:

.. code-block:: none

   [CATEGORY] subject

   Resolves: issue number
   
The issue number is optional. Github will automatically create a link to
the issue. 


.. code-block:: none

   Related: #issue

or

.. code-block:: none


   Resolves: #issue

Using resolves, will automatically close the issue. You can refer to more than one issue.

The following categories can be used:

* **[NEW]** : for new documentation. If you add a manual, a chapter, a section or a 
  new sentence, just use [NEW]
* **[FIX]** : for fixing something. Can be a typo, an outdated code sample or somehting
  that is just plain wrong
  
As in the TYPO3 core commit message rules, keep the whole line below 52 characters
if possible, but below 80 in any case.   


   


