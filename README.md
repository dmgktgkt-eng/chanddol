# 급식대장의 동작분석

체육 수업용 자세 분석·평가 웹앱입니다. 학생이 동작을 촬영하거나 영상을 올리면 기준 자세와 비교해 일치율(%), 항목별 일치 여부, 고칠 점을 알려 줍니다.

- 11개 종목 47개 동작, 측면·정면 촬영 기준
- 영상은 기기 안에서만 분석되고 서버로 전송·저장되지 않습니다 (MoveNet + TensorFlow.js)

## 파일 구성

| 경로 | 내용 |
| --- | --- |
| `index.html` | 앱 전체(화면·채점 로직) |
| `model/` | 자세 인식 모델(MoveNet Thunder·Lightning) |
| `rubric.pdf` | 평가 기준표(다운로드용) |
| `.nojekyll` | GitHub Pages가 파일을 그대로 서비스하도록 설정 |

## 배포 (GitHub Pages)

1. 저장소 **Settings → Pages**
2. **Source: Deploy from a branch**, **Branch: `main` / `(root)`** 선택 후 Save
3. 1~2분 뒤 `https://dmgktgkt-eng.github.io/chanddol/` 에서 열립니다

카메라 촬영은 HTTPS에서만 동작하므로 GitHub Pages 주소(https)로 접속하세요.

## 라이선스 표기

자세 인식: MoveNet (Google, Apache-2.0) · TensorFlow.js
