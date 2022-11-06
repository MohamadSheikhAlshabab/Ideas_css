__HTML Code:__

      <div class="product">
        <h2 class="title">Product Title</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores,
          nisi id earum corrupti neque sunt ea molestiae
          iusto. Quasi fugit cum optio aliquam corporis impedit
          quia numquam fuga error laudantium.
        </p>
      </div>
      
      
__CSS Code:__

        * {
            box-sizing: border-box;
            padding: 0;
            margin: 0;
          }
          body {
            font-family: Arial, Tahoma;
          }
          .product {
            width: 400px;
            margin: 20px auto;
            padding: 20px;
            background-color: #f5f5f5;
            text-align: center;
          }
          .product h2 {
            margin: 0 0 20px;
            background-color: #009688;
            color: #fff;
            padding: 15px;
            width: calc(100% + 80px);
            position: relative;
            left: -40px;
          }
          .product h2:before {
            content: "";
            position: absolute;
            left: 0;
            bottom: -20px;
            border-width: 10px;
            border-color: #02766b #02766b transparent transparent;
            border-style: solid;
          }
          .product h2:after {
            content: "";
            position: absolute;
            right: 0;
            bottom: -20px;
            border-width: 10px;
            border-color: #02766b transparent transparent #02766b;
            border-style: solid;
          }
          .product p {
            line-height: 1.6;
          }