<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="project.css">
    <title>my project</title>
</head>
<body>
    <p1 id="obb">i not rak namwan</p1>
    <button class="pp" type="button" onclick="Myfunction()";>Changne Text</button>
    <button class="gg" type="button" onclick="youfunction()";>Next Text</button>
    <button class="dd" type="button" onclick="ourfunction()";>Defult Text</button>

    <script>
        function Myfunction() {
            document.getElementById("obb").innerHTML = '<span id="ogg">haha gu gohok</span>';
        }

        alert("Welcome To My website");

        console.log(document.getElementById("obb"));

        function youfunction() {
            document.getElementById("ogg").innerHTML = "หยอกเล่นๆ";
        }

        function ourfunction() {
            document.getElementById("ogg").innerHTML = '<span id="odd">mai re hai mueng rok</span>';
        }
        
    </script> 

</body>
</html>
