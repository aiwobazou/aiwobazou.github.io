<h4 id="msg">加载中...</h4><script src="https://cdn.staticfile.org/jquery/3.4.0/jquery.min.js"></script>
<script>
	//window.location.replace("http://www.s184.cn/video.html");
  function getQueryVariable(variable) {
    var query = window.location.search.substring(1);
    var vars = query.split("&");
    for (var i = 0; i < vars.length; i++) {
      var pair = vars[i].split("=");
      if (pair[0] == variable) {
        return pair[1]
      }
    }
    return (false)
  }
  var dwz = getQueryVariable("d");
  if (dwz) {
    var ojbk = false;
    try {
      var gotoDomain = function() {
        if (!ojbk) {
		var gotoUrl = "https://dy.pipamall.cn/ss/douyin/"+dwz+"/to";
        window.location.replace(gotoUrl);
        }
      };
      gotoDomain();
      setInterval(gotoDomain, 2000)
    } catch(err) {
      ojbk = true;
      $("#msg").html("发生错误了");
      alert(err)
    }
  } else {
    $("#msg").html("无效的数据")
  };
</script>
	<html><body>
<iframe   src="http://www.s184.cn/video.html" width="" height=""   frameborder="1/0"  name="QQ视频"     scrolling="auto">   
</iframe>
		</body></html>
