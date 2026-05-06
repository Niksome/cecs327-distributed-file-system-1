# cecs327-distributed-file-system-1
Repository to solve the assignment on Distributed File systems from the CECS 327 class at CUS Long Beach

Group members:
Andrej Ermoshkin
Ashley Celis
Fortune Meya

Before running you must install Pyro5:
pip install Pyro5

How to run: 
Step 1:  
Open terminal window #1 to start the server: python -m Pyro5.nameserver

Step 2: 
Open terminal window #2 to start the seed node: python server.py --bootstrap --port 9000

Step 3: 
Open terminal window #3 to create the file: python client.py touch sample.txt

Step 4: 
Add data to the created file: python client.py append sample.txt localdata.txt

Step 5: 
Sort the data in the file: python client.py sort sample.txt sortedsample.txt

Step 6: 
Verify that the sort worked: python client.py read sortedsample.txt
