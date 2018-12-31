## Welcome to Algorithms!

This page is intended to provide a list of top algorithms in computer science any programming students would look for.

### Algorithms List:
<button onclick="sortList()">Sort A-Z</button>

<ol id="id01">
  <li>Linear Search</li>
  <li>Binary search</li>
  <li>Insertion sort</li>
  <li>Selection sort</li>
  <li>Bubble sort</li>
  <li>Merge sort</li>
  <li>Quick sort</li>
  <li>Heap sort</li>
  <li>Inorder Tree Traversal</li>
  <li>Preorder Tree Traversal</li>
  <li>Postorder Tree Traversals</li>  
  <li>Kruskal's algorithm for finding a minimum spanning tree</li>
  <li>Dijkstra's algorithm for Single-Source Shortest Paths (finding the shortest paths between nodes in a graph)</li>
  <li>Floyd Warshall Algorithm for All-Pairs Shortest Paths (finding shortest paths in a weighted graph with positive or negative edge weights (but with no negative cycles))</li>
</ol>

<script>
function sortList() {
  var list, i, switching, b, shouldSwitch;
  list = document.getElementById("id01");
  switching = true;
  /* Make a loop that will continue until
  no switching has been done: */
  while (switching) {
    // Start by saying: no switching is done:
    switching = false;
    b = list.getElementsByTagName("LI");
    // Loop through all list items:
    for (i = 0; i < (b.length - 1); i++) {
      // Start by saying there should be no switching:
      shouldSwitch = false;
      /* Check if the next item should
      switch place with the current item: */
      if (b[i].innerHTML.toLowerCase() > b[i + 1].innerHTML.toLowerCase()) {
        /* If next item is alphabetically lower than current item,
        mark as a switch and break the loop: */
        shouldSwitch = true;
        break;
      }
    }
    if (shouldSwitch) {
      /* If a switch has been marked, make the switch
      and mark the switch as done: */
      b[i].parentNode.insertBefore(b[i + 1], b[i]);
      switching = true;
    }
  }
}
</script>
