# Applications
  <pre>
  <b><a href="https://github.com/teja963/DSA_All_Models/blob/master/Priority%20Queue/8.%20Task%20Scheduler.cpp">Task Scheduler</a></b>
     <img alt="task" width="600" height="300" src="https://github.com/teja963/DSA_All_Models/blob/master/Priority%20Queue/images/task.png">
      1. Find freq and push into priority queue
      eg:    n=2
            A B C D E
            9 7 5 3 2   push(8,6,4)    
            first we will take frst n elements(and store in array)and decrease each freq and push it to priority queue
            8 6 4 3 2   push(7,5,3)   
            7 5 3 3 2   push(6,4,2)
            6 4 3 2 2   push(5,4,2)
            5 4 2 2 2   push(4,3,1)
            4 3 2 2 1   push(3,2,1)
            3 2 2 1 1   push(2,1,1)
            2 1 1 1 1   push(1)
            1 1 1 0 0      
            
            ans += pq.empty ? tmp.size : n+1;
            
  **<b><a href="https://github.com/teja963/DSA_All_Models/blob/master/Priority%20Queue/9.%20Course%20Scheduler%203.cpp">Course Scheduler</a></b>**
       sorting is imp based on end time of course
       add all the duration
       while pq.top > course[i][0] // don't add that remove from pq
       
  </pre>
# Priority queue usage
  <pre>
  pq.push() - adds a copy of an element
  pq.emplace() - adds a new element
  Max:- priority_queue< int >pq;
        priority_queue< pair< int,int >>pq;
        priority_queue< pair< int,pair< int,int >>>pq;
  Min:- priority_queue< int,vector< int>,greater< int >>pq;
  </pre>
  
# Multimap
  <pre>
  multimap< data type, data type>m;  //by default asc order
  multimap< data type, data type, greater< data type>>m; //sort according to datatype in greater
  Multimap is similar to map with an addition that multiple elements can have same keys. Also, it is NOT required that
  the key value  and mapped value pair has to be unique in this case. One important thing to note about multimap is that
  multimap keeps all the keys in sorted order always
  </pre>
