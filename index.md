## Welcome to Algorithms!

This page is intended to provide a list of top algorithms in computer science any programming students would look for. I have also tried to provide useful links on more information about each of them, mostly <a href="https://www.geeksforgeeks.org/" target="_blank">GeeksforGeeks</a> references.

### Algorithms List:
<button onclick="sortList(document.getElementsByClassName('list')[0]);">Sort A-Z</button>

<ol id="id01" class="list">
  <li id='Linear search'><a href="https://www.geeksforgeeks.org/linear-search/" target="_blank">Linear search</a></li>
  <li id='Binary search'><a href="http://geeksquiz.com/binary-search/" target="_blank">Binary search</a></li>  
  
  <li id='Selection sort'><a href="http://geeksquiz.com/selection-sort/" target="_blank">Selection sort</a></li>
  <li id='Insertion sort'><a href="http://geeksquiz.com/insertion-sort/" target="_blank">Insertion sort</a></li>
  <li id='Bubble sort'><a href="http://geeksquiz.com/bubble-sort/" target="_blank">Bubble sort</a></li>
  <li id='Merge sort'><a href="http://geeksquiz.com/merge-sort/" target="_blank">Merge sort</a></li>
  <li id='Quick sort'><a href="http://geeksquiz.com/quick-sort/" target="_blank">Quick sort</a></li>
  <li id='Heap sort'><a href="http://geeksquiz.com/heap-sort/" target="_blank">Heap sort</a></li>
  <li id='Radix sort'><a href="https://www.geeksforgeeks.org/radix-sort/" target="_blank">Radix sort</a></li>
  <li id='Bucket sort'><a href="https://www.geeksforgeeks.org/bucket-sort-2/" target="_blank">Bucket sort</a></li>
  <li id='Shell sort'><a href="https://www.geeksforgeeks.org/shellsort/" target="_blank">Shell sort</a></li>  
  
  <li id='Inorder Tree Traversal'><a href="https://www.geeksforgeeks.org/tree-traversals-inorder-preorder-and-postorder/" target="_blank">Inorder Tree Traversal</a></li>
  <li id='Preorder Tree Traversal'><a href="https://www.geeksforgeeks.org/tree-traversals-inorder-preorder-and-postorder/" target="_blank">Preorder Tree Traversal</a></li>
  <li id='Postorder Tree Traversal'><a href="https://www.geeksforgeeks.org/tree-traversals-inorder-preorder-and-postorder/" target="_blank">Postorder Tree Traversal</a></li>  
  
   <li id='Breadth First Search (BFS for a Graph)'><a href="https://www.geeksforgeeks.org/breadth-first-search-or-bfs-for-a-graph/" target="_blank">Breadth First Search (BFS for a Graph)</a></li>
   <li id='Depth First Search (DFS for a Graph)'><a href="https://www.geeksforgeeks.org/depth-first-search-or-dfs-for-a-graph/" target="_blank">Depth First Search (DFS for a Graph)</a></li>   
   
   <li id='Prim’s algorithm for Minimum Spanning Tree'><a href="https://www.geeksforgeeks.org/greedy-algorithms-set-5-prims-minimum-spanning-tree-mst-2/" target="_blank">Prim’s algorithm for Minimum Spanning Tree</a></li>
   <li id='Kruskal's algorithm for Minimum Spanning Tree'><a href="https://www.geeksforgeeks.org/kruskals-minimum-spanning-tree-algorithm-greedy-algo-2/" target="_blank">Kruskal's algorithm for Minimum Spanning Tree</a></li>   
   
   <li id='Dijkstra's algorithm for Shortest Path'><a href="https://www.geeksforgeeks.org/dijkstras-shortest-path-algorithm-greedy-algo-7/" target="_blank">Dijkstra's algorithm for Shortest Path</a></li>
  <li id='Floyd Warshall algorithm for All Pairs Shortest Path'><a href="https://www.geeksforgeeks.org/floyd-warshall-algorithm-dp-16/" target="_blank">Floyd Warshall algorithm for All Pairs Shortest Path</a></li>
  <li id='Dijkstra's algorithm for Adjacency List Representation'><a href="https://www.geeksforgeeks.org/dijkstras-algorithm-for-adjacency-list-representation-greedy-algo-8/" target="_blank">Dijkstra's algorithm for Adjacency List Representation</a></li>
  <li id='Dijkstra's algorithm for Adjacency Matrix Representation'><a href="https://www.geeksforgeeks.org/prims-minimum-spanning-tree-mst-greedy-algo-5/" target="_blank">Dijkstra's algorithm for Adjacency Matrix Representation</a></li>  
  
  
   <li id='Travelling Salesman Problem using Dynamic Programming'><a href="https://www.geeksforgeeks.org/travelling-salesman-problem-set-1/" target="_blank">Travelling Salesman Problem using Dynamic Programming</a></li>
  <li id='Travelling Salesman Problem using MST'><a href="https://www.geeksforgeeks.org/travelling-salesman-problem-set-2-approximate-using-mst/" target="_blank">Travelling Salesman Problem using MST</a></li>
  
</ol>

<script>
// Reference: this script is from https://stackoverflow.com/questions/8837191/sort-an-html-list-with-javascript
function sortList(ul){  
    var new_ul = ul.cloneNode(false);

    // Add all lis to an array
    var lis = [];
    for(var i = ul.childNodes.length; i--;){
        if(ul.childNodes[i].nodeName === 'LI')
            lis.push(ul.childNodes[i]);
    }

    // Sort the lis in descending order
    lis.sort(function(a, b){
       return parseInt(b.childNodes[0].data , 10) - 
              parseInt(a.childNodes[0].data , 10);
    });

    // Add them into the ul in order
    for(var i = 0; i < lis.length; i++)
        new_ul.appendChild(lis[i]);
    ul.parentNode.replaceChild(new_ul, ul);
}
</script>
