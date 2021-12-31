# Loading-Screen

- Preview

![preview](loading.gif)


- Adjustment
```
    <!-- Loading Script -->
<script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>
  <script type="text/javascript">
	  function counter(){
		  var count = setInterval(function(){
			  var c = parseInt($('.counter').text());
			  $('.counter').text((++c).toString());
			  if (c == 100){
				  clearInterval(count);
				  $('.counter').addClass('hide')
				  $('.preloader').addClass('active')
			  }
        // 1-100, 1 superfast countdown 50 mild countdown and so on, the higher number the slower.
		  },30)
	  }
	  counter()
</script>
```
