__HTML Code:__

  _tooltip from top:_
  
          <button>
            Click
            <span>My Awesome Tooltip</span>
          </button>



 _tooltip from bootom:_

          <button data-position="bottom">
            Click
            <span>My Awesome Tooltip</span>
          </button>

__CSS Code:__

        * {
          box-sizing: border-box;
          padding: 0;
          margin: 0;
        }
        body {
          font-family: Arial, Tahoma;
        }
        button {
          background-color: #eee;
          margin: 100px auto;
          padding: 10px 20px;
          display: block;
          font-size: 40px;
          border: none;
          position: relative;
          cursor: pointer;
          overflow: hidden;
        }
        button:focus {
          outline: none;
        }
        button span {
          background-color: #333;
          color: #fff;
          position: absolute;
          left: 50%;
          transform: translateX(-50%);
          font-size: 18px;
          min-width: 240px;
          padding: 10px 15px;
          top: -60px;
          transition: 0.5s;
          opacity: 0;
        }
        button span:before {
          content: "";
          position: absolute;
          bottom: -20px;
          left: 50%;
          transform: translateX(-50%);
          border-style: solid;
          border-width: 10px;
          border-color: #333 transparent transparent;
        }
        button:hover {
          overflow: visible;
        }
        button:hover span {
          opacity: 1;
        }
        [data-position="bottom"] span {
          top: auto;
          bottom: -60px;
        }
        [data-position="bottom"] span:before {
          bottom: auto;
          top: -20px;
          border-color: transparent transparent #333;
        }
