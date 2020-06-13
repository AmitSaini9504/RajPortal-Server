# RajPortal-Server
This is only a link based site 
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <style>
        body {
            background-color: rgb(153, 0, 255);
            background-size: cover;
            background-blend-mode: hard-light;
            background-attachment: fixed;
        }
        /* navigation Bar */
        
        .navbar1 {
            width: 100%;
            background-color: #555;
            overflow: auto;
        }
        
        .navbar a {
            float: left;
            padding: 12px;
            color: white;
            text-decoration: none;
            font-size: 17px;
        }
        
        .navbar a:hover {
            background-color: black;
        }
        
        .active {
            background-color: green;
        }
        
        @media screen and (max-width: 500px) {
            .navbar a {
                float: none;
                display: block;
            }
        }
        
        .navbar {
            width: 100%;
            background-color: black;
            overflow: auto;
        }
        
        .navbar a {
            float: left;
            padding: 12px;
            color: white;
            text-decoration: none;
            font-size: 17px;
        }
        
        .navbar a:hover {
            background-color: #000;
        }
        
        .active {
            background-color: green;
        }
        
        @media screen and (max-width: 500px) {
            .navbar a {
                float: none;
                display: block;
            }
        }
        
        {
            font-family: 'Lato', sans-serif;
        }
        
        .overlay {
            height: 100%;
            width: 0;
            position: fixed;
            z-index: 1;
            top: 0;
            left: 0;
            background-color: rgb(0, 0, 0);
            background-color: rgba(0, 0, 0, 0.9);
            overflow-x: hidden;
            transition: 0.5s;
        }
        
        .overlay-content {
            position: relative;
            top: 25%;
            width: 100%;
            text-align: center;
            margin-top: 30px;
        }
        
        .overlay a {
            padding: 8px;
            text-decoration: none;
            font-size: 36px;
            color: #818181;
            display: block;
            transition: 0.3s;
        }
        
        .overlay a:hover,
        .overlay a:focus {
            color: #f1f1f1;
        }
        
        .overlay .closebtn {
            position: absolute;
            top: 20px;
            right: 45px;
            font-size: 60px;
        }
        
        @media screen and (max-height: 450px) {
            .overlay a {
                font-size: 20px
            }
            .overlay .closebtn {
                font-size: 40px;
                top: 15px;
                right: 35px;
            }
        }
        
        .container {
            display: grid;
            grid-template-columns: 30% 30% 30%;
            justify-content: space-evenly;
            grid-gap: 10px;
            width: 1300px;
            height: 400px;
            background-color: transparent;
            padding: 10px;
        }
        
        .container div {
            border: 1px solid black;
            background-color: transparent;
        }
        
        .item1 {
            /* grid-row-start:1;
            grid-row-end:3;
            grid-column-start:1;
            grid-column-end:3; */
            /* grid-column: 1/3;
            grid-row:1/3 */
            grid-area: 1/1/3/3;
        }
        
        * {
            box-sizing: border-box;
        }
        
        .checked {
            color: orange;
        }
        
        body {
            margin: 0;
            font-family: Arial;
            font-size: 17px;
        }
        
        #myVideo {
            position: fixed;
            right: 0;
            bottom: 0;
            min-width: 100%;
            min-height: 100%;
        }
        
        .content {
            position: fixed;
            bottom: 0;
            background: rgba(0, 0, 0, 0.5);
            color: #f1f1f1;
            width: 100%;
            padding: 20px;
        }
        
        #myBtn {
            width: 200px;
            font-size: 18px;
            padding: 10px;
            border: none;
            background: #000;
            color: #fff;
            cursor: pointer;
        }
        
        #myBtn:hover {
            background: #ddd;
            color: black;
        }
        
        .loader {
            border: 16px solid #f3f3f3;
            border-radius: 50%;
            border-top: 16px solid #3498db;
            width: 120px;
            height: 120px;
            -webkit-animation: spin 2s linear infinite;
            /* Safari */
            animation: spin 3s linear infinite;
        }
        /* Safari */
        
        @-webkit-keyframes spin {
            0% {
                -webkit-transform: rotate(0deg);
            }
            100% {
                -webkit-transform: rotate(360deg);
            }
        }
        
        @keyframes spin {
            0% {
                transform: rotate(0deg);
            }
            100% {
                transform: rotate(360deg);
            }
        }
    </style>
</head>

<body>


    <!-- Navigation Bar -->
    <div class="navbar 1">
        <a class="active" href="https://jansoochna.rajasthan.gov.in/index.php/kiosks-main/"><i class="fa fa-fw fa-home"></i>ई मित्र</a>
        <a href="https://jansoochna.rajasthan.gov.in/index.php/employment-main/"><i class="fa fa-fw fa-globe"></i>रोजगार</a>
        <a href="https://jansoochna.rajasthan.gov.in/index.php/sampark-main/"><i class="fa fa-fw fa-envelope"></i> संपर्क</a>
        <a href="https://jansoochna.rajasthan.gov.in/index.php/e-panchayat-main/"><i class="fa fa-fw fa-user"></i>ई- पंचायत</a>
        <a href="https://jansoochna.rajasthan.gov.in/index.php/rti-main/"><i class="fa fa-fw fa-search"></i>सूचना का अधिकार</a>
        <a href=""></a>
        <a href=""></a>
        <a href=""></a>
        <a href=""></a>


        <a class="active" href="#"><i class="fa fa-fw fa-home"></i> RajPortal-></a>
        <a href="https://sso.rajasthan.gov.in/register"><i class="fa fa-fw fa-user"></i>Sign Up</a>
        <a href="https://sso.rajasthan.gov.in/dashboard"><i class="fa fa-fw fa-user"></i> Sign in</a>

        <a href="https://searchsecurity.techtarget.com/definition/single-sign-on"><i class="fa fa-fw fa-search"></i>Search</a>


    </div>


    <div>
        <!-- <p style="color: White; font-size:30px;margin-top: 0px;"  <h1>Government Of Rajasthan</h1> -->
    </div>


    <!-- Inside Icon -->
    <div id="myNav" class="overlay">
        <a href="javascript:void(0)" class="closebtn" onclick="closeNav()">&times;</a>
        <div class="overlay-content">

            <a href="http://sampark.rajasthan.gov.in"><i class="fa fa-fw fa-feedback"></i>About</a>
            <a href="https://docs.google.com/forms/d/e/1FAIpQLSeIbxFTioasoF2gkV0ZC0-TGrHD-L8FpT7owXS73y5IHHp9UA/viewform">Feedback</a>
            <a href="https://docs.google.com/forms/d/e/1FAIpQLSeIbxFTioasoF2gkV0ZC0-TGrHD-L8FpT7owXS73y5IHHp9UA/viewform">Suggestion</a>
            <a href="
          https://docs.google.com/forms/d/e/1FAIpQLSfi8V4DQYnesJi74B1jwmBTbupthXbSDzKOn3VN6yZo9V85wQ/viewform">Contact Me</a>
        </div>
    </div>


    <span style="font-size:30px;cursor:pointer" onclick="openNav()">&#9776; open</span>

    <script>
        function openNav() {
            document.getElementById("myNav").style.width = "100%";
        }

        function closeNav() {
            document.getElementById("myNav").style.width = "0%";
        }
    </script>



    </div>
    <div>

        <!-- Rajasthan Map -->

        <div class="container">
            <div class="item1">
                <form action="https://www.google.co.in/maps/place/Rajasthan/@26.5674306,69.3774632,6z/data=!3m1!4b1!4m5!3m4!1s0x396a3efaf7e30e37:0xb52b9b4506c088e5!8m2!3d27.0238036!4d74.2179326">
                    <style></style>
                    <button type="submit" style="padding: 1px;width: 250px;font-size: 30px;background-color: transparent;">Rajasthan Map</button></form>




                <form action="https://www.holidify.com/state/rajasthan/map-view.html">
                    <style></style>
                    <button type="submit" style="padding: 1px;width: 250px;font-size: 30px;background-color: transparent;margin-top: 10px;">Tourist Map</form>
         
                <form action="https://www.tripadvisor.in/Attractions-g297665-Activities-Rajasthan.html">
                    <style></style>
                    <button type="submit" style="padding: 1px;width: 250px;font-size: 30px;background-color: transparent;margin-top: 10px;">Top 10 Palace</form>
                     
                    


          </div>
          
          
          
          
          <div class="item2">
            <img src="jaipur.jpg" height="220px;" width="390px" alt="">
        </div>
        
        <div class="item3">
            <img src="Jaipur1.jpg" height="220px;" width="390px" alt="">
        </div>
        
        
        
        
        
        
       
    </div>
   
    
    <div>
    <center> <p style="color: black;font-size: 30px;margin-top: 70px;">राजस्थान राज्य भारत के उत्तर-पश्चिम में स्थित सबसे खूबसूरत राज्यों में गिना जाता है। राजस्थान स्टेट लगभग 342,239 वर्ग किलोमीटर के क्षेत्र में फैला हुआ हैं और भारत का सबसे बड़ा राज्य है। राजस्थान की भूमि राजा-महाराजाओं की भूमि होने के साथ-साथ बहुत ही लोकप्रिय और ऐतिहासिक स्थान माना जाता हैं। राजस्थान में कई प्राचीन किले, स्मारक, प्रसिद्ध भवन राजस्थान की प्रसिद्धि के प्रमुख कारण है।

        राजस्थान अपनी रंगीन संस्कृति, खूबसूरत पहनावा, दिलचस्प कलाकृति और यहाँ के प्रसिद्ध व्यंजनों के लिए दुनियाभर में प्रसिद्ध हैं। राजस्थान में विशाल थार रेगिस्तान स्थित है जोकि भारत का सबसे बड़ा रेगिस्तान है और दुनिया के सबसे बड़े उष्णकटिबंधीय रेगिस्तानों में यह 18 वे नंबर पर है।
        
        </p></center>
        <h2>Star Rating</h2>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star checked"></span>
        <span class="fa fa-star"></span>
      

    </div>
    

      </div>
      <div> <h1 style="background-color:transparent">राजस्थान की राजधानी : -</h1></div>
      <div>
        <img src="jaipur.jpg" height="500px;" width="1250px"margin-left="100px;"  alt="">
      </div>
        <div>
            <center> <p style="color:black;font-size: 30px;margin-top: 70px;">
            जयपुर शहर(पिंक सिटी) अपनी शाही किले, महलों, प्राचीन इमारतों और दुनिया के कई आकर्षक होटलों की वजह से राज्य का प्रमुख पर्यटन शहर है। जयपुर में स्थित कई विशाल किलों और महलों को देखने के लिए दुनिया भारत से यहां पर्यटक आते हैं। जयपुर की यात्रा के दौरान आप नीचे दिए गए पर्यटन स्थलों की सैर कर सकते हैं।

             बिरला मंदिर
             राम निवास उद्यान
             खाटू श्याम जी मंदिर
             जयगढ़ किला
             आमेर का किला
             सिटी पैलेस
             जल महल
             नाहरगढ़ किला
             जंतर मंतर
             हवा महल
             गलताजी मंदिर
             चोखी ढाणी
</p></center>
        </div>
        
         <center><div class="loader"></div></center>
         <center><h2>Loading...</h2> </center>

</body>
</html>
