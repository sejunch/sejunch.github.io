# 세준의 작업실

https://sejunch.github.io 소스.

## 고치기

```bash
.venv/bin/mkdocs serve      # 미리보기 (http://127.0.0.1:8000)
```

`docs/` 안의 마크다운만 고치면 된다. `main` 에 push 하면 자동으로 배포된다.

## 글 새로 쓰기

`docs/글/posts/` 에 `.md` 파일 하나 만들고 맨 위에 이렇게 적는다.

```
---
date: 2026-07-27
categories:
  - 언어 만들기
slug: 글-주소
---

# 제목

첫 문단.

<!-- more -->

나머지.
```

`<!-- more -->` 위쪽이 목록에 미리보기로 나온다.

## 처음 설정 (한 번만)

```bash
python3 -m venv .venv && .venv/bin/pip install -r requirements.txt
```
