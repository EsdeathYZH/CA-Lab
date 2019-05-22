## Lab1:Benchmarking
### 1. Download Rodinia and build BFS
### 2. Simulate BFS with GPGPU-sim.
Follow instructions in lab document.
### 3. What's your L1 data cache miss rate? (15%)
L1D_total_cache_miss_rate = 0.3234
L1D_total_cache_miss_rate = 0.3388
L1D_total_cache_miss_rate = 0.3806
L1D_total_cache_miss_rate = 0.4407
L1D_total_cache_miss_rate = 0.4034
L1D_total_cache_miss_rate = 0.4529
L1D_total_cache_miss_rate = 0.4064
L1D_total_cache_miss_rate = 0.4202
L1D_total_cache_miss_rate = 0.4535
L1D_total_cache_miss_rate = 0.4578
L1D_total_cache_miss_rate = 0.3944
L1D_total_cache_miss_rate = 0.3973
L1D_total_cache_miss_rate = 0.3927
L1D_total_cache_miss_rate = 0.3924
L1D_total_cache_miss_rate = 0.3922
L1D_total_cache_miss_rate = 0.3919
### 4. What's your average memory fetch latency? (15%)
averagemflatency = 259 
averagemflatency = 220 
averagemflatency = 196 
averagemflatency = 184 
averagemflatency = 172 
averagemflatency = 170 
averagemflatency = 177 
averagemflatency = 177 
averagemflatency = 233 
averagemflatency = 232 
averagemflatency = 229 
averagemflatency = 229 
averagemflatency = 227 
averagemflatency = 227 
averagemflatency = 227 
averagemflatency = 227
### 5. Name several characteristic of BFS based on your results, such as cache, memory and instructions. (15%)
First I check I-cache miss rate:
L1I_total_cache_miss_rate = 0.1653
L1I_total_cache_miss_rate = 0.1979
L1I_total_cache_miss_rate = 0.1236
L1I_total_cache_miss_rate = 0.1020
L1I_total_cache_miss_rate = 0.0569
L1I_total_cache_miss_rate = 0.0522
L1I_total_cache_miss_rate = 0.0264
L1I_total_cache_miss_rate = 0.0259
L1I_total_cache_miss_rate = 0.0165
L1I_total_cache_miss_rate = 0.0166
L1I_total_cache_miss_rate = 0.0134
L1I_total_cache_miss_rate = 0.0136
L1I_total_cache_miss_rate = 0.0132
L1I_total_cache_miss_rate = 0.0134
L1I_total_cache_miss_rate = 0.0134
L1I_total_cache_miss_rate = 0.0136
We can see that the miss rate goes down with iterations.

And L2-cache miss rate:
L2_total_cache_miss_rate = 0.7609
L2_total_cache_miss_rate = 0.4897
L2_total_cache_miss_rate = 0.3891
L2_total_cache_miss_rate = 0.2594
L2_total_cache_miss_rate = 0.2063
L2_total_cache_miss_rate = 0.1606
L2_total_cache_miss_rate = 0.1137
L2_total_cache_miss_rate = 0.1058
L2_total_cache_miss_rate = 0.0550
L2_total_cache_miss_rate = 0.0537
L2_total_cache_miss_rate = 0.0442
L2_total_cache_miss_rate = 0.0435
L2_total_cache_miss_rate = 0.0427
L2_total_cache_miss_rate = 0.0426
L2_total_cache_miss_rate = 0.0426
L2_total_cache_miss_rate = 0.0425

Network latency average = 8.41848
Network latency average = 8.41848 (1 samples)
Network latency average = 7.90196
Network latency average = 8.16022 (2 samples)
Network latency average = 7.44361
Network latency average = 7.92135 (3 samples)
Network latency average = 12.05
Network latency average = 8.95351 (4 samples)
Network latency average = 7.88135
Network latency average = 8.73908 (5 samples)
Network latency average = 15.3602
Network latency average = 9.84259 (6 samples)
Network latency average = 12.9038
Network latency average = 10.2799 (7 samples)
Network latency average = 15.5778
Network latency average = 10.9422 (8 samples)
Network latency average = 23.5866
Network latency average = 12.3471 (9 samples)
Network latency average = 15.5147
Network latency average = 12.6638 (10 samples)
Network latency average = 17.2559
Network latency average = 13.0813 (11 samples)
Network latency average = 15.3006
Network latency average = 13.2662 (12 samples)
Network latency average = 16.5529
Network latency average = 13.5191 (13 samples)
Network latency average = 7.80952
Network latency average = 13.1112 (14 samples)
Network latency average = 8.26923
Network latency average = 12.7884 (15 samples)
Network latency average = 8.29412
Network latency average = 12.5075 (16 samples)

## Lab2:Schedule policy
### 1. Modify '-gpgpu_scheduler' in gpgpusim.config to switch schedule policies.
### 2. Build and simulate 'pathfinder' with parameters ‘ 1000 100 20’ with all three schedule policies.
Follow instructions in lab document.
### 3. What is the runtime, simulation rate (cycle/sec) for each configuration? (15%)
+ GTO
gpgpu_simulation_rate = 451280 (inst/sec)
gpgpu_simulation_rate = 4839 (cycle/sec)
gpgpu_simulation_rate = 386811 (inst/sec)
gpgpu_simulation_rate = 4007 (cycle/sec)
gpgpu_simulation_rate = 406152 (inst/sec)
gpgpu_simulation_rate = 4158 (cycle/sec)
gpgpu_simulation_rate = 416566 (inst/sec)
gpgpu_simulation_rate = 4147 (cycle/sec)
gpgpu_simulation_rate = 418918 (inst/sec)
gpgpu_simulation_rate = 4102 (cycle/sec)

gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 3 sec (3 sec)
gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 7 sec (7 sec)
gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 10 sec (10 sec)
gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 13 sec (13 sec)
gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 16 sec (16 sec)

+ LRR
gpgpu_simulation_rate = 338460 (inst/sec)
gpgpu_simulation_rate = 3702 (cycle/sec)
gpgpu_simulation_rate = 338460 (inst/sec)
gpgpu_simulation_rate = 3572 (cycle/sec)
gpgpu_simulation_rate = 312424 (inst/sec)
gpgpu_simulation_rate = 3260 (cycle/sec)
gpgpu_simulation_rate = 338460 (inst/sec)
gpgpu_simulation_rate = 3431 (cycle/sec)
gpgpu_simulation_rate = 335134 (inst/sec)
gpgpu_simulation_rate = 3343 (cycle/sec)

gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 4 sec (4 sec)
gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 8 sec (8 sec)
gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 13 sec (13 sec)
gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 16 sec (16 sec)
gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 20 sec (20 sec)

+ TL
gpgpu_simulation_rate = 338460 (inst/sec)
gpgpu_simulation_rate = 3718 (cycle/sec)
gpgpu_simulation_rate = 386811 (inst/sec)
gpgpu_simulation_rate = 4110 (cycle/sec)
gpgpu_simulation_rate = 406152 (inst/sec)
gpgpu_simulation_rate = 4262 (cycle/sec)
gpgpu_simulation_rate = 416566 (inst/sec)
gpgpu_simulation_rate = 4247 (cycle/sec)
gpgpu_simulation_rate = 418918 (inst/sec)
gpgpu_simulation_rate = 4201 (cycle/sec)

gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 4 sec (4 sec)
gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 7 sec (7 sec)
gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 10 sec (10 sec)
gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 13 sec (13 sec)
gpgpu_simulation_time = 0 days, 0 hrs, 0 min, 16 sec (16 sec)
### 4. List L1 data cache miss rate, average memory fetch latency of three schedule policies. (20%)
+ GTO
L1D_total_cache_miss_rate = 0.5653
L1D_total_cache_miss_rate = 0.5653
L1D_total_cache_miss_rate = 0.5653
L1D_total_cache_miss_rate = 0.5653
L1D_total_cache_miss_rate = 0.5680

averagemflatency = 263 
averagemflatency = 254 
averagemflatency = 251 
averagemflatency = 252 
averagemflatency = 251
+ LRR
L1D_total_cache_miss_rate = 0.5653
L1D_total_cache_miss_rate = 0.5653
L1D_total_cache_miss_rate = 0.5653
L1D_total_cache_miss_rate = 0.5653
L1D_total_cache_miss_rate = 0.5680

averagemflatency = 265 
averagemflatency = 260 
averagemflatency = 256 
averagemflatency = 252 
averagemflatency = 253
+ TL
L1D_total_cache_miss_rate = 0.5653
L1D_total_cache_miss_rate = 0.5653
L1D_total_cache_miss_rate = 0.5653
L1D_total_cache_miss_rate = 0.5653
L1D_total_cache_miss_rate = 0.5680

averagemflatency = 264 
averagemflatency = 260 
averagemflatency = 255 
averagemflatency = 253 
averagemflatency = 252
