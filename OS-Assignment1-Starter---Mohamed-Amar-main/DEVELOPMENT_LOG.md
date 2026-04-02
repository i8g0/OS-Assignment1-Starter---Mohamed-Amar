# Development Log

## Entry 1
* **Date & Time:** March 27, 2026, 4:00 PM
* **Task:** GitHub Account & Repository Setup
* **Challenges:** Understanding how to properly fork the repository and ensure it is public while using the university email.
* **Solutions:** Carefully followed the instructions in the README, created the fork, and updated line 92 in `SchedulerSimulation.java` with my actual student ID.
* **Time Spent:** 45 minutes

## Entry 2
* **Date & Time:** March 28, 2026, 5:30 PM
* **Task:** Feature 1 - Implement Process Priority
* **Challenges:** Deciding where to generate the random priority (1-5) and how to pass it correctly to the `Process` class.
* **Solutions:** Added a `priority` attribute to the `Process` class constructor. Generated a random number in the `main` method before object creation and updated the `addProcessToQueue` print statement to display it.
* **Time Spent:** 1 hour

## Entry 3
* **Date & Time:** March 28, 2026, 8:00 PM
* **Task:** Feature 2 - Count Context Switches
* **Challenges:** Identifying the exact point in the code where a context switch actually occurs.
* **Solutions:** Added a `public static int contextSwitches` variable in the `SchedulerSimulation` class. Incremented it right before calling `currentThread.start()` in the scheduler loop, and printed the total at the end.
* **Time Spent:** 30 minutes

## Entry 4
* **Date & Time:** March 29, 2026, 1:00 AM
* **Task:** Feature 3 - Track Waiting Time
* **Challenges:** Calculating the waiting time was tricky because a process can run, go back to the queue, and wait again. 
* **Solutions:** Added `creationTime` and `lastRunTime` to the `Process` class. Updated `lastRunTime` every time the process finishes a quantum, and accumulated the waiting time before each execution.
* **Time Spent:** 1.5 hours

## Entry 5
* **Date & Time:** March 29, 2026, 2:30 AM
* **Task:** Finalizing output and summary table
* **Challenges:** Formatting the final waiting time summary table to look clean and professional in the terminal.
* **Solutions:** Used `System.out.printf` for formatted columns and created an `ArrayList` to keep track of all processes during creation so I could iterate over them at the end of the simulation to print their stats.
* **Time Spent:** 45 minutes
