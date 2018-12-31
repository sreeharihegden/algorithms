## Welcome to Algorithms!

This page is intended to provide a list of top algorithms in computer science any programming students would look for.

### Algorithms List:
<button onclick="sortList()">Sort A-Z</button>

<ol id="id01">
  <li><a href="https://www.geeksforgeeks.org/linear-search/">Linear Search</a></li>
  <li><a href="">Binary search</a></li>
  <li><a href="">Insertion sort</a></li>
  <li><a href="">Selection sort</a></li>
  <li><a href="">Bubble sort</a></li>
  <li><a href="">Merge sort</a></li>
  <li><a href="">Quick sort</a></li>
  <li><a href="">Heap sort</a></li>
  <li><a href="">Inorder Tree Traversal</a></li>
  <li><a href="">Preorder Tree Traversal</a></li>
  <li><a href="">Postorder Tree Traversal</a></li>  
  <li><a href="">Kruskal's algorithm</a></li>
  <li><a href="">Dijkstra's algorithm</a></li>
  <li><a href="">Floyd Warshall algorithm</a></li>
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
