# AWS Flow Logs to Neo4j
I was doing some threat hunting, and needed to review AWS logs for malicious actors. I found so many I wanted a way to synthesize more information from all the data. 

Take all data needed, export to csv. All nodes have to be unique and contigous. Your relationships can store data that is non-contigous and unreliable (such as encrypted bytes are dashes and would cause an error).
![bloom-visualisation](https://user-images.githubusercontent.com/50241257/215506751-3b605ad1-902c-46a0-bf6b-e13162310a38.png)


### There are three main cell blocks in this example
* 1. Push external suspicious IP's that are the source going to internal IP's.
2. Push internal IP's as the source going to malicious IP's.
3. Clear the database to rerun the the above.


### Notes
* I seperate the source vs destination as malicious because malicious has different information. Such as in my case I was able to nest internal crowdstrike intel on nodes. Therefore if I didn't seperate the source and destination it would error out. 

 
### Contact
***If you have issues and need help reach out to colleybrb@gmail.com

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)




