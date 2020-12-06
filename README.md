# BD_0087_0196_0230_0252_Project
<h2>Folder Structure</h2>
 - src

    - Master.py
  
    - Worker.py
  
    - Analysis.py
  
-logs

    - logs_RR.txt
  
    - logs_LL.txt
  
    - logs_RA.txt
  

<h3>Steps to run:</h3>

- src folder has the Master.py, Worker.py, Analysis.py and also config.json and
<br></br>
- Run the Master.py with command 
 ```python
    $ python3 Master.py <Config.json> <Scheduling Algo(RR/LL/RA)>
  ```
 - Run three workers with the following commands
 ```python
    $ python3 Worker.py <port[4000/4001/4002]> <worker_id[1/2/3]>
 ```
 - Then run the requests.py to generate task queue
 ```python
    $ python3 requests.py <no_of_requests>
 ```
- 3 log files are then created and Analysis.py helps in analysing them. To run it
 ```python
    $ python3 Analysis.py
 ```