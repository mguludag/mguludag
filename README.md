<!--
**mguludag/mguludag** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- ### Hi there 👋
- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

<html>
  <head>
    <meta charset="UTF-8" />
    <link
      href="https://fonts.googleapis.com/css2?family=Nunito:wght@200;300;400;600;700;800;900&family=Pacifico&display=swap"
      rel="stylesheet"
    />
    <style>
      html {
        height: 100%;
      }
      body {
        margin: 0;
        padding: 0;
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        background-color: white;
      }
      #particles-js {
        position: absolute;
        width: 100%;
        height: 100%;
        z-index: -1;
      }
      #app {
        font-family: "Consolas", sans-monospace;
        align-self: center;
        text-align: center;
        color: black;
      }
      #app > .head_one {
        font-size: 48px;
      }
      #app > .head_two {
        font-size: 32px;
      }
      .point {
        font-size: 42px;
        font-family: "Consolas", monospace;
      }
      .point_small {
        font-size: 28px;
        font-family: "Consolas", monospace;
      }
      a {
        color: black;
        text-decoration: none;
      }
    </style>
  </head>

  <body>
    <div id="particles-js"></div>
    <div id="app">
      <div class="head_one" id="head_one"></div>
      <div class="head_two" id="head_two"></div>
    </div>
    <script src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>
    <script src="https://unpkg.com/typewriter-effect@latest/dist/core.js"></script>
    <script type="text/javascript">
      particlesJS("particles-js", {
        particles: {
          number: { value: 80, density: { enable: true, value_area: 800 } },
          color: { value: "#000000" },
          shape: {
            type: "circle",
            stroke: { width: 0, color: "#000000" },
            polygon: { nb_sides: 5 }
          },
          opacity: {
            value: 0.25,
            random: false,
            anim: { enable: false, speed: 1, opacity_min: 0.1, sync: false }
          },
          size: {
            value: 3,
            random: true,
            anim: { enable: false, speed: 40, size_min: 0.1, sync: false }
          },
          line_linked: {
            enable: true,
            distance: 150,
            color: "#000000",
            opacity: 0.3,
            width: 1
          },
          move: {
            enable: true,
            speed: 3,
            direction: "none",
            random: false,
            straight: false,
            out_mode: "out",
            bounce: false,
            attract: { enable: false, rotateX: 600, rotateY: 1200 }
          }
        },
        retina_detect: true
      });
      const typeWriterOne = new Typewriter("#head_one", {
        delay: 20,
        deleteSpeed: 20,
        stringSplitter: true
      });
      const typeWriterTwo = new Typewriter("#head_two", {
        delay: 20,
        deleteSpeed: 20
      });

      typeWriterOne
        .typeString("Hey there, I'm <span class='point'>M. Galib.</span>")
        .pauseFor(2500)
        .deleteAll()
        .typeString("I'm a <span class='point'>Software Engineer</span>")
        .pauseFor(3000)
        .deleteChars(20)
        .typeString(" an <span class='point'>Open Source Enthusiast</span>")
        .pauseFor(3000)
        .deleteAll()
        .typeString("Check out my work!")
        .pauseFor(2500)
        .start();

      typeWriterTwo
        .typeString("Nice to meet you")
        .pauseFor(3500)
        .deleteAll()
        .typeString("C++, Qt, C, MATLAB, Python")
        .pauseFor(2500)
        .deleteAll()
        .typeString("QTextRecognizer, RandomMAC, QImgProc")
        .pauseFor(3000)
        .deleteAll()
        .typeString(
          "Twitter: <span class='point_small'><a href='https://twitter.com/mguludag' target='_blank' >@mguludag</a>.</span>"
        )
        .pauseFor(3500)
        .start();
    </script>
  </body>
</html>
