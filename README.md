# Job-Concurrency
Concurrency controls how many workflow runs can execute at the same time.

# Exmaple: Suppose you push code 3 times quickly:

* Push 1 → Workflow Running
* Push 2 → Workflow Running
* Push 3 → Workflow Running

Now 3 workflows are running simultaneously, wasting time and resources.

# In Concurrency

* Push 1 → Workflow Running
* Push 2 → Cancels Push 1 and Starts New Run
* Push 3 → Cancels Push 2 and Starts New Run
