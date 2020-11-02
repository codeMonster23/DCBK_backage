$(function(){
    $("table").each(function(){
        $(this).find("tr:even").css("background-color","#f5f5f5");
    })

    $(".checkbox-box .checkbox,.checkbox-label").click(function(){
        $(this).parent(".checkbox-box").toggleClass('active').siblings().removeClass('active');
    });

    $(".sidebar .nav-item").click(function(){
        $(this).toggleClass('cur').siblings().removeClass('cur');
    });

    $(".sidebar .menu-level2").click(function(e){
        $(this).addClass('active').siblings().removeClass('active');
        e.stopPropagation();
    });
    // 左右高度自适应
    calc()
    function calc(){
        var sHeight=$('.sidebar').height();
        var cHeight=$('.content').height();
        var arrHeight=[sHeight,cHeight];
       var maxHeight=Math.max.apply(null,arrHeight);	
        $('.sidebar').height(maxHeight);
        $('.content').height(maxHeight);
    }
    $(window).resize(function(){
        calc()
    });

	 
})