
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>대전 청년 로컬 라이프 플랫폼</title>
    <!-- 개발자 느낌의 깔끔한 폰트 (JetBrains Mono / Fira Code 계열 폰트 적용) -->
    <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;500;700&family=Noto+Sans+KR:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-color: #f7f5fa;
            --card-bg: #FFFFFF;
            --primary-color: #B58AE6;
            --primary-light: #f3effc;
            --text-main: #1a1a1a;
            --text-muted: #555555;
            --border-color: #e5def5;
            --code-font: 'Fira Code', monospace;
        }

        body {
            font-family: 'Noto Sans KR', -apple-system, BlinkMacSystemFont, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }

        header {
            background: linear-gradient(135deg, #cbb5f0, var(--primary-color));
            color: white;
            text-align: center;
            padding: 60px 20px;
        }

        header h1 {
            margin: 0;
            font-size: 2.6rem;
            font-weight: 700;
            letter-spacing: -0.5px;
            font-family: var(--code-font); //
        }

        header p {
            margin-top: 10px;
            font-size: 1.1rem;
            opacity: 0.95;
            font-family: var(--code-font);
        }

        .container {
            max-width: 900px;
            margin: -30px auto 50px auto;
            padding: 0 20px;
        }

        .card {
            background-color: var(--card-bg);
            border-radius: 16px;
            box-shadow: 0 8px 24px rgba(181, 138, 230, 0.12);
            padding: 30px;
            margin-bottom: 25px;
            border: 1px solid var(--border-color);
        }

        h2 {
            color: #7b4fc7;
            font-size: 1.4rem;
            border-bottom: 2px solid var(--primary-light);
            padding-bottom: 10px;
            margin-top: 0;
            font-family: var(--code-font);
        }

        ul {
            padding-left: 20px;
        }

        li {
            margin-bottom: 10px;
        }

        /* Codex / Terminal 스타일의 하이라이트 박스 */
        .highlight-box {
            background-color: #1e1e2e; 
            color: #cdd6f4
            border-left: 4px solid var(--primary-color);
            padding: 15px 20px;
            border-radius: 8px;
            margin: 15px 0;
            font-family: var(--code-font);
            font-size: 0.95rem;
            box-shadow: inset 0 2px 4px rgba(0,0,0,0.2);
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 15px;
        }

        .grid-item {
            background-color: #faf8fd;
            border: 1px solid var(--border-color);
            border-radius: 12px;
            padding: 20px;
        }

        .grid-item h3 {
            margin-top: 0;
            color: #7b4fc7;
            font-size: 1.1rem;
            font-family: var(--code-font);
        }

        /* 이미지 쇼케이스 스타일 */
        .image-showcase {
            margin-top: 20px;
            background: #faf8fd;
            border: 2px solid var(--border-color);
            border-radius: 12px;
            padding: 20px;
            text-align: center;
        }

        .image-showcase img {
            width: 100%;
            max-width: 100%;
            height: auto;
            border-radius: 8px;
            box-shadow: 0 4px 12px rgba(0,0,0,0.08);
            margin-bottom: 15px;
        }

        .image-showcase p {
            margin: 0;
            color: var(--text-muted);
            font-size: 0.95rem;
            text-align: left;
        }

        .image-showcase h4 {
            margin: 0 0 8px 0;
            color: #7b4fc7;
            font-size: 1.2rem;
            text-align: left;
            font-family: var(--code-font);
        }

        footer {
            text-align: center;
            padding: 30px;
            color: var(--text-muted);
            font-size: 0.85rem;
            font-family: var(--code-font);
        }
    </style>
</head>
<body>

    <header>
        <h1>분류</h1>
        <p>생활</p>
    </header>

    <div class="container">
        <!-- 기획 배경 -->
        <div class=card">
            <h2>기획 배경 (Background)</h2>
            <p>대전 동구 로컬 프로그램에 참여하며 청년들이 경험할 수 있는 공간과 콘텐츠가 있음에도, 정보가 분산되어 있다는 점을 발견했습니다. 단순한 관광이 아닌, 청년의 관점에서 지역의 공간과 사람, 체험을 연결하는 서비스를 기획했습니다[cite: 1].</p>
            <div class="highlight-box">
                &gt; target_flow: [ 지역 발견 ➔ 방문 체험 ➔ 관계 형성 ➔ 지역 활동 ➔ 대전 정착 ]
            </div>
        </div>

        <!-- 핵심 차별점 -->
        <div class="card">
            <h2>✨ 주요 서비스 및 차별점 (Features)</h2>
            <div class="grid">
                <div class="grid-item">
                    <h3> 캐릭터 가이드</h3>
                    <p>작은 로봇 캐릭터가 철길마을, 원동, 청년공간 등 핫플레이스를 친근하게 안내합니다.</p>
                </div>
                <div class="grid-item">
                    <h3> 온·오프라인 연계</h3>
                    <p>콘텐츠 관람에서 끝나지 않고, QR을 통해 실제 공간의 체험 프로그램으로 연결합니다.</p>
                </div>
                <div class="grid-item">
                    <h3> 웰컴 키트</h3>
                    <p>대전에 정착하는 청년을 위한 실물 웰컴 키트(수건, 가글, 충전기, 독서대 등)를 제공합니다.</p>
                </div>
            </div>
        </div>

        <!-- 사업화 단계 및 캐릭터 샘플 (이미지 첨부) -->
        <div class="card">
            <h2> 사업화 단계 및 캐릭터 굿즈 샘플 (Roadmap)</h2>
            <ul>
                <li><strong>1단계 (디자인 및 도안):</strong> 생활 속 캐릭터 제작 및 웰컴키트 도안 기획</li>
                <li><strong>2단계 (인프라 활용):</strong> 대전 동구 인쇄거리 및 지역 업체와 연계한 굿즈·카드 제작</li>
                <li><strong>3단계 (샘플링 및 검증):</strong> 지역 공방·철공소 협력 샘플 제작 및 청년 소비 대상 피드백 수렴<img src="sample1.png" alt></li>
            </ul>

            <!-- 이미지 파일명 sample.png 연동 -->
            <div class="image-showcase">
                <img src="sample.png" alt="사부작 자취 캐릭터 굿즈 및 커피·쿠키 패키지 샘플">
                <h4> 사부작 자취 캐릭터 굿즈 및 패키지 시제품</h4>
                <p>로봇 캐릭터와 연계된 드립백 커피, 보라색 너트 쿠키 패키지, 브랜드 카드 및 머그컵으로 구성된 웰컴 키트 샘플입니다. 지역 인쇄거리 및 공방과 협력하여 제작됩니다.</p>
            </div>
        </div>
    </div>

    <footer>
    </footer>

</body>
</html>
