### 3/10/24

- [x] Try to find GPUs jobs that are longer than a month (there are some in 2024) and see if they are not lost in the "year" analysis
- [x] Update yearly function to merge entire year rather than iterate over months -> **EQUAL BUT SLOWER!**
- [ ] Check cross year for yearly, or cross month for monthly
- [x] One more time interval to handle: from date to date (vs particular year or a month)
- [ ] Other items from Katia's list [https://github.com/bu-rcs/gpu_util/blob/katia/Questions.md]
- [ ] CLI tool with python to get all useful information for a user, see qaccct -j \<jobid\>
- [ ] Show util for user, gpu memory usage
- [ ] Data viz should show gpu util based on used/total over time
- [ ] Shared vs buy in, <5% util, etc. fixes  


## Findings:  
- merging all files at once for yearly has same dataframe but is much slower
- investigating missing values: since using util as main table and merging accounting, we miss info for jobs that finish after the month
