# Workflow

## Plan at first
Describe the task objectives in Cascade panel.

Prompt:
```
I have an existing codebase that requires modifications. My planned tasks are:
1. Make alterations to `filename1`
2. Implement updates in `filename2`
3. Perform a review of `filename3`

Please provide guidance on how to PLAN these tasks without proceeding to implementation.
In your PLAN, include the specific commands I should execute for each step.
If you need any clarification, please ask before proceeding.
```

Review the task plan, make sure everything is clear and reasonable.

## Fix bugs
Prompt:
```
Reflect on 5-7 different possible sources of the problem, distill those down to 1-2 most likely sources, and then add logs to validate your assumptions before we move onto implementing the actual code fixes.
```

## Write plan
Prompt:
```
create a `todolist.md` file, use check boxes and list all the tasks you need to complete. make each task a tick box, put bullet points below it. 
```

## Implement plan
Prompt:
```
We need to follow `todolist.md` one by one because there are multiple things we need to accomplish and we should do them one at a time and test them before moving on to the next part.

once completed, you can work down the task list one at a time ticking them off.

It's critical that all of the changes we make are done in a surgical way, with minimal code changes when possible. We must be very careful not to break or remove existing functionality. Do not introduce any new bugs or syntax errors.
```
