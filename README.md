#Greetr JavaScript Library#

**Greetr** is a simple reusable library allows developers to log greetings to users. 

This is my first JavaScript library created, I hope you enjoy!

##Version##
0.1.0

##Usage##
    // gets a new object (the architecture allows us to not have to use the 'new' keyword here)
	var g = G$('John', 'Doe');

	// use our chainable methods
	g.greet().setLang('es').greet(true).log();

	// let's use our object on the click of the login button
	$('#login').click(function() {
   
    	// create a new 'Greetr' object (let's pretend we know the name from the login)
    	var loginGrtr = G$('John', 'Doe');
    
     	// hide the login on the screen
    	$('#logindiv').hide();
    
    	 // fire off an HTML greeting, passing the '#greeting' as the selector and the chosen language, and log the welcome as well
    	loginGrtr.setLang($('#lang').val()).HTMLGreeting('#greeting', true).log();
    
	});


##License##
MIT License



