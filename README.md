# TEAMPLAYER 공식 웹사이트

## 프로젝트 개요
㈜팀플레이어 공식 웹사이트 - https://www.teamplayer.co.kr

## 기술 스택
- Next.js 14
- React 18
- HTML5/CSS3
- AWS S3 + CloudFront

## 주요 기능
- 반응형 웹 디자인
- 다국어 지원 (한국어, 영어, 일본어)
- 다크 모드
- 상담 요청 폼 (개발 중)

## 배포 이력

### 2024-09-17 v1.1.0
- 회사명 브랜딩 업데이트 (TEAMPLEAN → TEAMPLAYER)
- 로고 파일 교체 (teamplayer-logo.png)
- 메타데이터 및 SEO 정보 수정
- CloudFront 캐시 최적화

### 2024-08-13 v1.0.0
- 초기 사이트 배포
- 회사 소개, 제품, 서비스 페이지 구현
- IMSMS 제품 소개
- 파트너십 및 글로벌 네트워크 섹션

## 배포 방법

### S3 배포
```bash
# S3 동기화
aws s3 sync . s3://teamplayer-website/ --exclude ".git/*" --exclude ".DS_Store" --exclude "_next/*" --delete

# CloudFront 캐시 무효화
aws cloudfront create-invalidation --distribution-id E2P9KZWX3A6ET0 --paths "/*"
```

## 디렉토리 구조
```
├── index.html              # 메인 페이지
├── about/                  # 회사 소개
├── products/               # 제품 소개
├── technology/             # 기술 소개
├── partnerships/           # 파트너십
├── support/                # 지원
├── mypage/                 # 마이페이지
├── 404/                    # 404 페이지
├── _next/                  # Next.js 정적 자산
├── teamplayer-logo.png     # 회사 로고
└── favicon.ico             # 파비콘
```

## 연락처
- 대표: 김원철
- 이메일: charles@teamplayer.co.kr
- 전화: 1522-8061 / 070-8080-0511
- 주소: 경기도 용인시 기흥구 동백로 22

## 라이선스
Copyright © 2024 TEAMPLAYER Inc. All rights reserved.