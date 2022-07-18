# Frequent-Itermset-Mining
Effiecient implementation of Apriopri and FP-growth algorithm to mine frequent items
Dataset used- Retail data of an anonymous store in belgium: http://fimi.ua.ac.be/data/retail.dat, more details available at http://fimi.ua.ac.be/data/retail.pdf

##Running
Executing the command: ```sh run.sh retail.txt X -apriori output``` generates a file output.txt containing the frequent itemsets at >=X% support threshold with the Apriori algorithm. Similarly, executing the command ```sh run.sh retail.txt X -fptree output``` generates a file output.txt containing the frequent itemsets using FP-tree algorithm. 
X is in percentage and not the absolute count. Our implementations ensure that the transactions are not loaded into main memory. However, the frequent patterns and candidate sets are stored in memory.
