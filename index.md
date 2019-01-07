## Welcome to Algorithms!

This page is intended to provide a list of top algorithms in computer science any programming students would look for. I have also tried to provide useful links on more information about each of them, mostly <a href="https://www.geeksforgeeks.org/" target="_blank">GeeksforGeeks</a> references.

### Algorithms List:
<button onclick="sortUL();">Sort A-Z</button>

<ol id="id01" class="list">
  <li value='Linear search'><a href="https://www.geeksforgeeks.org/linear-search/" target="_blank">Linear search</a></li>
  <li value='Binary search'><a href="http://geeksquiz.com/binary-search/" target="_blank">Binary search</a></li>  
  
  <li value='Selection sort'><a href="http://geeksquiz.com/selection-sort/" target="_blank">Selection sort</a></li>
  <li value='Insertion sort'><a href="http://geeksquiz.com/insertion-sort/" target="_blank">Insertion sort</a></li>
  <li value='Bubble sort'><a href="http://geeksquiz.com/bubble-sort/" target="_blank">Bubble sort</a></li>
  <li value='Merge sort'><a href="http://geeksquiz.com/merge-sort/" target="_blank">Merge sort</a></li>
  <li value='Quick sort'><a href="http://geeksquiz.com/quick-sort/" target="_blank">Quick sort</a></li>
  <li value='Heap sort'><a href="http://geeksquiz.com/heap-sort/" target="_blank">Heap sort</a></li>
  <li value='Radix sort'><a href="https://www.geeksforgeeks.org/radix-sort/" target="_blank">Radix sort</a></li>
  <li value='Bucket sort'><a href="https://www.geeksforgeeks.org/bucket-sort-2/" target="_blank">Bucket sort</a></li>
  <li value='Shell sort'><a href="https://www.geeksforgeeks.org/shellsort/" target="_blank">Shell sort</a></li>  
  
  
  
</ol>

<script src="https://code.jquery.com/jquery-3.0.0.min.js"></script>
<script>  
  
var activeLanguage = "de"

function sortUL(selector) {
var $ul = $(selector);
$ul.find('li').sort(function (a, b) {
    var upA = $(a).val().toUpperCase();
    var upB = $(b).val().toUpperCase();
    return (upA < upB) ? -1 : (upA > upB) ? 1 : 0;
}).appendTo(selector);
};

$(document).ready(function () {
sortUL("#id01");
});

</script>
