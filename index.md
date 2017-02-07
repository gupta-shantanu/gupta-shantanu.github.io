---
layout: default
title: Welcome
---

<div class="posts">
<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
<script src="resources/typed.js" type="text/javascript"></script>
    <script>
    $(function(){

        $("#typed").typed({
			strings: ['<h1>shantanu</h1>'],
            stringsElement: $('#typed-strings'),
            typeSpeed: 20,
            backDelay: 500,
            loop: true,
            contentType: 'html', // or text
            // defaults to false for infinite loop
            loopCount: false,
            callback: function(){ foo(); },
            resetCallback: function() { newTyped(); }
        });

        $(".reset").click(function(){
            $("#typed").typed('reset');
        });

    });

    function newTyped(){ /* A new typed object */ }

    function foo(){ console.log("Callback"); }

    </script>
    <link href="main.css" rel="stylesheet"/>
    <style>
        /* code for animated blinking cursor */
        .typed-cursor{
            opacity: 1;
            font-weight: 100;
            -webkit-animation: blink 0.7s infinite;
            -moz-animation: blink 0.7s infinite;
            -ms-animation: blink 0.7s infinite;
            -o-animation: blink 0.7s infinite;
            animation: blink 0.7s infinite;
        }
        @-keyframes blink{
            0% { opacity:1; }
            50% { opacity:0; }
            100% { opacity:1; }
        }
        @-webkit-keyframes blink{
            0% { opacity:1; }
            50% { opacity:0; }
            100% { opacity:1; }
        }
        @-moz-keyframes blink{
            0% { opacity:1; }
            50% { opacity:0; }
            100% { opacity:1; }
        }
        @-ms-keyframes blink{
            0% { opacity:1; }
            50% { opacity:0; }
            100% { opacity:1; }
        }
        @-o-keyframes blink{
            0% { opacity:1; }
            50% { opacity:0; }
            100% { opacity:1; }
        }
		.typed-strings{

		font-style: italic;
		}

    </style>


    <div class="wrap highlight">
        <div style="font-size: 30px; width: 100%;" class="type-wrap">
		
            <div id="typed-strings">
                <p>Hi!</p>
                <p>I am Shantanu...</p>
                <p>And this is my website...</p>
                <p>It's not complete yet..!!!</p>
				<p>But feel free to roam around :smile: :smile: :smile:  </p>
            </div>
			
            <span id="typed" style="white-space:pre;"></span>
        </div>
	</div>
</div>