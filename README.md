<div id="container" style="width:100%; height:300px; background:#eee; display:flex; align-items:center; justify-content:center;">
  <p>Your Content Here</p>
  <button onclick="goFullscreen()">Fullscreen</button>
</div>

<script>
  function goFullscreen() {
    var element = document.getElementById("container");
    if (element.requestFullscreen) {
      element.requestFullscreen();
    } else if (element.webkitRequestFullscreen) {
      element.webkitRequestFullscreen();
    } else if (element.msRequestFullscreen) {
      element.msRequestFullscreen();
    }
  }
</script>
