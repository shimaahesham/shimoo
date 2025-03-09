(function ($) {
 "use strict";
    
/*-- Intelligent-header
------------------------------ */ 
    var myElement = document.querySelector(".intelligent-header");
    var headroom  = new Headroom(myElement);
    headroom.init();  

    
    
    
/*- smoth-scroll js
-------------------------*/ 
$('.smooth-scroll a,.hire-me').on("click", function (e) {
    var anchor = $(this);
    $('html, body').stop().animate({
        scrollTop: $(anchor.attr('href')).offset().top - 40
    }, 1000);
    e.preventDefault();
});  
    
/*- Extra js 
---------------------*/	    
$(document).on('click', '.navbar-collapse.in', function (e) {
    if ($(e.target).is('a') && $(e.target).attr('class') != 'dropdown-toggle') {
        $(this).collapse('hide');
    }
});
$('body').scrollspy({
    target: '.navbar-collapse',
    offset: 200
});  
    
    
 /*-- Isotope active JS
-----------------------------*/
$('.grid').imagesLoaded( function() {
	
    // filter items on button click
    $('.portfolio-menu').on( 'click', 'button', function() {
      var filterValue = $(this).attr('data-filter');
      $grid.isotope({ filter: filterValue });
    });	

    // init Isotope
    var $grid = $('.grid').isotope({
      itemSelector: '.grid-item',
      percentPosition: true,
      masonry: {
      columnWidth: '.grid-item',
      }
    });

});
$('.portfolio-menu button').on('click', function(event) {
	$(this).siblings('.active').removeClass('active');
	$(this).addClass('active');
	event.preventDefault();
});   
    
/*--- Magnific Popup
------------------------*/
    $('.img-poppu').magnificPopup({
        type: 'image',
        gallery:{
        enabled:true
    }
});    
 /* magnificPopup video popup */
    $('.video-play').magnificPopup({
        type: 'iframe'
    });
 
  
    
/*-- owl active
------------------------------ */    
$('.testimonel-carousel').owlCarousel({
    loop:true,
    items:1,
    autoplay: false,
    dots:true,
    responsive:{
        0:{items:1},
        600:{items:1},
        1000:{items:1}
    }
});

    
/*-- CounterUp
------------------------------*/
    
$('.counter').counterUp({
    delay: 10,
    time: 1000
});
    
    
    
    
    
    
    
    
    
    
    
 
})(jQuery); 