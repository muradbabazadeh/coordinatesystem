<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    <script>
        var myCoordinate={x:450,y:333}
         var coordinates = [
        {x:45,y:69},
        {x:23,y:90},
        {x:126,y:456},
        {x:450,y:1222},
        {x:12,y:345},
        {x:42,y:691},
        {x:203,y:900},
        {x:106,y:4561},
        {x:410,y:1222},
        {x:56,y:3457}
    ] ;
        var minDistance= Math.sqrt(Math.pow(myCoordinate.x-coordinates[0].x,2)+
        Math.pow(myCoordinate.y-coordinates[0].y,2));

    for (var i=1;i < coordinates.length; i++) {
            var taxiCoordinate=coordinates[i];
        
        var distance= Math.sqrt(Math.pow(myCoordinate.x-taxiCoordinate.x,2)+
        Math.pow(myCoordinate.y-taxiCoordinate.y,2));

        console.log(distance)

        if(distance<minDistance){
            minDistance=distance

        }

    }
        alert(minDistance)


        

         



    
    
    </script>
    
</body>
</html>
