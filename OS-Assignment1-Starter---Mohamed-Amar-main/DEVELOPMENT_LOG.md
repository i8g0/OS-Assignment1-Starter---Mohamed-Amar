# Development Log

## Entry 1
* **Date & Time:** Sunday, March 29, 2026, 4:00 PM
* **Task:** GitHub Setup and Code Review
* **Challenges:** Understanding the flow of the provided Round-Robin starter code and setting up the Git environment.
* **Solutions:** I carefully traced the `SchedulerSimulation.java` file, forked the repository, and successfully updated line 92 with my actual student ID to ensure unique outputs.
* **Time Spent:** 1 hour

## Entry 2
* **Date & Time:** Monday, March 30, 2026, 5:30 PM
* **Task:** Feature 1 - Implement Process Priority
* **Challenges:** Figuring out where to generate the random priority (1-5) and how to pass it to the objects.
* **Solutions:** I added a `priority` attribute to the `Process` class constructor. I generated a random number before creating the object in the main loop and updated the `addProcessToQueue` print statements to display it properly.
* **Time Spent:** 1 hour

## Entry 3
* **Date & Time:** Tuesday, March 31, 2026, 8:00 PM
* **Task:** Feature 2 - Count Context Switches
* **Challenges:** Identifying the exact moment a context switch happens during the scheduling loop.
* **Solutions:** I added a `public static int contextSwitches` variable in the main class. I incremented it right before calling `currentThread.start()` and printed the total after the while-loop finishes.
* **Time Spent:** 45 minutes

## Entry 4
* **Date & Time:** Wednesday, April 1, 2026, 9:30 PM
* **Task:** Feature 3 - Track Waiting Time
* **Challenges:** Calculating the waiting time was tricky because processes yield the CPU and re-enter the queue multiple times.
* **Solutions:** I introduced `creationTime`, `lastRunTime`, and `totalWaitingTime` to the `Process` class. I updated `lastRunTime` after each execution and added to the waiting time right before executing.
* **Time Spent:** 1.5 hours

## Entry 5
* **Date & Time:** Thursday, April 2, 2026, 3:00 PM
* **Task:** Formatting Output and Finalizing Documentation
* **Challenges:** Creating a clean, readable summary table for the waiting times at the end of execution while concurrent threads are running.
* **Solutions:** I created an `ArrayList` to store references to all generated processes. I used `System.out.printf` to loop through the list at the end of the simulation and print the formatted summary. I also finalized all markdown documentation files.
* **Time Spent:** 1 hour