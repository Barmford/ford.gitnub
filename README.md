<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FordMartrix PortFolio</title>
    <!--FontAwesome Kits Code-->
    <script src="https://kit.fontawesome.com/aae94b1b16.js" crossorigin="anonymous"></script>
    <style>
        html{
            scroll-behavior: smooth;
        }
        body{
            background: rgb(26, 37, 34);
            color: rgb(8, 1, 1);
        }
        header{
            width: 100%;
            height: 100vh;
            background-image: url(Letter\ M\ Am\ Ma\ Mm\ Monogram\ Logo\ Design\ Minimal\ PNG\ Images\,\ \ Logo\,\ Ma\,\ Am\ PNG\ Transparent\ Background\ -\ Pngtree.jpeg);
            background-size: cover;
            background-position: center;
        }
        .container{
            padding: 10px 10%;

        }
        nav{
            display: flex;
            align-items: center;
            justify-content: space-between;
            flex-wrap: wrap;
        }
        .logo{
            width:140px;
        }
        nav ul li{
            display: inline-block;
            list-style: none;
            margin: 10px 20px;
        }
        nav ul li a{
            color: rgb(0, 0, 0);
            text-decoration: none;
            font-size: 18px;
            position: relative;
        }
        nav ul li a::after{
            content: '';
            width: 0;
            height: 3px;
            background: #24fc08;
            position: absolute;
            left: 0;
            bottom: -6px;
            transition: 0.5s;
        }
        nav ul li a:hover::after{
            width: 100%;
        }
        nav .fas{
            display: none;
        }
        .header-text{
            margin-top: 20%;
            font-size: 30px;
        }
    .header-text h1{
        font-size: 60px;
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    }
    #About{
        padding: 80px 0;
        color: rgb(83, 241, 207);
    }
    .row{
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
    }
    .about-col-1{
        flex-basis: 35%;
    }
    .about-col-1 img{
        border-radius: 15px;
        width: 100%;
        height: 100%;
    }
    .about-col-2{
        flex-basis: 60%;
    } 
    .sub-title{
        font-size: 60px;
        font-weight: 600;
        color: white;
    }
    .tab-titles{
        display: flex;
        margin: 20px 0 40px;
    }
    .tab-links{
        margin-right: 50px;
        font-size: 18px;
        font-weight: 500;
        cursor: pointer;
        position: relative;
    }
    .tab-links::after{
        content: '';
        width: 0%;
        height: 3px;
        background: #00ff22;
        position: absolute;
        left: 0%;
        bottom: -8px;
        transition: 0.5s;
    }
    .tab-links.active-link::after{
        width: 50%;
    }
    .tab-contents ul li{
        list-style: none;
        margin: 10px 0;
    }
    .tab-contents ul li span{
        color: #b61414;
        font-size: 14px;
    }
    .tab-contents{
        display: none;
    }
    .tab-contents.active-tab{
        display: block;
    }
    <!-- services-->
    #services{
        padding: 30px 0;
    }
    .services-list{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
        grid-gap: 40px;
        margin-top: 50px;
    }
    .services-list div{
        background: #262626;
        padding: 40px;
        font-size: 13px;
        font-weight: 300;
        border-radius: 10px;
        transition: (background 0.5s)transform 0.5s;
        border-radius: 10px;
    }
    .services-list div i{
        font-size: 50px;
        margin-bottom: 30px;

    }
    .services-list div h3{
        font-size: 30px;
        font-weight: 500;
        margin-bottom: 15px;
    }
    .services-list div a{
        text-decoration: none;
        color: #fff;
        font-size: 12px;
        margin-top: 20px;
        display: inline-block;
    }
    .services-list div:hover{
        background: rgb(172, 19, 19);
        transform: translateY(-10px)

    }
 <!--Portfolio-->
    #Portfolio{
        padding: 50px 0;

    }
    .Worklist{
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
        grid-gap: 40px;
        margin-top: 50px;
    }
    .work{
        border-radius: 10px;
        position: relative;
        overflow: hidden;
    }
    .work img{
        width: 100%;
        height: 70%;
        border-radius: 10px;
        display: block;
        transition: transform 0,5s;
    }
    .layer{
        width: 100%;
        height: 0%;
        background: linear-gradient(rgba(0,0,0,0.6), #ff004f);
        border-radius: 10px;
        position: absolute;
        left: 0;
        bottom: 0;
        overflow: hidden;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        padding: 0 40px;
        text-align: center;
        font-size: 14px;
        transition: height 0.5s;
    }
    .layer h3{
        font-weight: 500;
        margin-bottom: 20px;
    }
    .work:hover img{
        transform: scale(1.1);
    }
    .work:hover .layer{
        height: 100%;
    }
    .btn{
        display: block;
        margin: 50px auto;
        width: fit-content;
        border: 1px solid #ff004f;
        padding: 14px 50px;
        border-radius: 6px;
        text-decoration: none;
        color: #fff;
        transition: background 0.5s;
    }
    .btn:hover{
        background: #ff004f;
    }
    <!--Contact-->
    .contact-left{
        flex-basis: 35%;
    }
    .contact-right{
        flex-basis: 60%;
    }
    .contact-left p{
       margin-top: 30px;
    }
    .contact-left p i{
        color: #3cff00;
        margin-right: 15px;
        font-size: 25px;
        transition: transform 0.5s;
    }
    .contact-left p i:hover{
        color: #ff004f;
        transform: translateY(-5px);
    }
    .social-icons{
        margin: 30px;
    }
    .social-icons a{
        text-decoration: none;
        font-size: 30px;
        margin-right: 15px;
        color: #ababab;
        display: inline-block;
        transition: transform 0.5s;
    }
    .social-icons a:hover{
        color: #ff004f;
        transform: translateY(-5px);
    }
    .btn.btn2{
        display: inline-block;
        background: #ff004f;
    }
    .contact-right form{
        width: 100%;
    }
    form input, form textarea{
        width: 100%;
        border: 0;
        outline: none;
        background: #262626;
        padding: 15px;
        margin: 15px 0;
        color:#fff;
        font-size: 18px;
        border-radius: 6px;
    }
    form .btn2{
        padding: 14px;
        font-size: 18px;
        margin-top: 20px;
        cursor: pointer;
    }
    .copyright{
        width: 100%;
        text-align: center;
        padding: 25px 0;
        background: #262626;
        font-weight: 300;
        margin-top: 20px;
    }
    .copyright i{
        color: #00ff22;
    }
    @media only screen and (max-width:600px) {
        #header-text{
            margin-top: 100%;
            font-size: 16px;
        }
        .header-text h1{
            font-size: 30px;
        }
        nav .fas{
            display: block;
            font-size: 25px;
        }
        nav ul{
            background: #ff004f;
            position: fixed;
            top: 0%;
            right: -200px;
            width: 200px;
            height: 100vh;
            padding-top: 50px;
            z-index: 2;
            transform: right 0.7s;
        }
        nav ul li{
            display: block;
            margin: 25px;
        }
        nav ul.fas{
            position: absolute;
            top: 25px;
            left: 25px;
            cursor: pointer;
        }
        .sub-title{
            font-size: 40px;
        }
        .about-col-1, .about-col-2{
            flex-basis: 100%;
        }
        .about-col-1{
            margin-bottom: 30px;

        }
        .about-col-2{
            font-size: 14px;
        }
        .tab-links{
            font-size: 16px;
            margin-right: 20px;
        }
        .contact-left,.contact-right{
            flex-basis: 100%;
        }
        .copyright{
            font-size: 14px;
        }
    }
    #span{
        color: #61b752;
        margin-top: -40px;
        display: block;
    }
    </style>
</head>
<body>
    <div id="header">
        <header>
            <div class="container">
            <nav >
                <img src="Artboard 1@2x-100.jpg" class="logo">
                <ul id="sidemenu">
                    <li><a href="#header"> Home</a></li>
                    <li><a href="#About"> About</a></li>
                    <li><a href="#services"> My Services</a></li>
                    <li><a href="#Portfolio"> My Work</a></li>
                    <li><a href="#Contact"> Contact Me</a></li>
                   <i class="fas fa-times"onclick="closemenu()"></i> 
                </ul>
                <i class="fas fa-bars" onclick="openmenu()"></i>
            </nav>
        </div>
        <div id="header-text">
            <p>FORDMARTRIX</p>
            <H1>Hello, We are<span style="color: #0bff17;">FordMartrix</span> <br> from Nairobi Kenya</H1>
        </div>
        </header>

        <!--About-->
    </div>
    <div id="About">
        <div class="container">
            <div class="row">
                <div class="about-col-1">
                    <img src="20240315_124118.jpg" alt=" photo">
                </div>
                <div class="about-col-2">
                <h2 class="sub-title">ABOUT ME</h2>
                <p >Welcome to <b>Ford Matrix</b>, your one-stop destination for all your creative needs! <br>
                <p> Are you looking to elevate your brand with captivating visuals, engaging voiceovers, and impactful advertising? <br>Look no further! Our team of expert designers, talented voice artists, <br>and seasoned advertisers are here to bring your vision to life.</p>
                </p>
                
                <div class="tab-titles">
                    <p class="tab-links active-link" onclick="opentab('Skills')">Skills</p>
                    <p class="tab-links" onclick="opentab('Experience')">Experience</p>
                    <p class="tab-links" onclick="opentab('Education')">Education</p>
                </div>
                <div class="tab-contents active-tab" id="Skills">
                    <ul>
                        <li><span>Advertising</span> <br>I write Scripts for Adverts</li>
                        <li><span>Graphical</span> <br>I do Graphical design </li>
                        <li><span>Voice Over</span> <br> I do the best Voice Over's</li>
                        <li><span>Script</span> <br> I'm a good Script writer </li>
                    </ul>
                </div>
                <div class="tab-contents"id="Experience">
                    <ul>
                        <li><span>Attachment</span> <br> Kenya Broadcasting Corporation (KBC)</li>
                        <li><span>Internship</span> <br> Moonsun International</li>
                    </ul>
                </div>
                <div class="tab-contents" id="Education">
                    <ul>
                        <li><span>Primary</span> <br> Unity Primary School </li>
                        <li><span>High School</span> <br> Shikunga High</li>
                        <li><span>University</span> <br>The Presbyterian University of East Africa</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
<!--services-->
            <div id="services">
                <div class="container">
                    <h2 class="sub-title">My Services</h2>
                    <div class="services-list">
                        <div>
                            <i class="fas fa-code"></i>
                            <h3>Graphical Design</h3>
                            <p>First impressions matter,and our graphic design team is dedicated to creating <br>visually stunning graphics that resonate with your audience. From logo design to branding<br> materials,we craft designs that leave a lasting impression and communicate your brand's identity effectively.</p>
                            <a href="#">Learn More</a>
                        </div>
                        <div>
                            <i class="fas fa-crop-alt"></i>
                            <h3>Advertising Script</h3>
                            <p>Stand out in today's competitive market with our tailored advertising <br>solutions. Whether you're looking to launch a new product, promote<br> an event, or increase brand awareness, our advertising experts will<br> develop strategies that resonate with your target audience and drive<br> results.</p>
                            <a href="#">Learn More</a>
                        </div>
                        <div>
                            <i class="fa-brands fa-app-store"></i>
                           <h3>Voice Over</h3>
                            <p>Capture your audience's attention with compelling voiceovers that convey your<br> message with clarity and emotion. Our team of professional voice <br>artists can provide a wide range of styles and tones<br>to suit your project, whether it's for commercials, animations, audiobooks, <br>or presentations.</p>
                            <a href="#">Learn More</a> 
                        </div>
                    </div>
                </div>
            </div>
<!----Portfolio-->
            <div id="Portfolio">
                <div class="container">
                    <h3 class="sub-title">My Work</h3>
                    <div class="Worklist">
                        <div class="work">
                            <img src="Happy international womens day.png" alt="posters">
                            <div class="layer">
                                <h4>Womens International Day</h4>
                                <p>This Poster was dedicated to all the <br>Women, celebrating them for being<br> our Super Heroes</p>
                            </div>
                        </div>
                        <div class="work">
                            <img src="Flowers Flyer.jpg" alt="posters">
                            <div class="layer">
                                <h4>Valentines Day</h4>
                                <p>This Poster was dedicated to all the Lovers, <br>to give Comfort to every Couple <br>in the City</p>
                            </div>
                        </div>
                        <div class="work">
                            <img src="BET 4.jpg" alt="posters">
                            <div class="layer">
                                <h4>Betting Poster</h4>
                                <p>Do you love Betting?, <br>Join Bang Bet to enjoy the best Odds.</p>
                            </div>
                        </div>
                        <div class="work">
                            <audio controls src="Promo 2 Mixdown.mp3"></audio>
                        </div>
                        <div class="work">
                            <audio controls src="Q7 Kiu yako Mixdown 1.mp3"></audio>
                        </div>
                        <div class="work">
                            <audio controls src="Pwani  Mixdown 1.mp3"></audio>
                        </div>
                    </div>
                    <a href="#" class="btn">See More</a>
                </div>
            </div>
<!--Contact-->
            <div id="Contact">
                <div class="container">
                    <div class="row">
                        <div class="contact-left">
                            <h2 class="sub-title">Contact me</h2>
                            <p><i class="fa-solid fa-paper-plane"></i>alvisbarmford@gmail.com</p>
                            <p ><i class="fa-solid fa-phone"> </i>0799941170</p>
                            <div class="social-icons">
                                <a href="https://www.instgram.com/zir_ford?igsh=czUwdzRpZWxvNTgw"><i class="fa-brands fa-instagram"></i></a>
                                <a href="https://www.threads.net/@zir_ford"><i class="fa-brands fa-threads"></i></i></i></a>
                            </div>
                            <a href="Barmford Resume.pdf" download class="btn btn2" class="btn btn2">Download CV</a>
                        </div>
                        <div class="contact-right">
                            <form  name="submit-to-google-sheet">
                                <input type="text" name="Name" placeholder="Your Name" required>
                                <input type="email" name="Email" placeholder="Your Email" required>
                                <textarea name="Message" rows="6" placeholder="Your Message"></textarea>
                                <button type="submit" class="btn btn2"> Submit</button>
                            </form>
                            <span id="msg"></span>
                        </div>
                    </div>

                </div>
                <div class="copyright">
                    <p>&copy; 2024 FordMartrix PortFolio<i class="fa-solid fa-umbrella"></i>. All rights reserved.</p>
                </div>
            </div>

    <!--Java Script-->
    <script>
        var tablinks = document.getElementsByClassName("tab-links");
        var tabcontents = document.getElementsByClassName("tab-contents");
        function opentab(tabname){
            for(tablink of tablinks){
                tablink.classList.remove("active-link");
            }
            for(tabcontent of tabcontents){
                tabcontent.classList.remove("active-tab");
            }
            event.currentTarget.classList.add("active-link");
            document.getElementById(tabname).classList.add("active-tab")
        }   
    </script>
    <script>
        var sidemenu=document.getElementById("sidemenu")
        function openmenu(){
            sidemenu.style.right="0";
        }
        function closemenu(){
            sidemenu.style.right="-200px";
        }
    </script>
   

<script>
  const scriptURL = 'https://script.google.com/macros/s/AKfycbwn8fPGkzpgKFUeaWmoIEifNj2acj019D8Ei9n_7MAfm_kuHvwQLLBkp3Axpt-NaJGKFw/exec'
  const form = document.forms['submit-to-google-sheet']
  const msg = document.getElementById("msg")

  form.addEventListener('submit', e => {
    e.preventDefault()
    fetch(scriptURL, { method: 'POST', body: new FormData(form)})
      .then(response => {
        msg.innerHTML ="Message sent Successfully"
        setTimeout(function(){
            msg.innerHTML =""
        },5000)
        form.reset()
      })
      .catch(error => console.error('Error!', error.message))
  })
</script>
</body>
</html>
