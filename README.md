
<html>
    <head>
        
        <link rel="stylesheet" href="style.css">
    </head>
    
    <body>

        <!-- <script src = "style.css"> </script> -->
        <h2>
            JackNC
        </h2>
        <p>
                go from smol to swoll
        </p>
    
        <h1>YEET</h1>
        <input id="getJacked" type="button" value= "get jacked">
        <p> 

        </p>
        <img src = "output-onlinepngtools.png" alt = "jack" id = "jack">
        
        <!-- <button type = "button" onclick = "enlarge()"> get jacked</button> -->
        
        <script> 
        document.getElementById("getJacked").onclick = function () {
            var elem = document.getElementById("jack");
            var heightProp = window.getComputedStyle(elem, null).getPropertyValue("height");
            var widthProp = window.getComputedStyle(elem, null).getPropertyValue("width");
            // console.log(theCSSprop);
            var jackHeight = Number(heightProp.substring(0,heightProp.length-2));
            jackHeight+= 20;
            var jackWidth = Number(widthProp.substring(0, widthProp.length -2 ));
            jackWidth += 20;
            console.log(jackHeight);
            console.log(jackWidth);
        
            document.getElementById('jack').style.height = jackHeight.toString() + "px";
            document.getElementById('jack').style.width = jackWidth.toString() + "px";
        }
       
        </script>
        
        
    </body>
</html>
