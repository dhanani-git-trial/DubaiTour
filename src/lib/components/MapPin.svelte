<style>

  .GMAMP-maps-pin-view {
    display: grid;
    grid-template-columns: auto;
    grid-template-rows: 5.5px auto;
    gap: 0px;
    justify-items: center;
    pointer-events: none;
    user-select: none;
    width: 26px;
    height: 38px;
    margin-right: 10px;
  }
  .GMAMP-maps-pin-view svg {
    display: block;
    overflow: visible;
    grid-area: 1;
  }
  .GMAMP-maps-pin-view div {
    grid-area: 2;
    display: flex;
    align-items: center;
    justify-content: center;
    color: rgb(255, 255, 255);
    width: 15px;
    height: 15px;
  }

  .fscode {
    font-size: 12px;
  }
</style>
<div class="GMAMP-maps-pin-view">
  <svg xmlns="http://www.w3.org/2000/svg" width="26px" height="38px" viewBox="0 0 26 37" style="display: block; overflow: visible; grid-area: 1;">
    <defs>
      <filter id="B5FCD016-6025-4355-8692-7387AC810D13">
        <feFlood result="floodFill"></feFlood>
        <feComposite in="floodFill" in2="SourceAlpha" operator="in" result="sourceAlphaFill"></feComposite>
        <feComposite in="sourceAlphaFill" in2="SourceGraphic" operator="in"></feComposite>
      </filter>
    </defs>
    <g fill="none" fill-rule="evenodd" style="pointer-events: auto;">
      <path class="RIFJN-maps-pin-view-border" d="M13 0C5.8175 0 0 5.77328 0 12.9181C0 20.5733 5.59 23.444 9.55499 30.0784C12.09 34.3207 11.3425 37 13 37C14.7225 37 13.975 34.2569 16.445 30.1422C20.085 23.8586 26 20.6052 26 12.9181C26 5.77328 20.1825 0 13 0Z" fill="#fff"></path>
      <path class="RIFvHW-maps-pin-view-background" fill="#1484CD" d="M13.0167 35C12.7836 35 12.7171 34.9346 12.3176 33.725C11.9848 32.6789 11.4854 31.0769 10.1873 29.1154C8.92233 27.1866 7.59085 25.6173 6.32594 24.1135C3.36339 20.5174 1 17.7057 1 12.6385C1.03329 6.19808 6.39251 1 13.0167 1C19.6408 1 25 6.23078 25 12.6385C25 17.7057 22.6699 20.55 19.6741 24.1462C18.4425 25.65 17.1443 27.2193 15.8793 29.1154C14.6144 31.0442 14.0818 32.6135 13.749 33.6596C13.3495 34.9346 13.2497 35 13.0167 35Z"></path>
      <path class="KWCFZI-maps-pin-view-default-glyph" d="M13 18C15.7614 18 18 15.7614 18 13C18 10.2386 15.7614 8 13 8C10.2386 8 8 10.2386 8 13C8 15.7614 10.2386 18 13 18Z" fill="#fff" style="display: none;"></path>
      <image x="50%" y="50%" preserveAspectRatio="xMidYMid meet" width="15px" height="15px" style="transform: translate(-7.5px, -12.5px);" href=""></image>
      <text x="50%" y="50%" text-anchor="middle" style="font-size: 16px; fill: #fff;"></text>
    </g>
  </svg>
  <div>
    <div class="fscode"><slot name="fscode"></slot></div>
  </div>
</div>
