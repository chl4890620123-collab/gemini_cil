# GEMINI Mandates

이 파일은 이 프로젝트에서 Gemini CLI의 행동 지침과 엔지니어링 표준을 정의합니다. 모든 작업은 아래 지침을 최우선으로 준수해야 합니다.

## 1. 기술 스택 (Tech Stack)
- **Framework:** React 19 (TypeScript)
- **Build Tool:** Vite
- **Package Manager:** npm
- **Styling:** Vanilla CSS (기본 설정, 필요 시 사용자 협의)
- **Linting:** ESLint (v9+)

## 2. 코딩 표준 (Engineering Standards)
- **컴포넌트:** 함수형 컴포넌트와 Hooks를 사용합니다.
- **타입 안정성:** 모든 변수와 함수에 명시적인 타입을 지정합니다 (`any` 지양).
- **디렉토리 구조:**
  - `src/components`: 재사용 가능한 UI 컴포넌트
  - `src/hooks`: 커스텀 훅
  - `src/assets`: 이미지 및 전역 CSS
- **코드 스타일:** ESLint 설정을 엄격히 준수하며, `npm run lint`로 검증합니다.

## 3. 보안 및 품질 (Security & Quality)
- **비밀번호 보호:** `.env` 파일이나 소스 코드에 API 키, 비밀번호를 절대 포함하지 않습니다.
- **검증:** 모든 코드 변경 후에는 `npm run build`와 `npm run lint`를 실행하여 빌드 오류 및 린트 에러가 없는지 확인합니다.
- **테스트:** 새로운 기능 추가 시 테스트 코드 작성을 권장합니다 (현재 테스트 환경 미구축).

## 4. 커뮤니케이션 (Communication)
- 변경 사항은 항상 기술적인 근거와 함께 간결하게 설명합니다.
- 복잡한 아키텍처 변경 전에는 반드시 사용자에게 확인을 받습니다.
