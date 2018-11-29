<div id="demo">
<h2>The XMLHttpRequest Object</h2>
<button type="button" onclick="loadDoc()">Change Content</button>
</div>

<script>
function loadDoc() {
  var xhttp = new XMLHttpRequest();
  xhttp.onreadystatechange = function() {
    if (this.readyState == 4 && this.status == 200) {
      var str = this.responseText;
      //var res = str.split(" ");
     // alert(res);
      document.getElementById("demo").innerHTML = str;
      
      
      }
  };
  xhttp.open("GET", "test.txt", true);
  xhttp.send();
}
</script>
