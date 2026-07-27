# 세준위키

https://sejunch.github.io 소스.

## 고치기

```bash
.venv/bin/mkdocs serve      # 미리보기 (http://127.0.0.1:8000)
```

`docs/` 안의 마크다운만 고치면 된다. `main` 에 push 하면 자동으로 배포된다.

## 문서 새로 만들기

`docs/` 에 `.md` 파일 하나 만들고 맨 위에 분류를 적는다.

```
---
tags:
  - 만든 것
---

# 문서 이름

!!! abstract "개요"
    한 문단 요약.

## 1. 개요
## 2. 특징
## 3. 관련 문서
```

그다음 `mkdocs.yml` 의 `nav:` 에 한 줄 추가하면 왼쪽 메뉴에 나온다.

- 각주는 `[^이름]` 으로 달고 아래에 `[^이름]: 내용` 을 적는다
- 다른 문서로 링크는 `[한랭](한랭.md)`
- 분류(`tags`)를 적으면 분류 문서에 자동으로 모인다

## 처음 설정 (한 번만)

```bash
python3 -m venv .venv && .venv/bin/pip install -r requirements.txt
```
