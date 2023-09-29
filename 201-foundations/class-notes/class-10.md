# Class 10 (29/09/2023)

## Lab Review

- Add hourly total on footer

## Debugging

- First thing is to go to the console log.
- Always add console log to check errors.
- Delete console log when all is fixed.
- console.log(typeof a) --> tells you the type of "a" (string, number, boolean).
- Most common mistakes are spelling errors, order of function calls, and name incongruencies (capital letters...).

- Functions can be declared anywhere; they will only run whenever they are invoked. You can write the call before the declaration and it will run.
- Variables need to be declared before the function for it to run.

## GitHub branches

- Branches are useful to work on a new website feature without affecting the live website.
- The branch will create a copy of the code you are working on.

- On terminal(to create and move to a new branch):
  git checkout -b add-new-content --> add-new-content is the name of the branch. We don't use ""

  - When you acp for the first time after creating a new branch, you need to
    git push -u origin add-new-content.
  - After you acp, on GitHub you need to pull request into the main branch once you are finished with the branch.
    - update: new content added. You can also add a comment, if required.
  - After reviewing the changes, you can merge changes.
  - When you merge content and you want to see the changes in the main branch locally, you need to git pull.

- On terminal:
  git checkout is used to change branches.
- It is best practice to delete branches when you are finished with them.
