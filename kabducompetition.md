  <!DOCTYPE html>
  <html lang="en">

  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple HTML HomePage</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <style>
      @import url('https://fonts.googleapis.com/css2?family=Sriracha&display=swap');

      body {
        margin: 0;
        box-sizing: border-box;
      }

      /* CSS for header */
      .header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: #f5f5f5;
        position: -webkit-header;
        position:sticky;
        height: 100px;
      top:0;
      width:100%;
      z-index:100;
      }

      .kabdu {
        font-size: 25px;
        font-family: 'Sriracha', cursive;
        color: #000;
        text-decoration: none;
        margin-left: 50px;
      }

      .nav-items {
        display: flex;
        justify-content: space-around;
        align-items: center;
        background-color: #f5f5f5;
        
      }

      .nav-items a {
        text-decoration: none;
        color: #000;
        padding: 35px 20px;
      }

      /* CSS for main element */
      .intro {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 100%;
        height: 610px;
        background: linear-gradient(to bottom, rgba(0.5, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.5) 100%), url("https://images.unsplash.com/photo-1587620962725-abab7fe55159?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1031&q=80");
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
      }

      .intro h1 {
        font-family: sans-serif;
        font-size: 60px;
        color: #fff;
        font-weight: bold;
        text-transform: uppercase;
        margin: 0;
      }

      .intro p {
        font-size: 20px;
        color: #d1d1d1;
        text-transform: uppercase;
        margin: 20px 0;
      }

      .intro button {
        background-color: #5edaf0;
        color: #000;
        padding: 10px 25px;
        border: none;
        border-radius: 5px;
        font-size: 20px;
        font-weight: bold;
        cursor: pointer;
        box-shadow: 0px 0px 20px rgba(255, 255, 255, 0.4)
      }

      .achievements {
        display: flex;
        justify-content: space-around;
        align-items: center;
        padding: 40px 80px;
      }

      .achievements .work {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        padding: 0 40px;
      }

      .achievements .work i {
        width: fit-content;
        font-size: 50px;
        color: #333333;
        border-radius: 50%;
        border: 2px solid #333333;
        padding: 12px;
      }

      .achievements .work .work-heading {
        font-size: 20px;
        color: #333333;
        text-transform: uppercase;
        margin: 10px 0;
      }

      .achievements .work .work-text {
        font-size: 15px;
        color: #585858;
        margin: 10px 0;
      }

      .about-me {
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 40px 80px;
        border-top: 2px solid #eeeeee;
      }

      .flashcards {
  display: flex;
  padding: 3rem;
  overflow-x: scroll;
}
.flashcards::-webkit-scrollbar {
  width: 10px;
  height: 10px;
}
.flashcards::-webkit-scrollbar-thumb {
  background: #201c29;
  border-radius: 10px;
  box-shadow: inset 2px 2px 2px hsla(0, 0%, 100%, 0.25),
    inset -2px -2px 2px rgba(0, 0, 0, 0.25);
}


      .about-me img {
        width: 500px;
        max-width: 100%;
        height: auto;
        border-radius: 10px;
      }

      .flashcards {
        background-color: #c7d5dc;
        padding-left: 350px;
      }
      .orange {
        background-color: orange;
        width: 200px;
        height: 300px;
        border-radius: 15px;
        z-index:2;
position:absolute:
      }
      .card:hover {
  transform: translateY(-1rem);
}
.card:focus-within ~ .card,
.card:hover ~ .card {
  transform: translateX(130px);
}
.card:not(:first-child) {
  margin-left: -130px;
}

      .test {
        margin-left:50px;
        background-color: whitesmoke;
        width: 100px;
        height: 35px;
        border-radius: 15px;
      }

    .green{
        background-color: greenyellow;
        width: 200px;
        height: 300px;
        border-radius: 15px;

}

.headingorange {
  background-color: white;
  border-radius: 15px;
  z-index: -1;
}

.black {
        background-color: black;
        width: 200px;
        height: 300px;
        border-radius: 15px;
}


      .about-me-text h2 {
        font-size: 30px;
        color: #333333;
        text-transform: uppercase;
        margin: 0;
      }

      .about-me-text p {
        font-size: 15px;
        color: #585858;
        margin: 10px 0;
      }

      /* CSS for footer */
      .footer {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: #302f49;
        padding: 40px 80px;
      }

      .footer .copy {
        color: #fff;
      }

      .bottom-links {
        display: flex;
        justify-content: space-around;
        align-items: center;
        padding: 40px 0;
      }

      .bottom-links .links {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        padding: 0 40px;
      }

      .bottom-links .links span {
        font-size: 20px;
        color: #fff;
        text-transform: uppercase;
        margin: 10px 0;
      }

      .bottom-links .links a {
        text-decoration: none;
        color: #a1a1a1;
        padding: 10px 20px;
      }

      .something {
        margin-top: 10px;
        z-index: -1;
      }
      .card {
  height: 350px;
  width: 400px;
  min-width: 250px;
  padding: 1.5rem;
  border-radius: 16px;
  background: #17141d;
  box-shadow: -1rem 0 3rem #000;
  display: flex;
  flex-direction: column;
  transition: 0.2s;
  margin: 0;
  scroll-snap-align: start;
  clear: both;
  position: relative;
}
.textgreen :hover{
   background: linear-gradient(90deg, #ff8a00, #e52e71);
  text-shadow: none;
  -webkit-text-fill-color: transparent;
  -webkit-background-clip: text;
  background-clip: text;
}
#learn {
  border-radius: 1px;
  border: solid;
  border-color: white;
  color: white;
  background-color: #17141d;
}

#learn :hover {
  border: solid;
  background-color: white;
  color: #17141d;
  transition: 0.5s;
}
    </style>
  </head>

  <body>
    <main>
      <div class="intro">
        <h1>A Web Developer</h1>
        <p>I am a web developer and I love to create websites.</p>
        <button>Learn More</button>
      </div>
       <header class="header">
      <a href="#" class="logo"><p class="kabdu" style="margin-bottom: 20px; margin-left: 100px;">Kabdu</p></a>
      <nav class="nav-items">
        <a href="#">Home</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
      </nav>
    </header>

      <div class="achievements">
        <div class="work">
          <i class="fas fa-atom"></i>
          <p class="work-heading">Projects</p>
          <p class="work-text">I have worked on many projects and I am very proud of them. I am a very good developer and I am always looking for new projects.</p>
        </div>
        <div class="work">
          <i class="fas fa-skiing"></i>
          <p class="work-heading">Skills</p>
          <p class="work-text">I have a lot of skills and I am very good at them. I am very good at programming and I am always looking for new skills.</p>
        </div>
        <div class="work">
          <i class="fas fa-ethernet"></i>
          <p class="work-heading">Network</p>
          <p class="work-text">I have a lot of network skills and I am very good at them. I am very good at networking and I am always looking for new network skills.</p>
        </div>
      </div>
      <div class="flashcards">
        <br>
        <div class="something">
        </div>
        <table>
        <tr>  
          <th>
        <div class="card">
          <p>m has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap</p>
                </div>
         </th>
         <th>
        <div class="card">
          
            <div class="textgreen"><h2>Green</h2></div>
          
        </div>
      </th>
      <th>
          <th>
        <div class="card">
          
            <h2>Green</h2>
                    <button id="learn">
          Learn More
        </button>
          
        </div>
      </th>
      <th>
          <th>
        <div class="card">
          
            <h2>Green</h2>
          
        </div>

      </th>
      <th>
          <th>
        <div class="card">
          
            <h2>Green</h2>
          
        </div>
      </th>
      <th>
          <th>
        <div class="card">
          
            <h2>Green</h2>
          
        </div>
      </th>
      <th>
        <div class="card">
       
          <h2>
            Black
          </h2>
          
        </div>
      </th>
            </tr>
    </table>

      </div>


      <div class="about-me">
        <div class="about-me-text">
          <h2>About Me</h2>
          <p>I am a web developer and I love to create websites. I am a very good developer and I am always looking for new projects. I am a very good developer and I am always looking for new projects.</p>
        </div>
        <img src="https://images.unsplash.com/photo-1596495578065-6e0763fa1178?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=871&q=80" alt="me">
      </div>
    </main>

    <footer class="footer">
      <div class="copy">&copy; 2022 Developer</div>
      <div class="bottom-links">
        <div class="links">
          <span>More Info</span>
          <a href="#">Home</a>
          <a href="#">About</a>
          <a href="#">Contact</a>
        </div>
        <div class="links">
          <span>Social Links</span>
          <a href="#"><i class="fab fa-facebook"></i></a>
          <a href="#"><i class="fab fa-twitter"></i></a>
          <a href="#"><i class="fab fa-instagram"></i></a>
        </div>
      </div>
    </footer>
  </body>

  </html>
