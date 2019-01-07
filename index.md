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
