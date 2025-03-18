<div class="card1">
    <div class="content">
      <h1><slot name="title"></slot></h1>
      <p class="para"><slot name="subtitle"></slot></p>
    </div>
  </div>
  
  <style>
    .card1 {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      width: 320px;
      border-radius: 10px;
      line-height: 1.6;
      transition: all 0.48s cubic-bezier(0.23, 1, 0.32, 1);
      font-family: 'Kanit';
    }

     img {
      margin-bottom: 30px;
     }

    h1 {
      font-size: 24px;
      margin-bottom: 0px;
    }
  
    .content {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      gap: 12px;
      padding: 36px;
      border-radius: 20px;
      color: #ffffff;
      overflow: hidden;
      background:rgba(3, 70, 148, 1);
      transition: all 0.48s cubic-bezier(0.23, 1, 0.32, 1);
    }
  
    .content::before {
      position: absolute;
      content: "";
      top: -4%;
      left: 50%;
      width: 90%;
      height: 90%;
      transform: translate(-50%);
      background: #ced8ff;
      z-index: -1;
      transform-origin: bottom;
  
      border-radius: inherit;
      transition: all 0.48s cubic-bezier(0.23, 1, 0.32, 1);
    }
  
    .content::after {
      position: absolute;
      content: "";
      top: -8%;
      left: 50%;
      width: 80%;
      height: 80%;
      transform: translate(-50%);
      background: #e7ecff;
      z-index: -2;
      transform-origin: bottom;
      border-radius: inherit;
      transition: all 0.48s cubic-bezier(0.23, 1, 0.32, 1);
    }
  
    .content .para {
      z-index: 1;
      opacity: 1;
      font-size: 16px;
      transition: all 0.48s cubic-bezier(0.23, 1, 0.32, 1);
      margin-bottom: 0px;
    }

  
    .card1:hover {
      transform: translate(0px, -16px);
    }
  
    .card1:hover .content::before {
      rotate: -8deg;
      top: 0;
      width: 100%;
      height: 100%;
    }
  
    .card1:hover .content::after {
      rotate: 8deg;
      top: 0;
      width: 100%;
      height: 100%;
    }
  </style>
  