# AWS Flow Logs to Neo4j
Take all data needed export to csv. All nodes have to be unique and contigous. Your relationships can store data that is non contigous and unreliable (such as encrypted bytes are dashes and would cause an error).


### There are three main cell blocks in this example
* 1. Push external suspicious IP's that are the source going to internal IP's.
2. Push internal IP's as the source going to malicious IP's.
3. Clear the database to rerun the the above.


### Notes
* I seperate the source vs destination as malicious because malicious has different information. Such as in my case I was able to nest internal crowdstrike intel on nodes. Therefore if I didn't seperate the source and destination it would error out. 

 
### Contact
***If you have issues and need help reach out to colleybrb@gmail.com




