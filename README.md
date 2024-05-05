# README
# Maysan Chelbi 2201130563
- I used Python language using PyCharm Community.

- I have four files: PPscheduler, RRscheduler, SRTFscheduler, CustomShceduler

- You should open the file and right click in mouse then choose --> (Run'PPscheduler'), same thing for other files.




# PPscheduler:
- Task Class: represent a process, and it has an attributes (pid, arrival_time, burst_time, remaining_time, priority, waiting_time, response_time).

- Scheduler Class: represent a scheduler, has a method 'run_simulation' to be implemented by subclass.

- PPscheduler Class (Subclass of Scheduler): 
         * it iterates over tasks, sorts them based on priority, and executes them one by one, updating waiting and response times.

- parse_input() Function: parse the input file containing task information, read the list of tasks then return it.

- main() Function: Parses the input file, initializes the scheduler with tasks, and runs the simulation. Prints statistical information like average waiting time, response time, and turnaround time.



## RRscheduler:
- Task Class: represent a process, and it has an attributes (pid, arrival_time, burst_time, remaining_time, priority, waiting_time, response_time).

- Scheduler Class: represent a scheduler, has a method 'run_simulation' to be implemented by subclass.

- RRscheduler Class (Subclass of Scheduler):
         * Inherits from the Scheduler class. 
         * Constructor takes an additional parameter time_slice, representing the time quantum for RR scheduling. 
         * Method run_simulation() runs the scheduling simulation. 
         * It iterates over tasks, executes them for the time quantum or until completion, and updates waiting and response times accordingly.


- parse_input() Function: parse the input file containing task information, read the quantum and the list of tasks then return them.

- main() Function: Parses the input file, initializes the scheduler with tasks, and runs the simulation. Prints statistical information like average waiting time, response time, and turnaround time.




### SRTFscheduler:

- Task Class: represent a process, and it has an attributes (pid, arrival_time, burst_time, remaining_time, priority, waiting_time, response_time).

- Scheduler Class: represent a scheduler, has a method 'run_simulation' to be implemented by subclass.

- SRTFscheduler Class (Subclass of Scheduler): 
       * Method run_simulation() executes the SRTF scheduling algorithm. 
       * Sorts tasks based on their remaining time. 
       * Executes the task with the shortest remaining time for one unit of time. 
       * Updates waiting and response times accordingly. 
       * Calculates and returns average waiting time, response time, and turnaround time. 

- parse_input() Function: parse the input file containing task information, read the list of tasks then return it.

- main() Function: Parses the input file, initializes the SRTF scheduler with tasks, and runs the simulation. Prints statistical information like average waiting time, response time, and turnaround time.






#### CustomScheduler:
- Task Class: represent a process, and it has an attributes (pid, arrival_time, burst_time, remaining_time, priority, waiting_time, response_time).

- Scheduler Class: represent a scheduler, has a method 'run_simulation' to be implemented by subclass.

- CustomScheduler (Subclass of Scheduler): 
      * Method run_simulation() executes the custom scheduling algorithm.
      * Pops the first task in the list. 
      * Executes the task for its burst time.
      * Updates waiting and response times accordingly.
      * Updates waiting and response times accordingly.


- parse_input() Function: parse the input file containing task information, read the list of tasks then return it.

- main() Function: Parses the input file, initializes the SRTF scheduler with tasks, and runs the simulation. Prints statistical information like average waiting time, response time, and turnaround time.













