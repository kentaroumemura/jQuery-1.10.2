# jQuery-1.10.
newquery <スクリプト>
  $(function () {
    var headerHight = 60; //Specify the height of the header and assign it to headerHeight
    $('a[href^="#"]').click(function () {　//Event handling on click of anchor link
      var href = $(this).attr("href");　//Get anchor link attributes
      var target = $(href == "#" || href == "" ? "html" : href);　//"html" if href value is "#" or "", otherwise assign href to target
      var position = target.offset().top - headerHight;　//Distance from top of screen to target element - assign header height to position
      $("html, body").animate({ scrollTop: position }, 200, "swing");　// Move slowly in 0.5 seconds to the acquired position
      return false;　//Cancel the href link of the a tag after executing the click event
    });
  });
</script>
Dear Developers, Thank you for visiting.

I am unfamiliar with HTML and English, but I will do my best, so please help me.
