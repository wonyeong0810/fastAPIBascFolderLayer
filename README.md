# fastAPIBascFolderLayer
파이썬 fastAPI 폴더 구조 기본 세팅 | python fastAPI folder Layer Basic Setting



project_root/
├── app/
│   ├── __init__.py
│   ├── main.py                # FastAPI 애플리케이션 진입점
│   ├── config.py              # 환경설정 및 설정 관련 코드
│   ├── api/
│   │   ├── __init__.py
│   │   ├── deps.py            # 의존성 주입 관련 모듈
│   │   ├── endpoints/         # API 엔드포인트 (라우터) 정의
│   │   │   ├── __init__.py
│   │   │   ├── user.py        # 사용자 관련 라우터
│   │   │   └── item.py        # 아이템 관련 라우터
│   │   └── router.py          # 모든 라우터 등록
│   ├── db/
│   │   ├── __init__.py
│   │   ├── models.py          # SQLAlchemy 모델 정의
│   │   └── session.py         # 데이터베이스 세션 관리
│   ├── crud/
│   │   ├── __init__.py
│   │   ├── user.py            # 사용자 관련 CRUD 함수
│   │   └── item.py            # 아이템 관련 CRUD 함수
│   ├── schemas/
│   │   ├── __init__.py
│   │   ├── user.py            # 사용자 관련 Pydantic 스키마
│   │   └── item.py            # 아이템 관련 Pydantic 스키마
│   └── utils.py               # 재사용 가능한 유틸리티 함수
├── .env                       # 환경 변수 설정 파일
├── requirements.txt           # Python 패키지 목록
└── README.md                  # 프로젝트 설명 파일
