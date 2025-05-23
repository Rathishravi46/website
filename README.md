# Ex.07 Restaurant Website
# Date: 10.05.2025
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:
```
home.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>restarent page</title>
    <link rel="stylesheet" href="res.css">
</head>
<header>
   <div class="name">
     <li class="name1">🍔MR.</li> 
    <li class="name2">Honey🍯</li><br>
</div>
</header>

<body>
    <div class="menu">
        <ul>
            <li><a href="res.html">HOME</a></li>
            <li><a href="menu.html">MENU</a></li>
            <li><a href="admin.html">ADMINISTRATION</a></li>
            <li><a href="contect.html">CONTACT US</a></li>
        </ul> 
    </div>
    <div class="food">
        <center>
         <table>
            <tr>
                <td><p>OUR RESTARENT IS UNIQUE</p><br><img src="cooking.jpeg"><br>our restarent is very spcial in burger.<br>we make burger in pure attapowder<br>we useing only contery chicken.<br>   <br>   <br> <br></td>
                <td><center><p>FACILITIES</center><br></p><img src="restarent.jpeg"><br>we have luxery outlook.we<br> are NO.1 in india.we have<br> party hall also and we provide<br>inernational drinks and we gave<br>our own brand jigarthanda also<br>     <br>  <br></td>
                <td><p>WORKING DAYS</p><br><img src="chef.jpeg"><center>our restarent working time</center><br>MONDAY TO SUNDAY<BR>10:00AM-11:00PM<BR>MONDAY IT'S OUR OFFER DAY<BR> <a href="menu.html">GO TO MENU AND PLASE ORDER</a> </td>
            </tr>
         </table>
        </center>
    </div>
    <div class="offer">
      <center>
        <table>
            <tr>
          <td>
            <p class="title">OUR FRIDAY FRY CHICKEN OFFER IS GOING ON....</p><BR>
                <P class="title1">YOU AER A FIRST COSTOMER GET YOUR FLAT 50% OFFER.we provide many offer like buy one get one offer in 🍔burgur and 🍕pizza.we contect some contest and we provide unlimited food for winers.if you order through our web site and get extra offers.</P>
        </td>
           </tr>
        </table>
    </center> 
    </div>
    <footer>
       <hr style="color: rgb(91, 38, 38);"> 
       <center>
      <p class="author">DISIGNED AND DEVLOPED BY </p><P class="name">CHANDRU.K</P>
    </center>
    </footer>
</body>
</html>

home.css

header{
    ;
}
.name{
    margin-top: 13px;
    margin-left: 45%;
}
.name1{
    font-family: 'Times New Roman', Times, serif;
    font-weight: bolder;
    font-size: 39px;
    color: rgba(215, 49, 7, 0.803);
    
}
.name2{
    font-family: cursive;
    font-size: 37px;
    color: rgba(222, 215, 13, 0.97);
    font-weight: bold;
    
}
li{
    float: left;
    list-style: none;
}

ul li a{
display: flex;
padding-left: 50px;
padding-right: 50px;
color: aquamarine;
}
ul li a:hover{
    color: aliceblue;
    cursor: pointer;
}
body{
    background-image: url(bg.jpg);
    background-size: cover;
    background-blend-mode: color-burn;
}
.menu{
    margin-top: 60px;
    margin-left: 330px;
    border-width: 30px;
    border-color: aquamarine;
    background-color: rgb(84, 92, 92);
    display: inline-flex;
    padding-left: 30px;
    padding-right: 30px;
    color: rgb(176, 129, 100);
    border-radius:  25px;
}
.food{
    margin-top: 90px;
    padding: 14px;
}
td{
padding: 20px;
background-color: bisque;
border-width: px;
border-radius: 18px;
white-space: 5px;
}
tr{
    padding: 5px;
}
p{
    font-weight: bolder;
    align-items: center;
}
img{
    align-items: center;
}  
.offer table tr{
    width: 70%;
}
.offer td{
    background-image: url(footer.jpeg);
    width: 900px;
    height: 150px;
    align-items: center;
    border-color: rgb(219, 8, 152);
    border-width: 5px;
    border-radius: 20px;
    border-style: double;
}
.offer .title{
    color: rgb(214, 210, 210);
    font-size:xx-large ;
    font-weight: bolder;
    font-family: 'Times New Roman', Times, serif;
    ;
}
.offer .title1{
    color: aliceblue;
    font-weight: bold;
    font-size: larger;
}
footer .author{
    color: rgb(245, 126, 7);
    
}
footer .name{
    font-weight: bold;
    font-family: cursive;
    margin-left: 50px;
    font-size: larger;
    color: rgb(220, 22, 68);
}

menu.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>admin page</title>
    <link rel="stylesheet" href="menu.css">
</head>
<body>
    <center>
        <h1>OUR  SPICHAL  MENU</h1>
        <div class="menu">
            <ul>
                <li><a href="res.html">HOME</a></li>
                <li><a href="menu.html">MENU</a></li>
                <li><a href="admin.html">ADMINISTRATION</a></li>
                <li><a href="contect.html">CONTACT US</a></li>
            </ul> 
        </div>
    <table>
        <tr>
            <td><img src="burger.jpeg">   <br><button href="#">order</button><br>chicken burker</td>
            <td><img src="bireyani.jpeg"> <br><button href="#">order</button><br>tum biriyani</td>
            <td><img src="dosa.jpeg">     <br><button href="#">order</button><br>onion dosa</td>
            <td><img src="kfc.jpeg">      <br><button href="#">order</button><br> fryed chicken</td>
        </tr>
        <tr>
            <td><img src="frys.jpeg">     <br><button href="#">order</button><br>finger chipes</td>
            <td><img src="meal.jpeg">     <br><button href="#">order</button><br>kerala meal</td>
            <td><img src="pastha.jpeg">   <br><button href="#">order</button><br>allo pastha</td>
            <td><img src="thali.jpeg">    <br><button href="#">order</button><br>panjabi thali</td>
        </tr>
        <tr>
            <td> <img src="parota.jpeg">  <br><button href="#">order</button><br>bun porotta</td>
            <td><img src="idly.jpeg">     <br><button href="#">order</button><br>madurai idly</td>
            <td> <img src="puri.jpeg">    <br><button href="#">order</button><br>andhra puri</td>
            <td><img src="kulfi.jpeg">    <br><button href="#">order</button><br>badham kulfi</td>
        </tr>
    </table>
    </center>
</body>
<footer>
    <hr style="color: rgb(91, 38, 38);"> 
    <center>
   <p class="author">DISIGNED AND DEVLOPED BY </p><P class="name">CHANDRU.K</P>
 </center>
 </footer
<style>
    .body{
        background-image:bgimage.jpeg ;
    }
</style>
</html>

menu.css

*
table{
   align-content: center; 
   margin-top: 140px;
}
body{
    background-image:url(bgiamge2.jpg) ;
    background-size: cover;
    backdrop-filter: blur(6px),darken(30px);
}
h1{
    word-spacing: 4px;
    color: rgba(207, 20, 20, 0.855);}
li{
    float: left;
    list-style: none;
}

ul li a{
display: flex;
padding-left: 50px;
padding-right: 50px;
color: aquamarine;
}
ul li a:hover{
    color: aliceblue;
    cursor: pointer;
}
.menu{
    margin-top: 60px;
    margin-left: 110px;
    border-width: 30px;
    border-color: aquamarine;
    background-color: rgb(84, 92, 92);
    display: inline-flex;
    padding-left: 30px;
    padding-right: 30px;
    color: rgb(176, 129, 100);
    border-radius:  25px}

td{
    background-color: blanchedalmond;
    padding: 9px;
    align-items: center;
    font-family: 'Times New Roman', Times, serif;
    font-weight: bold;
    text-align: center;

}
button{
    width: 60px;
    height: 20px;
    color: brown;

}
button :hover{
    color: aquamarine;
    cursor: pointer;
}
footer .author{
    color: rgb(245, 126, 7);
    
}
footer .name{
    font-weight: bold;
    font-family: cursive;
    margin-left: 50px;
    font-size: larger;
    color: rgb(220, 22, 68);
}

admin.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>admin page</title>
    <link rel="stylesheet" href="admin.css">
</head>
<body>
    <center>
        <h1>OUR ADMINISRATOES</h1>
        <div class="menu">
            <ul>
                <li><a href="res.html">HOME</a></li>
                <li><a href="menu.html">MENU</a></li>
                <li><a href="admin.html">ADMINISTRATION</a></li>
                <li><a href="contect.html">CONTACT US</a></li>
            </ul> 
        </div>
    <table>
        <tr>
            <td><img src="chef1.jpg"> <P>CHEF:Saravanan<br>CEO of saravanabavan.pvt.limited</P>  </td>
           <td><img src="chef2.jpg"> <p>CHEF:THAMU<br>most famose Indian celebrity chef</p> </td>
            <td><img src="chef3.jpg">  <p>CHEF:vankat bhat<br>most famose Indian celebrity chef</p>   </td>
        
        </tr>
        <tr>
            <td><img src="chef4.jpg">  <p>CHEF:kunnal kapuur<br>chif cook in taj hotels.pvt.limited</p>   </td>
            <td><img src="CHEF5.jpg"> <p>CHEF:Dalmia<br> first indian woman who won master chef tittle</p>    </td>
            <td><img src="chef6.jpg">  <P>CHEF:Garmaiya <br>very popular youtube channek chef</P> </td>
        </tr>
       
    </table>
    </center>
</body> 
<footer>
    <hr style="color: rgb(91, 38, 38);"> 
 </footer


</html>

asmin.css

header{
    ;
}
.name{
    margin-top: 13px;
    margin-left: 45%;
}
h1{
    font-family: 'Times New Roman', Times, serif;
    font-weight: bolder;
    font-size: 39px;
    color: rgba(215, 49, 7, 0.803);
    
}
.name2{
    font-family: cursive;
    font-size: 37px;
    color: rgba(222, 215, 13, 0.97);
    font-weight: bold;
    
}
li{
    float: left;
    list-style: none;
}

ul li a{
display: flex;
padding-left: 50px;
padding-right: 50px;
color: aquamarine;
}
ul li a:hover{
    color: aliceblue;
    cursor: pointer;
    transform: scale(1.3);
}
body{
    background-image: url(bg.jpg);
    background-size: cover;
    background-blend-mode: color-burn;
}
.menu{
    margin-top: 40px;
    margin-left: 80px;
    border-width: 30px;
    border-color: aquamarine;
    background-color: rgb(84, 92, 92);
    display: inline-flex;
    padding-left: 30px;
    padding-right: 30px;
    color: rgb(176, 129, 100);
    border-radius:  25px;
}
.food{
    margin-top: 90px;
    padding: 14px;
}
td{
padding: 20px;
background-color:rgba(15, 1, 1, 0.636);
border-width: px;
border-radius: 18px;
white-space: 5px;
color: azure;
}
tr{
    padding: 5px;
}
p{
    font-weight: bolder;
    align-items: center;
}
img{
    align-items: center;
}  

footer .author{
    color: rgb(245, 126, 7);
    
}
footer .name{
    font-weight: bold;
    font-family: cursive;
    margin-left: 50px;
    font-size: larger;
    color: rgb(220, 22, 68);
}
table tr td img{
    border-radius: 50%;
}
table{
    margin-top: 80px;
}

contect.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>admin page</title>
    <link rel="stylesheet" href="contect.css">
</head>
<body>
    <center>
        <h1>CONTECT US</h1>
        <div class="menu">
            <ul>
                <li><a href="res.html">HOME</a></li>
                <li><a href="menu.html">MENU</a></li>
                <li><a href="admin.html">ADMINISTRATION</a></li>
                <li><a href="contect.html">CONTACT US</a></li>
            </ul> 
        </div>
        </center>
        <div class="form">
           <center> 
            <h1>contect us</h1>
            <input type="name" name="name" placeholder="Enter your name here">
            <input type="name" placeholder="Enter your number">
            <input type="number" name="" placeholder="Enter age here">
            <button class="btrn"><a href="#">send massage</a></button>
            <h1>our contect No:98765432</h1>
        </center>
       </div>
        </body>
        </html>

contect.css

header{
    ;
}
.name{
    margin-top: 13px;
    margin-left: 45%;
}
h1{
    font-family: 'Times New Roman', Times, serif;
    font-weight: bolder;
    font-size: 39px;
    color: rgba(215, 49, 7, 0.803);
    
}
.name2{
    font-family: cursive;
    font-size: 37px;
    color: rgba(222, 215, 13, 0.97);
    font-weight: bold;
    
}
li{
    float: left;
    list-style: none;
}

ul li a{
display: flex;
padding-left: 50px;
padding-right: 50px;
color: aquamarine;
}
ul li a:hover{
    color: aliceblue;
    cursor: pointer;
    transform: scale(1.3);
}
body{
    background-image: url(bg.jpg);
    background-size: cover;
    background-blend-mode: color-burn;
}
.menu{
    margin-top: 40px;
    margin-left: 80px;
    border-width: 30px;
    border-color: aquamarine;
    background-color: rgb(84, 92, 92);
    display: inline-flex;
    padding-left: 30px;
    padding-right: 30px;
    color: rgb(176, 129, 100);
    border-radius:  25px;
}
.form{
    width: 320px;
    height: 350px;
    background: linear-gradient(to top,rgba(0,0,0,0.8)50%,rgba(0,0,0,0.8)50%);
    position: absolute;
    top: 250px;
    left: 600px;
    border: 3px;
    border-style: groove;                
    align-items: center;
}
.form h1{
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    text-align: center;
    color: #de1212;
    width: 220px;
    font-size: 22px;
    background-color: aliceblue;
    border-radius: 30px;
    margin: 2px;
    padding: 8px;

}

.form input{
    background: transparent;
    width: 240px;
    height: 28px;
     border-bottom: 1px solid  #de1212;
     border-top: none;
     border-left: none;
     border-right: none;
     color: aliceblue;
     font-size: 10px;
     letter-spacing: 1px;
     margin-top: 25px;
     font-family: Verdana, Geneva, Tahoma, sans-serif;
}
.form input :focus{
    outline: none;
}

::placeholder{
    color: aliceblue;
    font-family: arial;

}

.btrn{
    width: 240px;
    height: 40px;
    background: #de1212;
    margin-top: 26px;
    font-size: 16px;
    border-radius:10px;
    cursor: pointer;
    color: rgb(235, 239, 242);
    transition: 0.4s ea;
}

.btrn :hover{
    background: #f3f6f7;
    color: #de1271;
    width: 240px;
    height: 40px;
}
.btrn a{
    text-decoration: none;
    color: black;
    font-weight: bold;
}
.form .link{
    font-family: Arial, Helvetica, sans-serif;
    font size: 17px;
    text align:center;
    padding-top:20px

}
.form .link a{
    text-decoration:none;
    color: #de1212;
}
.liw{padding-bottom: 10px;
    text-align: center;
    padding-top: 14px;
    

}
.icons a{
    color: aliceblue;
    text-decoration: none;
}
.icons ion-icon{
    color: aliceblue;
    font-size: 30px;
    padding-left: 14px;
    padding-top: 5px;
}
```

# OUTPUT:
![image](https://github.com/user-attachments/assets/bb4720da-121f-4ae6-a9ad-5b1c8cd97491)

![image](https://github.com/user-attachments/assets/818bf4eb-af51-4a33-bea3-f9e24a6898b7)

![image](https://github.com/user-attachments/assets/c912387c-ce2c-4b1a-9272-14c042b7acc1)

![image](https://github.com/user-attachments/assets/29c1d81b-33da-422e-a21a-c9c53115a9ad)




# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
