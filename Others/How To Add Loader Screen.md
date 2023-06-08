######## Add inside <head>

  <style>
    :root {
      --loaderbg: rgb(0, 0, 0);
    }

    #loader {
      display: flex;
      justify-content: center;
      align-items: center;
      position: fixed;
      top: 0;
      left: 0;
      z-index: 9999;
      width: 100%;
      height: 100%;
      background-color: var(--loaderbg);
      animation: anim2 1s cubic-bezier(0.19, 1, 0.22, 1) 15s both;
      text-align: center;

    }

    #wrapperload p {
      font-size: 20px;
      margin-left: 20px;
      margin-right: 20px;
      line-height: 1.5;
    }

    #wrapperload {
      width: 500px;
      height: 100px;
      overflow: hidden;
      background-color: transparent;
    }

    #wrapperload .elem {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 100%;
      height: 100%;
    }

    #wrapperload .elem h3 {
      margin: 0;
    }

    #wrapperload .elem:nth-child(1) {
      animation: anim 2s cubic-bezier(0.19, 1, 0.22, 1) 1s both;
    }

    #wrapperload .elem:nth-child(2) {
      animation: anim 2s cubic-bezier(0.19, 1, 0.22, 1) 3s both;
    }

    #wrapperload .elem:nth-child(3) {
      animation: anim 2s cubic-bezier(0.19, 1, 0.22, 1) 5s both;
    }

    #wrapperload .elem:nth-child(4) {
      animation: anim 2s cubic-bezier(0.19, 1, 0.22, 1) 7s both;
    }

    #wrapperload .elem:nth-child(5) {
      animation: anim 2s cubic-bezier(0.19, 1, 0.22, 1) 9s both;
    }

    #wrapperload .elem:nth-child(6) {
      animation: anim 2s cubic-bezier(0.19, 1, 0.22, 1) 11s both;
    }

    #wrapperload .elem:nth-child(7) {
      animation: anim 2s cubic-bezier(0.19, 1, 0.22, 1) 13s both;
    }

    #wrapperload .elem:nth-child(8) {
      animation: anim 2s cubic-bezier(0.19, 1, 0.22, 1) 15s both;
    }

    @keyframes anim {
      to {
        margin-top: -100px;
      }
    }

    @keyframes anim2 {
      to {
        transform: translateY(-100%);
      }
    }

    @media only screen and (min-width: 768px) {
      #wrapperload p {
        font-size: 40px;
      }

      #wrapperload {
        width: 700px;
        height: 200px;
        overflow: hidden;
        background-color: transparent;
      }

      @keyframes anim {
        to {
          margin-top: -200px;
        }
      }

      @keyframes anim2 {
        to {
          transform: translateY(-200%);
        }
      }
    }

    #main-content {
      display: none;
    }
  </style>

######## Add right after <body> tag starts

   <div id="loader">
    <div id="wrapperload">
      <div class="elem">
        <p style="font-weight: bold; color: #f99c84;">Hey! This Is Not Your Regular Developer!</p>
      </div>
      <div class="elem">
        <p style="font-weight: bold; color: #56adfe;">Lets Explore Something New Today, Together</p>
      </div>
      <div class="elem">
        <p style="font-weight: bold; color: #00ddff;">Enter The World of Relentless Innovation</p>
      </div>
      <div class="elem">
        <p style="font-weight: bold; color: #4848ff;">Unleash The Power of Software Engineering</p>
      </div>
      <div class="elem">
        <p style="font-weight: bold; color: #F2AE36;">Embark on a Journey with a Robotics Enthusiast</p>
      </div>
      <div class="elem">
        <p style="font-weight: bold; color: #ffe227;">Explore The Uncharted Territories of an AI Researcher
        </p>
      </div>
      <div class="elem">
        <p style="font-weight: bold; color: #ff00ff;">This is Eftakhar Ahmed Arnob</p>
      </div>
      <div class="elem">
        <p style="font-weight: bold; color: #E4B286;">And Welcome to my world!
        </p>
      </div>
    </div>
  </div>

//Optional

  <div id="main-content">

####### Add right before </body> ends

 </div>
  <script>
    setTimeout(function () {
      document.getElementById('loader').style.display = 'none';
      document.getElementById('main-content').style.display = 'block';
    }, 15000);
  </script>

//Optional
