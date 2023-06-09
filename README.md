# exp2-commercial-website
# EXP 02 - CREATING A COMMERCIAL WEBSITE USING HTML & CSS
## AIM:

To create a commercial website using html and css.

## SOFTWARE:

Visual Studio Code.

## ALGORITHM:

1) Create a new HTML file and save it with a .html extension.Begin with the basic structure by adding the <!DOCTYPE html> declaration at the top.
2) Set up the Head:

       Inside the <head> element, add the <title> element and give it a meaningful title for your website.
       Link your CSS file by adding the <link> element with the rel attribute set to "stylesheet" and 
       the href attribute pointing to your CSS file.

3) Develop the Content:

        Divide the main content area into sections using appropriate HTML elements like <section>, <div>, or <article>.
        Use headings <h1> to <h6> to structure your content hierarchically.
        Incorporate text, images, videos, and other media within the content sectionS


4) Style with CSS:
 
  Create a new CSS file and save it with a .css extension.
  Select the elements you want to style using CSS selectors.
  Apply styles using properties and values. 
  For example, you can change colors, fonts, sizes, margins, and padding.

5) Find a web hosting provider to host your website online.
Upload your HTML, CSS, and any other necessary files to the hosting server.

6) Test your website again after deployment to ensure it works as intended.
## PROGRAM:
### HTML CODE:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BAKERY</title>
    <link rel="stylesheet" href="bak.css" />
</head>
<body>
    <nav class="navbar">
        <ul>
            <li><a herf="#home">HOME&emsp;&emsp;</a></li>
            <li><a herf="#pages">PAGES&emsp;&emsp;</a></li>
            <li><a herf="#portfolio">PORTFOLIO&emsp;&emsp;</a></li>
            <li ><img src="font-removebg-preview.png" style="width: 150px; margin-top: 40px;"></li>
            <li><a herf="#blog">&emsp;BLOG&emsp;&emsp;</a></li>
            <li><a herf="#shop">SHOP&emsp;&emsp;</a></li>
            <li><a herf="#elements">ELEMENTS&emsp;&emsp;</a></li>
        </ul>
        <br><br>
        
    </nav>
    <section class="con">
        <div><img src="its-removebg-preview.png" class="image" ></div>
        <div><img src="bakery-removebg-preview.png" class="image1" ></div>
        <div><img src="time-removebg-preview.png" class="image2"></div>
    </section>


    <section class="s2">  
        <div class="ima">
            <img src="rolls-removebg-preview.png" style="height: 400px; margin-left: 20px;">
        </div>
        <!-- <div class="box1"></div> -->
        <!-- <p class="box">CINNAMON ROLLS</p> -->
        <p class="box">
            <b style="letter-spacing: 6px;">CINNAMON ROLLS </b><br><br>
            A cinnamon roll is a sweet roll commonly served in Northern Europe and North America.
             In Sweden it is called kanelbulle, in Denmark it is known as kanelsnegl. <br><br><br>
             <button type="button" class="block">READ MORE</button>
          
        </p>
    </section>


    <section class="s3">
        <div class="i"><img src="donut-strawberry.png" style="height: 350px;"></div>
        <p class="secondbox">
            <b style="letter-spacing: 6px;">STRAWBERRY</b><br>
            <b style="letter-spacing: 6px;">DONUT</b><br><br>
            a small cake of sweetened or, sometimes, unsweetened dough fried in deep fat,
             typically shaped like a ring or, when prepared with a filling, a ball.
             anything shaped like a thick ring; an annular object; toroid. <br><br><br>
             <button type="button" class="block">READ MORE</button>
          
        </p>
    </section>

    <section >  
        <div class="ima1">
            <img src="croissant-removebg-preview.png" style="height: 400px; margin-left: 20px;">
        </div>
        <!-- <div class="box1"></div> -->
        <!-- <p class="box">CINNAMON ROLLS</p> -->
        <p class="thirdbox">
            <b style="letter-spacing: 6px;">POPPY CROISSANT</b><br><br>
            A croissant is a buttery, flaky, viennoiserie pastry inspired
             by the shape of the Austrian kipferl but using the French yeast-leavened laminated dough. <br><br><br>
             <button type="button" class="block">READ MORE</button>
          
        </p>
        
    </section>

    <section >
        <div class="blue"><img src="muffin-blueberry-removebg-preview.png" style="height: 350px;"></div>
        <p class="fourthbox">
            <b style="letter-spacing: 6px;">BLUEBERRY</b><br>
            <b style="letter-spacing: 6px;">MUFFIN</b><br><br>
            a small cake of sweetened or, sometimes, unsweetened dough fried in deep fat,
             typically shaped like a ring or, when prepared with a filling, a ball.
             anything shaped like a thick ring; an annular object; toroid. <br><br><br>
             <button type="button" class="block">READ MORE</button>
          
        </p>
    </section>
    <div class="footer">
        Copyright &#169; 2023 BAKERY Developed by Anitha palani.
        <button type="button" class="block1">PURCHASE NOW</button>
      </div>
    
    
    
    
</body>
</html>

```
### CSS CODE:
```
*
{
    margin: 0;
    padding: 0;
}
html{
    scroll-behavior: smooth;
}
.navbar{
    display : flex;
    justify-content: center;
    height: 50px;
    align-items: center;
    /* position: sticky; */
    top: 0;
}
.navbar::before{
    content: "";
    position: absolute;
    background-color: rgb(247, 184, 195);
    height: 100%;
    width: 100%;
    z-index: -1;
}
.navbar ul{
    display : flex;
    list-style: none;
}
.navbar ul li{
    font-size: 1.1rem;
}
.navbar ul li a{
    position: relative;
    top: 60px;
    text-decoration: none;
    color: rgb(6, 2, 2);
}
.navbar ul li a:hover{
    border-bottom: 2px solid yellow;

}

.image{
    position: absolute;
    top: 10%;
    left: 45%;
}
.image1
{
    position: absolute;
    top: 25%;
    left: 30%;
}
.image2
{
    position: absolute;
    top: 30%;
    left: 52%;

}
/* .s1{
    height: 700px;
    width: 1590px;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    
    color: rgb(36, 22, 22);
    background-color: #f2e1e6;
    padding: 50px;
    
    
}
.roll{
    display: flex;
    position: sticky;
    margin-top: 400px;
    margin-left: 350px;
    position: absolute;
    font-size: 50px;
} */
.box1{
    width: 700px;
    height: 200px;
    border-radius: 20px;
    background-color: rgb(243, 228, 237);
    margin-left: 700px;
    margin-top: 400px;
    
}
.s2{
    height: 1000px;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size: medium;
    color: rgb(196, 178, 178);
    background-color: rgb(243, 228, 237);
    padding: 50px;
    
}
.s4{
    height: 1500px;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size: medium;
    color: rgb(196, 178, 178);
    background-color: rgb(243, 228, 237);
    padding: 50px;
    
}
.ima{
    
    width: 335px;
    height: 500px;
    /* padding: 10px; */
    margin-left: 100px;
    margin-top: 90px;
    /* background-color: blue; */
    border-radius: 20px;

}
.ima1{
    
    width: 335px;
    height: 500px;
    /* padding: 10px; */
    margin-left: 180px;
    margin-top: 350px;
    /* background-color: blue; */
    border-radius: 20px;

}
.box
{
    display: block;
    /* top: 0%; */
    height: 200px;
    width: 800px;
    color: rgb(17, 12, 3);
    background-color: rgb(243, 228, 237);
    margin-left: 550px;
    margin-top: -450px;
    border-radius: .50px;
    font-family: 'Times New Roman', Times, serif;
    font-size: 22px;
    word-spacing: 9px;
    letter-spacing: 0.45px;
    

}
.thirdbox
{
    display: block;
    /* top: 0%; */
    height: 200px;
    width: 800px;
    color: rgb(17, 12, 3);
    background-color: rgb(243, 228, 237);
    margin-left: 600px;
    margin-top: -450px;
    border-radius: .50px;
    font-family: 'Times New Roman', Times, serif;
    font-size: 22px;
    word-spacing: 9px;
    letter-spacing: 0.45px;
    
}
.con{
    height: 500px;
    background-color: rgb(247, 184, 195);

}
.block {
    
    width: 200px;
    height: 50px;
    border-radius: 5px;
    background-color:rgb(243, 228, 237);
    /* padding: 14px 28px; */
    padding-left: 2px;
    font-size: 16px;
    cursor: pointer;
    text-align: center;
    margin-left: 4px;
    margin-bottom: 20px;
  }
  .block1{
    
    width: 200px;
    height: 40px;
    /* border-radius: 5px; */
    background-color:rgb(17, 2, 11);
    /* padding: 14px 28px; */
    padding-left: 2px;
    font-size: 16px;
    cursor: pointer;
    color: antiquewhite;
    text-align: center;
    margin-left: 700px;
    margin-bottom: 20px;
  }
.secondbox
{
    display: block;
    /* top: 0%; */
    height: 250px;
    width: 800px;
    color: rgb(17, 12, 3);
    background-color: rgb(243, 228, 237);
    margin-left: 250px;
    margin-top: -1400px;
    border-radius: .50px;
    font-family: 'Times New Roman', Times, serif;
    font-size: 22px;
    word-spacing: 9px;
    letter-spacing: 0.45px;
    text-align: right;
    
}
.fourthbox
{
    display: block;
    /* top: 0%; */
    height: 250px;
    width: 800px;
    color: rgb(17, 12, 3);
    background-color: rgb(243, 228, 237);
    margin-left: 250px;
    margin-top: -1350px;
    border-radius: .50px;
    font-family: 'Times New Roman', Times, serif;
    font-size: 22px;
    word-spacing: 9px;
    letter-spacing: 0.45px;
    text-align: right;
    
}
.i{
    width: 380px;
    height: 500px;
    /* padding: 10px; */
    margin-left: 1200px;
     margin-top: -600px;
    /* background-color: blue; */
     top: 1000px; 
     margin-left: 70%;
    left: 70%;
    border-radius: 20px;
    /* background-color: aqua; */
    margin-bottom: 1000px;

}
.blue{
    width: 380px;
    height: 500px;
    /* padding: 10px; */
    margin-left: 1200px;
     margin-top: -4px;
    /* background-color: blue; */
     top: 500px; 
     margin-left: 70%;
    left: 70%;
    border-radius: 20px;
    /* background-color: aqua; */
    margin-bottom: 1000px;

}
.s3{
    height: 1000px;
    margin-bottom: -1550px;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size: medium;
    color: rgb(196, 178, 178);
    background-color: rgb(243, 228, 237);
    padding: 50px;
    
}
.footer {
    display: block;
    width: 1538px;
    height: 60px;
    background-color: rgb(247, 184, 195);
    padding-left: 150px;
    padding-top: 20px;
    margin-top:500px;
   
    color: rgb(23, 2, 2);
  }
```
## OUTPUT:
![image](https://github.com/anithapalani2123/exp2-commercial-website/assets/94184990/a5ba90b0-42ea-45d4-8189-ceb2ca346704)

![image](https://github.com/anithapalani2123/exp2-commercial-website/assets/94184990/6d3c1eb2-b6a7-4626-ba26-5b47f4d56093)

![image](https://github.com/anithapalani2123/exp2-commercial-website/assets/94184990/1a500c44-7029-46e8-a88a-7a055a23038e)
![image](https://github.com/anithapalani2123/exp2-commercial-website/assets/94184990/c4ce1df3-2efd-47df-911c-0edb43145767)





## RESULT:
      
Thus the website is created.



















