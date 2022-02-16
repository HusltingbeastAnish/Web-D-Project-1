# Web-D-Project-1
This project is a fully responsive website which is formed using HTML and CSS




<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Best Online Food Outlet Services | Spiceup</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Lobster&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Baloo+Bhai+2:wght@500&display=swap" rel="stylesheet">
    <link rel="stylesheet" media="screen and (max-width:1170px)" href="phone.css">
</head>

<body>
    <nav id="navbar">
        <div id="logo">
            <img src="Anishdp.jpeg" alt="Oops Slow internet">
        </div>
        <ul>
            <li id="item"><a href="#">Home</a></li>
            <li id="item"><a href="#">Menu</a></li>
            <li id="item"><a href="#">About Us</a></li>
            <li id="item"><a href="#">Contact</a></li>
        </ul>
    </nav>
    <section id="home">
        <div id="container">
          <h2 class="h-primary">Welcome To My Food Outlet</h2> 
          
            <p class="p-primary">We can deliver your craving with half hour</p>
            <p class="p-primary">We are know for our best services in Jamshedpur</p>
            <button class="btn">Order Now!</button>
        </div>
        <hr>
        <section id="services">
            <h2 class="h-primary " class="center">Welcome To Spice Up </h2>
            <div class="container">
                <div id="box1" class="box">
                    <img src="Food.jpg" alt="">
                    <h2 class="h-secondary center">Chineese Dishes</h2>
                    <p class="p-primary">Order your first Chineese Dishand get 20% discount</p>
                </div>
                <div id="box2" class="box">
                    <img src="pizza.jpg" alt="">
                    <h2 class="h-secondary center">Pizza</h2>
                    <p class="p-primary">Order your First Pizza and get 20% discount</p>
                </div>
                <div id="box3" class="box">
                    <img src="delivery.png" alt="">
                    <h2 class="h-secondary center">Super Fast Delivery</h2>
                    <p class="p-primary">Get Super Fast delivery on your first order</p>
                </div>
            </div>
        </section>
        <hr>

    </section>
    <section id="client-section">
        <h2 class="h-primary center">Our Clients </h2> 
        <div id="clients">
            <div id="client-item1" class="client-item">
                <img src="facebook.jpg" alt="">
            </div>
            <div id="client-item2" class="client-item">
                <img src="instagram.jpg" alt="">
            </div>
            <div id="client-item3" class="client-item">
                <img src="twitter.jpg" alt="">
            </div>
            <div id="client-item4" class="client-item">
                <img src="linkdin.jpg" alt="">
            </div>
        </div>   
    
    </section>

    <!-- Services Section  -->
    <section id="contact">
        <h2 class="h-primary center">Contact Us </h2>
        <div id="contact-box">
            <form action="backend.php">
                <div class="form-group">
                    <label for="name" >Name:</label>
                    <input type="text" name="name" placeholder="Enter Your Name ">
                </div>
                <div class="form-group">
                    <label for="name" >Email:</label>
                    <input type="text" name="name" placeholder="Enter Your Email ">
                </div>
                <div class="form-group">
                    <label for="name" >Phone No.:</label>
                    <input type="Phone" name="name" placeholder="Enter Your PhoneNumber ">
                </div>
                <div class="form-group">
                    <label for="name" >Message</label>
                    <textarea name="message" id="message" cols="30" rows="10"></textarea>
                </div>
            </form>
        </div>
    </section>
    <footer>
        <div class="center"> Copyright &copy; All Rights Reserved!!</div>
    </footer>


</body>

</html>



_______________________________________________________________________________________________________________________________________________________________________
The CSS File is :

/* CSS Reset  */
*{
    margin: 0;
    padding: 0;
    
}

#navbar{
    position: fixed;
    /* navbar ka position ko relative krne se background-color ka height surf navbar me hi adjust ho jaega  */
    display: flex;
    
}

#navbar ul{
    display: flex;}
    
    #navbar::before{
        content: "";
        background-color:rgb(43, 15, 15);
        position: absolute;
        height: 100%;
        width: 100%;
        z-index: -1;
        opacity: 0.7;
    }
    #navbar ul li{
        padding: 25px 1px;
        list-style: none;
        font-size: 1.4rem;
        
    }
    #navbar ul li a{
        border-radius: 25px;
        color: white;
        padding: 10px 12px;
        display: block;
        text-decoration: none;
        font-family: 'Baloo Bhai 2', cursive;
        
    }
    #navbar ul li a:hover{
        background-color: white;
        color: black;
    }
    #logo img{
        height: 117px;
        width: 115px;
        border-radius: 123px;
    }
.btn{
    border-radius: 30px;
    background-color: brown;
    padding: 5px 8px;
    color: white;
    cursor: pointer;
    /* cursor pointer kr dene se jab btn pe cursor le jaengey to haath banke aega  */
}
.btn:hover{
    background-color: black;
    color: grey;
}
#home{
    
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 665px;
    margin-bottom: 4px;
}
#home::before{
    content: "";
    position: absolute;
    background:url("Restro.jpg") ;
    background-repeat: no-repeat;
    background-size: cover;
    background-repeat: none;
    height: 100%;
    width: 100%;
    z-index: -1;
    opacity: 0.8;

}

/* Utility class( When We make classes so that it can reflect changes at similar  places it is called utility class) */
.h-primary{
    font-size: 25px;
    padding: 5px;
    font-family: 'Baloo Bhai 2', cursive;
   
  
}
.p-primary{
    font-size: 25px;
    padding: 5px;
  
    font-family: 'Lobster', cursive;
}
/* We have made a utility class in which we have made a center class so that where ever we will need to align the text at the center we can use that class  */
.center{
    text-align: center;
}



/* Service Section  */
#services {
    display:flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 34px;
}
#services .box{
    border: 2px solid red;
    background-color:#372637;
    margin: 10px;
    border-radius: 25px;
    color: white;
  
}
#services .box img{
    display: block;
    margin: auto;
    /* display block krke margin auto krne se box ka content center me aa jata hai  */
    padding: 10px 12px;
}
.container{
    display: flex;

}
#container{
    margin-top: 80px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
#box2 img{
    height: 178px;
    width: 280px;
}
#box3 img{
    height: 178px;
    width: 264px;
}



/* Client Section  */

#client-section{
    padding-top: 20px;
    padding-bottom: -10px;
}
#clients{
    
    display: flex;
    justify-content: center;
    align-items: center;
}
.clients img{
    height: 100px;
    width:100px ;
    padding: 25px;
   
}
#client-item1 img{
height: 83px;
    width: 90px;
}


#client-item2 img{   
     height: 75px;
    width: 77px;
}
#client-item3 img{
    height: 90px;
    width: 97px;
}
#client-item4 img{
    height: 80px;
    width: 78px;
}
#client-section::before
{
    content: "";
    position: absolute;
    background:url("clientbackground.jpg");
   background-repeat: no-repeat;
   background-size: cover;
   height: 38%; 
    width: 100%;
    z-index: -1;
    opacity: 0.7;

}

/* Designing of the contact section  */
#contact::before{
    content: "";
    position: absolute;
    background: url("contact.jpg") ;
    background-repeat: no-repeat;
    background-size: cover;
    height: 54%;
    width: 100%;
    z-index: -1;
    opacity: 0.7;
    margin-top: 68px;

}
#clients img{
    padding: 20px;
    margin: -11px;
}
footer{background-color: black;
    color: white;

}
#contact{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding-top: 43px;
  
  
}
#contact h2{
    margin-top: 67px;
}
#contact-box input{
    width: 100%;
    padding: 0.5rem;
}
#contact-box textarea{
    width: 100%;
    padding: 0.5rem;
    height: 100px;
    width: 100px;
}
#contact-box{
    padding-bottom: 23px;
}
#contact-box label{
    font-family: 'Baloo Bhai 2', cursive;
}
.box{
    transition: all 0.5s ease-in-out 0.1s;
}
#box1:hover{
    transform: scale(1.14);
}
#box2:hover{
    transform: scale(1.14);
}
#box3:hover{
    transform: scale(1.14);
}
#clients img:hover{
    transform: scale(1.18);
}

