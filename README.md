##日常积累
### 
 1).h5分享：
 
  ```
  // 另外使用meta同样可以达到该接口的作用
  <meta itemprop="name" content="这是分享的标题"/>
  <meta itemprop="image" content="http://ws234.com/content/templates/emlog_dux/images/fxlogo.png" />
  <meta name="description" itemprop="description" content="这是要分享的内容" />
  ```
 2).有趣的按钮
 ```
  css:
  <style>
    .btn{
          border: 1px solid #FFF;
          color: #FFF;
          padding: 10px 20px;
          margin:140px;
          text-decoration: none;
          display: inline-block;
          border-radius: 5px;
          /* overflow: hidden; */
          position: relative;
          background: transparent;
      }
      .btn:before{
         content: '';
         display: inline-block;
         transform: translate(-50%, -50%);
         background: #FFF;
         color: #FFF;
         border-radius: 50%;
         width: 0;
         position: absolute;
         top: 50%;
         left:50%;
         transition: all .5s;
         z-index: -1;
        }
      .btn:hover{
        color: orange;
      }
      .btn:hover:before{
         width: 105%;
         padding-top: 105%;
      }
  </style>
  
  
  html:
  <a class="btn">
    按钮文字
  </a>
``` 
 