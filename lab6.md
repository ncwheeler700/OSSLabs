# Lab 6

## 1. Five letter pairs results
Loaded words_dat.txt containing 5757 five-letter English words.  
Two words are connected if they differ in one letter.  
Graph has 5757 nodes with 14135 edges  
853 connected components  
Shortest path between chaos and order is  
chaos  
choos  
shoos  
shoes  
shoed  
shred  
sired  
sided  
aided  
added  
adder  
odder  
order  
Shortest path between nodes and graph is  
nodes  
lodes  
lores  
lords  
loads  
goads  
grads  
grade  
grape  
graph  
Shortest path between moron and smart is  
moron  
boron  
baron  
caron  
capon  
capos  
capes  
canes  
banes  
bands  
bends  
beads  
bears  
sears  
stars  
start  
smart  
Shortest path between pound and marks is  
None  

## 2. Diff of provided code to work with 4 letters
61c61  
<     fh = gzip.open('words_dat.txt.gz', 'r')  
\---  
\>     fh = gzip.open('words4_dat.txt.gz', 'r')  
67c67  
<         w = str(line[0:5])  
\---  
\>         w = str(line[0:4])  
74c74  
<     print("Loaded words_dat.txt containing 5757 five-letter English words.")  
\---  
\>     print("Loaded words_dat.txt containing %d four-letter English words." % (nx.number_of_nodes(G)))  
80,83c80,81  
<     for (source, target) in [('chaos', 'order'),  
<                              ('nodes', 'graph'),  
<                              ('moron', 'smart'),  
<                              ('pound', 'marks')]:  
\---  
\>     for (source, target) in [('warm', 'cold'),  
\>                              ('love', 'hate')]:  

## 3. Four letter pair results
Loaded words_dat.txt containing 2174 four-letter English words.  
Two words are connected if they differ in one letter.  
Graph has 2174 nodes with 8040 edges  
129 connected components  
Shortest path between warm and cold is  
warm  
ward  
word  
wold  
cold  
Shortest path between love and hate is  
love  
hove  
have  
hate  

## 4.
