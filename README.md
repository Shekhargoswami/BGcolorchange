# BGcolorchange

<html>
    <head>
        <title>Document</title>
        <style>
            body,html{
              background-color: rgb(119, 102, 102);
                margin: 0%;
                padding: 0%;
                height: 100%;
            }
            .container{
                display: flex;
                height: 100%;
                justify-content: center;
                align-items: center;
            }
            .box{
                text-align: center;
            }
            button{
                background-color: black;
                color: aliceblue;
                padding: 50px;
                border-radius: 50px;
                font-size: larger;
            }
        </style>
    </head>
    <body>
        <div class="container">
            <div class="box">
                <button onclick="clr()">mera desh badal rha hai but yha color badlega</button>
            </div>
        </div>
        <script>
                let color =['red','blue','black'];
                let index=0;

            function clr(){

                document.body.style.backgroundColor= color[index];
                index=(index+1) % color.length;

            }

        </script>
    </body>
</html>
