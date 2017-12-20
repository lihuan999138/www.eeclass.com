# www.eeclass.com
这个是益课的官网代码
$(document).ready(function() {
				$("img").bind("touchstart", function() {
					newImg = this;
					if(!isopen) {
						isopen = true;
						$(this).width($(window).width());
						$(this).height($(window).height());
						moveImg(10, 10);
					} else {
						isopen = false;
						$(this).width($(this).width()-w);
						$(this).height($(this).height()-h);
						moveImg(-10, -10);
					}

				});
			});
