---
layout: default
title: 홈
---

# 환영합니다!

여기는 제 블로그입니다.

## 최근 포스트

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url | relative_url }}) - {{ post.date | date: "%Y년 %m월 %d일" }}
{% endfor %}

## 소개

Jekyll과 GitHub Pages로 만든 블로그입니다.

# 블로그

전체 글 목록입니다.

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url | relative_url }})

{{ post.description }}

**작성일:** {{ post.date | date: "%Y년 %m월 %d일" }}

**카테고리:** {{ post.categories | join: ", " }}

**태그:** {{ post.tags | join: ", " }}

---
{% endfor %}

# 소개

안녕하세요!

## 블로그 소개

이 블로그는 Jekyll과 GitHub Pages를 이용해 만들었습니다.

## 관심사

- 웹 개발
- 블로그 운영
- 오픈소스

## 연락처

- GitHub: [@username](https://github.com/username)
- Email: your@email.com
