<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 220" width="100%">
  <defs>
    <!-- 폰트 등록 -->
    <style>
      @font-face {
        font-family: 'SchoolSafetyRoundedSmile';
        src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/2408-5@1.0/HakgyoansimDunggeunmisoTTF-B.woff2') format('woff2');
        font-weight: 700;
        font-display: swap;
      }

      /* 무한으로 흐려졌다 밝아지는 반짝반짝 애니메이션 효과 */
      @keyframes blink {
        0% { opacity: 0.3; text-shadow: 0 0 10px rgba(255,255,255,0.3); }
        50% { opacity: 1.0; text-shadow: 0 0 25px rgba(255,255,255,0.9), 0 0 40px rgba(255,255,255,0.6); }
        100% { opacity: 0.3; text-shadow: 0 0 10px rgba(255,255,255,0.3); }
      }

      .animated-text {
        font-family: 'SchoolSafetyRoundedSmile', sans-serif;
        font-weight: 700;
        font-size: 55px; /* 글자 크기 더 시원하게 키움 */
        fill: #ffffff;
        animation: blink 2.5s infinite ease-in-out; /* 2.5초 주기로 무한 반복 */
      }
    </style>

    <!-- 배경에 들어갈 물결 모양 곡선 정의 -->
    <path id="wave" d="M 0,0 L 0,190 Q 250,160 500,190 T 1000,190 L 1000,0 Z" />
  </defs>

  <!-- 원하셨던 연두색 배경 (#2ecc71) -->
  <use href="#wave" fill="#2ecc71" />
  <use href="#wave" fill="#2ecc71" opacity="0.3" transform="scale(1, 1.05)" />

  <!-- 대문자 + 정중앙 배치 + 반짝이 효과 텍스트 -->
  <text x="50%" y="48%" dominant-baseline="middle" text-anchor="middle" class="animated-text">
    YOUNG HYEN'S GITHUB
  </text>
</svg>
