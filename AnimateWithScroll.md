__HTML Code:__

        <section class="one">Section One</section>
        <section class="two">Section Two</section>
        <section class="three">
          <div class="skills">
            <h3>HTML</h3>
            <div class="progress">
              <span style="width: 0" data-width="80%"></span>
            </div>
            <h3>CSS</h3>
            <div class="progress">
              <span style="width: 0" data-width="90%"></span>
            </div>
            <h3>Scala</h3>
            <div class="progress">
              <span style="width: 0" data-width="50%"></span>
            </div>
          </div>
        </section>
        <section class="four">Section Four</section>


__CSS Code:__

        * {
          box-sizing: border-box;
        }
        body {
          font-family: "Trebuchet MS", "Lucida Sans Unicode", sans-serif;
          margin: 0;
        }
        section {
          min-height: 100vh;
          display: flex;
          justify-content: center;
          align-items: center;
        }
        section:first-child {
          background-color: #aaa;
        }
        section:nth-child(2) {
          background-color: #bbb;
        }
        section:nth-child(3) {
          background-color: #ccc;
        }
        section:last-of-type {
          background-color: #eee;
        }
        .progress {
          position: relative;
          width: 500px;
          height: 30px;
          background-color: white;
          margin: 10px;
        }
        .progress span {
          position: absolute;
          left: 0;
          top: 0;
          height: 100%;
          background-color: indianred;
          transition: width 0.3s linear;
        }

__JS Code:__


      let section = document.querySelector(".three");
      let spans = document.querySelectorAll(".progress span");

      window.onscroll = function () {
        if (window.scrollY >= section.offsetTop) {
          console.log("Reached Section Three");
          spans.forEach((span) => {
            span.style.width = span.dataset.width;
          });
        }
      };
