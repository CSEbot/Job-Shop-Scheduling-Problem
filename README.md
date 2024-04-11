# Job-Shop-Secheduling-Problem
This project aimed to further my undestanding of the Simulated Annealing Algorithm by applying it to the job shop scheduling problem. 
# Project Specification
To gain a thorough understanding of how the Simulated Annealing (SA) algorithm can be applied to solve a real-world scheduling problem. Unlike Project 1 this project will focus on a different type of optimization problem which is the Job Shop scheduling problem. This is a problem that occurs commonly in Industry across a number of different application domains. Some applications of job shop scheduling include process scheduling at a server farm, packet routing across a computer network, job scheduling at a manufacturing plant, amongst many others.
In job scheduling J jobs are scheduled for processing at M machines. Each job has a fixed number of operations (N). The problem then is to allocate the jobs and their corresponding operations such that the overall completion time (referred to as the makespan) is minimized.
# Environment Description
The environment is a simple one consisting of jobs and machines. Jobs have different completion times but have no constraints as to their starting time. The only constraint on a job is that its operations must run in strict sequence. Thus, for example operation J11 of job 1 must be scheduled before operation J12 of job 2. All machines may be assumed to have the same processing power. The operational times for each job are known in advance.
# Job/Operating Scheduling
cheduling is performed at the Job level, not at the operation level. Once an ordering of jobs is determined then that order is used consistently for all machines. Thus, if there are two machines, then the jobs execute in exactly the same sequence on both machines. The scheduler will exploit the availability of multiple machines by scheduling different job operations to run concurrently (at the same time) so as to minimize overall job completion time. Thus, an efficient schedule will maximize the use of parallelism across machines while minimizing idle time (i.e., waiting for other jobs to complete) on individual machines.
# Strategy 
The overall strategy is to use the SA algorithm to perform scheduling. This will involve specification of the successor function, the value function, and the temperature schedule.
# Implementation
Fully implement the SA algorithm that you designed in Part A in a Python notebook and deploy it in Collab for each of the 3 scenarios given as R3, R4 and R5 below.
R3: 
Use the jobs specified in Table 1 of  Tutorial 3. Your code should display the makespan for this job mix. Compare the makespan value with the value 27 which is the optimal schedule. For a definition of the makespan see Tutorial 3. 
R4: 
Create 50 jobs randomly with 3 operations per job. For each job randomly generate the 3 operation times in the range [5,50]. The jobs need to be scheduled to 5 machines. 
What is the makespan value returned by your SA algorithm? Compare this makespan value with the makespan returned from your initial random solution that you used to start off the SA algorithm.
R5: 
Create 50 jobs randomly with 5 operations per job. For each job randomly generate the 5 operation times in the range [5,50]. The jobs need to be scheduled to 3 machines. 
What is the makespan value returned by your SA algorithm? Compare this makespan value with the makespan returned from your initial random solution that you used to start off the SA algorithm.
