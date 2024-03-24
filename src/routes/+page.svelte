<script>

    import { NODE_ENV } from "$env/static/private";

</script>
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="shortcut icon" href="https://live.staticflickr.com/65535/53513844192_7c9f88587a_q.jpg" type="image/x-icon">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <title >Vishnu V</title>
    <style>
        
        body {
          background-color: white;
          color: black;
          scroll-behavior: smooth;
          background-position: 0%;
          margin:0%;
          background-repeat: no-repeat;
          background-size: auto;
          background-origin: 0%;
          padding:1%;
        }
        .dark-mode {
          background-color: black;
          color: white;
        }
                                      /* SCROLLBAR */
        ::webkit-scrollbar{
          height:10px;
        }
                                      /*conatiner of menu*/
        .container1 {
          display: flex;
          position: relative;
          justify-content: center;
          flex-direction:column;
        }
        .menu{
          display: flex;
          position:relative;
          align-items: center;
          justify-content: center;
          text-align: center;
          display:none;
        }
        .bar{
          display: inline-block;
          cursor: pointer;
          text-align: center;
        }
                                        /* name : vishnu v*/
        .name{
          width:25%;
          display:flex;
          margin-left: 5%;
          padding:0%;
          position:relative;
        }
        .n{
          margin: auto;
          position: relative;
          text-align: center;
          justify-content: center;
          align-items:center;
        }
                                        /* M E N U     I C O N  */

        .bar1, .bar2, .bar3 {
            background-color: rgba(196, 151, 3, 0.918);
            width: 19px;
            height: 2.5px;
            margin: 3px 0;
            transition: 0.4s;
            border-radius: 0.1rem;
        }
        .change .bar1 {
            transform: translate(0, 5.5px) rotate(-35deg);
        }
        .change .bar2 {opacity: 0;}
        
        .change .bar3 {
            transform: translate(0, -5.5px) rotate(35deg);
        }

                                            /*a l l    m e n u*/
        .nav{
          display: flex;
          height: 55px;
          position:fixed;
          width:100%;
          top:0;
          z-index:1000;
          backdrop-filter: blur(20px);
          overflow: hidden; 
          box-shadow: 1px 0px 0px 0px #10094b00 ;
        }
        .nav nav{
          width:80%;
          display:flex;
          justify-content: end;
        }
        .nav nav a  {  
          display:flex;
          justify-content: end;
          align-items: center;
          margin-right: 5%;
          text-decoration: none;
          color:inherit;
          cursor:pointer;
        }
        .mode{
          display:flex;
          margin-right:0% ;
          justify-content: end;
          align-items: center;
          margin-right: 5%;
          text-decoration: none;
          color:inherit;
          cursor:pointer;
          position: relative;
          margin-left:auto;
        }
        svg{
          width: 20px;
          height: 20px;
        }
        .dropdown{
          display:none;
        }
        .dropnav{
          display:flex;
          justify-content: center;
          width:100%;
          z-index: 1;
        }
        .dropnav a{
          display:flex;
          margin-right: 5%;
          text-decoration: none;
          color:inherit;
          cursor:pointer;
        }
        .intro{
        margin-top: 40px;
        }
        @media only  screen and (max-width: 1024px){
          .name{
              width:25%;
              margin-left:4%;
          }
          .nav nav{
              width:65%;
          }
          .dropdown{
              display:none;
          }
          .intro{
              margin-top: 40px;
          }
        }

        @media only  screen and (max-width: 860px){
          .nav nav{
              display:none;
          }
          .menu{
              display: flex;
          }
          .nav{
              height: 40px;
          }
          .name{
              font-size: 12px;
          } 
          .intro{
              margin-top: 35px;
          }
          svg{
              width: 12px;
              height: 12px;
          }
        }

        @media only  screen and (max-width: 640px){
          svg{
              width: 15px;
              height: 15px;
          }
          .nav{
              height: 45px;
          }
          .name{
              width:35%;
              font-size: 12px;
              justify-content: center;
          }
        
        }
        @media only  screen and (max-width: 475px){
          .container{
            padding-top:15%;
            padding-bottom:15%;
          }
          .content{
            text-align:justify-content;
          }
          .name{
              font-size: 13px;
              justify-content: center;
          }
          .mode{
              margin-right: 4%;
          }

          body{
              padding:1%;
          }
          svg{
              width: 15px;
              height: 15px;
          }
          .dropnav{
              flex-direction:column;
              gap:100px;
              width:100%;
              backdrop-filter: blur(20px);
              algin-items:center;
              justify-content:center;
              
          }
          .dropnav a{
              algin-items:center;
              justify-content:center;
          }
          .dropdown{
              font-size:13px;
          }
          .intro{
              margin-top: 55px;
          }
          .nav{
              height: 55px;
          }
        }
        @media only  screen and (max-width: 298px){
            .name{
              font-size: 8px;
              justify-content: center;
          }
        }
                                        /* S C R O L L I N G */
        .scroller{
          max-width:1000px;
          outline : 3px solid #fdae ;
          padding-left:5%;
          margin: auto ;
          
        }
        @media only  screen and (max-width: 1120px){
          .scroller{
            max-width:600px;
            margin: auto ;
          }
        }
        @media only  screen and (max-width: 660px){
          .scroller{
            max-width:400px;
            margin: auto ;
          }
        }
        @media only  screen and (max-width: 475px){
          .scroller{
            max-width:270px;
            margin: auto ;
          }
        }
        @media only  screen and (max-width: 320px){
          .scroller{
            max-width:200px;
            margin: auto ;
          }
        }

        legend{
          text-align:center;
          text-decoration:none;
          
        }
        fieldset{
          text-decoration:none;
          text-align:center;
        }
        .scroller_content{
          padding-block: 1rem;
          display:flex;
          flex-wrap:wrap ;
          gap:1rem;
          text-align:center ; 
        }
        .scroller[data-animated="true"]{
          overflow:hidden ;
          -webkit-mask :linear-gradient(100deg ,transparent,rgba(196, 151, 3, 0.918) 20%,rgba(196, 151, 3, 0.918) 80%,transparent);
          mask: linear-gradient(100deg ,transparent,rgba(196, 151, 3, 0.918) 20%,rgba(196, 151, 3, 0.918) 80%,transparent);
        }
        .scroller[data-animated="true"] .scroller_content{
          width: max-content;
          flex-wrap: nowrap;
          animation: scroll 20s linear infinite;
          scroll-behavior:smooth;
        } 
        @keyframes scroll{
          to{
            transform : translate(-49%);
          }
        }
        li{
          display:inline; 
        }
        .l{
          text-align:center ;
        }
                                            /* F O O T E R */
        .contact{
          flex-direction:column;
        }
        footer{
          display:flex;
          justify-content: center;
        }

        .footer{
          display:flex;
          flex-direction: row;
          width: 100%;
          justify-content: center;
          align-items: center;
          padding-top: 5%;
          padding-bottom:5%;
        }
        .footer a{
          display:flex;
          width: 5%;
          align-items: center;
          justify-content: center;
          text-align: center;
          position: relative;
          color: rgb(184, 150, 41);
        }
        .i{
          text-align: center;
          width:50px;
          height: 50px;
          color: rgb(184, 150, 41);
        }i:hover{
          color:rgb(29, 87, 74);
        }

        @media only  screen and (max-width: 860px){
          .footer a{
              display:flex;
              width: 15%;
          }
        }

    </style>
  </head>
  <body>
    <section class="nav">
      <div class="container1">
        <div class="menu" onclick="myFunction(this)" id="menu">
          <div class="bar">
            <div class="bar1" id="bar1"></div>
            <div class="bar2" id="bar2"></div>
            <div class="bar3" id="bar3"></div>
          </div>
        </div>
      </div>
      <div class="name">
        <h2 class="n">VISHNU V</h2>
      </div>
      <nav class="mainnav" id="nav">
        <a href="#">Home</a>
        <a href="#skills">Skills</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </nav>
      <div class="mode">
        <a onclick="mode()"><svg xmlns="http://www.w3.org/2000/svg"  fill="currentColor" class="bi bi-brightness-high" viewBox="0 0 16 16">
          <path d="M8 11a3 3 0 1 1 0-6 3 3 0 0 1 0 6m0 1a4 4 0 1 0 0-8 4 4 0 0 0 0 8M8 0a.5.5 0 0 1 .5.5v2a.5.5 0 0 1-1 0v-2A.5.5 0 0 1 8 0m0 13a.5.5 0 0 1 .5.5v2a.5.5 0 0 1-1 0v-2A.5.5 0 0 1 8 13m8-5a.5.5 0 0 1-.5.5h-2a.5.5 0 0 1 0-1h2a.5.5 0 0 1 .5.5M3 8a.5.5 0 0 1-.5.5h-2a.5.5 0 0 1 0-1h2A.5.5 0 0 1 3 8m10.657-5.657a.5.5 0 0 1 0 .707l-1.414 1.415a.5.5 0 1 1-.707-.708l1.414-1.414a.5.5 0 0 1 .707 0m-9.193 9.193a.5.5 0 0 1 0 .707L3.05 13.657a.5.5 0 0 1-.707-.707l1.414-1.414a.5.5 0 0 1 .707 0m9.193 2.121a.5.5 0 0 1-.707 0l-1.414-1.414a.5.5 0 0 1 .707-.707l1.414 1.414a.5.5 0 0 1 0 .707M4.464 4.465a.5.5 0 0 1-.707 0L2.343 3.05a.5.5 0 1 1 .707-.707l1.414 1.414a.5.5 0 0 1 0 .708"/>
        </svg></a>
      </div>
    </section>
    <section class="dropdown" id="dropdown">
      <nav class="dropnav" id="dropnav">
        <a href="#" id="bt">Home</a>
        <a href="#skills" id="bt">Skills</a>
        <a href="#about" id="bt">About</a>
        <a href="#contact" id="bt">Contact</a>
      </nav>
    </section>
    <section class="intro">
      <div class="container">
        <div class="l">Introduction</div>
          <div class="mar">
              <p class="content">&nbsp;&nbsp;&nbsp;Greetings , I am a seasoned artisan in the realm of Computer Science and Engineering,
                  weaving intricate tapestries of code and technological marvels . Possessing a bouquet of skills in software alchemy,my 
                  unwavering commitment to excellence propels me towards orchestrating innovation and elevating the landscape of Computer Science and Engineering. 
              </p>
        </div>
      </div>
    </section >
    <section class="skills" id="skills">
        <div class="l">Skills</div>
        <div class="container">
          <div class="scroller" data-animated="true">
            <div class="scroller_content">
              <li><div><img src="../src/lib/assets/html.png" width="85" height="90" alt="html"/></div> HTML</li>
              <li><div><img src="../src/lib/assets/css.png" width="85" height="90" alt="js"></div>CSS</li>
              <li><div><img src="../src/lib/assets/js.png" width="87" height="91" alt="js"></div>  JS</li>
              <li><div><img src="../src/lib/assets/python.png" width="100" height="90" alt="" srcset=""></div> Python</li>
              <li><div><img src="../src/lib/assets/django.png" width="90" height="90" alt="" srcset=""></div>DJango</li>
              <li><div><img src="../src/lib/assets/c.png" width="85" height="90" alt="" srcset=""></div>C</li>
              <li><div><img src="../src/lib/assets/ps.png" width="85" height="90" alt="" srcset=""></div>Photoshop</li>
              <li><div><img src="../src/lib/assets/java.png" width="85" height="90" alt="" srcset=""></div>Java</li>
              <li><div><img src="../src/lib/assets/figma.png" width="85" height="90" alt="" srcset=""></div>Figma</li>
              <li><div><img src="../src/lib/assets/git.png" width="85" height="85" alt="" srcset=""></div>git</li>
              <li><div><img src="../src/lib/assets/github.png" width="85" height="90" alt="" srcset=""></div>Github</li>
              <li><div><img src="../src/lib/assets/flickr.png" width="85" height="90" alt="" srcset=""></div>Flickr</li>
              <li><div><img src="../src/lib/assets/replit.png" width="85" height="90" alt="" srcset=""></div>Replit</li>
              <li><div><img src="../src/lib/assets/gimp.png" width="85" height="90" alt="" srcset=""></div>Gimp</li>
            </div>
          </div>
        </div>
    </section>
     <section class="Education" id="edu">
      <div class="container">
          <div class="l">Education</div>
          <div class="mar">
              <p class="content"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I hold a B.Tech in Computer Science, wielding a proficiency in diverse programming languages
                  and methodologies. My academic voyage has been enriched by a project centered on the creation of a Civil Plan Generator, showcasing my
                    prowess in algorithmic design and software architecture.<br>Currently, my endeavors extend into the realm of cutting-edge 
                    technology, where I am immersed in the development of a project focused on Deep Fake Detection using AI. 
                    This venture epitomizes my dedication to harnessing artificial intelligence for ethical and security-driven applications.
                    As a dynamic and forward-thinking engineer, I am driven to contribute innovative solutions to the ever-evolving landscape
                    of computer science.
              </p>
          </div>
      </div>
    </section> 
     <section class="Experience" id="exp">
      <div class="container">
          <div class="l">Experinece</div>
          <div class="mar">
              <p class="content"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I hold a B.Tech in Computer Science, wielding a proficiency in diverse programming languages
                  and methodologies. My academic voyage has been enriched by a project centered on the creation of a Civil Plan Generator, showcasing my
                    prowess in algorithmic design and software architecture.<br>Currently, my endeavors extend into the realm of cutting-edge 
                    technology, where I am immersed in the development of a project focused on Deep Fake Detection using AI. 
                    This venture epitomizes my dedication to harnessing artificial intelligence for ethical and security-driven applications.
                    As a dynamic and forward-thinking engineer, I am driven to contribute innovative solutions to the ever-evolving landscape
                    of computer science.
              </p>
          </div>
      </div>
    </section> 
    <section class="About" id="about">
      <div class="container">
          <div class="l">About Me</div>
          <div class="mar">
              <p class="content"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I hold a B.Tech in Computer Science, wielding a proficiency in diverse programming languages
                  and methodologies. My academic voyage has been enriched by a project centered on the creation of a Civil Plan Generator, showcasing my
                    prowess in algorithmic design and software architecture.<br>Currently, my endeavors extend into the realm of cutting-edge 
                    technology, where I am immersed in the development of a project focused on Deep Fake Detection using AI. 
                    This venture epitomizes my dedication to harnessing artificial intelligence for ethical and security-driven applications.
                    As a dynamic and forward-thinking engineer, I am driven to contribute innovative solutions to the ever-evolving landscape
                    of computer science.
              </p>
          </div>
      </div>
    </section> 
    <footer class="contact" id="contact">
      <div class="l">Contact</div>
      <div class="footer">
        <a href="https://www.instagram.com/_.vishnu.v._/" target="_blank"><i class="bi bi-instagram"></i></a>
        <a href="https://github.com/VISHNU02V" target="_blank"><i class="bi bi-github"></i></a>
        <a href="https://twitter.com/VishnuV64845443" target="_blank"><i class="bi bi-twitter-x"></i></a>
        <a href="http://www.linkedin.com/in/vishnu02v" target="_blank"><i class="bi bi-linkedin"></i></a>
      </div>
    </footer>
    <script>
        function myFunction(x) {
            if (x.classList.toggle("change")){
                document.getElementById('dropdown').style.display='flex';
                document.getElementById('dropdown').style.justifyContent='center';
                document.getElementById('dropdown').style.position='fixed';
                document.getElementById('dropdown').style.top='40px';
                document.getElementById('dropdown').style.height='100%';
                document.getElementById('dropdown').style.width='100%';
                document.getElementById('dropdown').style.zIndex='1000';
                document.getElementById('dropdown').style.backdropFilter='10px';
                
                document.getElementById('bt').addEventListener('click',function(){
                  document.getElementById('dropdown').style.display='none';
                  
                });
            } 
            else{
                document.getElementById('dropdown').style.display='none';
            }
        }
        function mode() {
            var element = document.body;
            element.classList.toggle("dark-mode");
        }
        const scrollers = document.querySelectorAll(".scroller");
        if(!window.matchMedia("(prefers-reduced-motion: reduce)").matches) {
          addAnimation();
        }
        function addAnimation() {
            scrollers.forEach((scroller) => {
              scroller.setAttribute("data-animated",true);

              const scrollerContent = scroller.querySelector(".scroller_content");
              const scrollerCon = Array.from(scrollerContent.children);

              scrollerCon.forEach((item) => {
                const duplicatedItem = item.cloneNode(true);
                duplicatedItem.setAttribute("aria-hidden",true);
                scrollerContent.appendChild(duplicatedItem);
              });
             
            });
        }

    </script>
  </body>
</html>