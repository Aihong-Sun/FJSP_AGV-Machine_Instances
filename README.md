# FJSP_AGV-Machine_Instances
The Instances of AGV and machine integrated scheduling problem in flexible job shop

## Introduction to the problems corresponding to the Instances
The problem corresponding to the Instances set is the AGV and machine integrated scheduling problem in the flexible job shop, or the flexible job shop scheduling problem with AGV, or the flexible job shop scheduling problem considering transportation time.

The specific description is as follows :

n Jobs need to be processed on m machines, and the intermediate material transportation is completed by K AGVs ; each job contains n_j operations, and each operation can be processed by any machine from a given optional machine set. The processing time of the operation will vary with the different machine ; the transfer of jobs between machines is realized by a limited number of AGVs.For the transfer of any job, the time of AGV's action can be devided into pickup time and delivery time. The scheduling goal is to determine each operation processing machine, arrange the appropriate operation processing sequence and assign the job to the appropriate AGV for transportation, so as to minimize the total completion time.

## Introduction to Instances Set

### Benchmark DataSet

The first data set is 10 small instances modified by Bilge and Ulusoy [ 1 ] proposed by Deroussi and Norre [ 2], which is denoted as fjsp1 : 10, located in the file __fjspT.py__.

The second data set uses 48 small examples proposed by Kumer et al. [ 70 ].These 48 small examples are divided into two groups according to the ratio of transportation time t to processing time p. The first group is t / p > 0.25, which is denoted as EX ( t / p > 0.25 ). The second group is, this group is realized by multiplying the processing time of the original example by 2 and dividing the transportation time by 2, located in file __EX.py__ 

The third data set is obtained by extending the FJSP example proposed by Fattahi [ 71 ], which is denoted as Fattahi _ Set, located in __DataSet1/FJSP_Fttahi__,Other data sets in the Data _ Set1 file can also be used.

In all the above instances, the number of AGVs is 2, and need to combine the file __M4 _ to _ M18.py__ and __Generator_FJSPT.py__ to load single instances.

Loading the above example uses the function __Load_Instance_FJSPT()__ in __Generator_FJSPT.py__

### Self-generated instances

In the benchmark instances, only the case of 2 AGVs is considered. In order to further verify the effectiveness of the algorithm under different AGV numbers, this paper also generates the following three random instances :

(1) 12 small-scale instances, where the number of jobs is J = { 10,15,20 }, the number of machines is M = { 4,6,8 }, the number of AGVs is R = { 2,3 }, and the small-scale instances are located in file __small_scale__ ; 

(2) 20 medium-sized instances, where the number of jobs is J = { 30,40,50 }, the number of machines is M = { 8,10,15 }, the number of AGVs is R = { 3,4,6 }, the medium-sized instances  are located in file __middle_scale__ ;

(3) 27 large-scale instances, where the number of jobs is J = { 60,80,100 }, the number of machines is M = { 15,20,25 }, the number of AGVs is R = { 4,6,8 }, and the large-scale instances are located in file __large_scale__. 

Loading the above example uses the function __Load_Instance_Data_Set1()__ in __Generator_FJSPT.py__

### Note that the loading file is required to modify the corresponding path
















