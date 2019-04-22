---
title: "How to start GitHub Pages with The remote theme!"
date: 2019-04-16 08:26:28
categories: jekyll github pages
tags: github pages jekyll
---

# 1. repository 생성

* `public`으로 생성할 것.
* repository name을 다음과 같이 설정.
	* 기본형의 경우, `myname.github.io` 로 설정.
		* 여기서 `myname`은 github의 계정명임.
	* Project Blog인 경우, `project_name` 으로 설정.
		* 여기서 `project_name`은 현재 생성하는 프로젝트의 이름이면 됨.
* theme를 고를것.
	* [themes_on_github](https://github.com/topics/jekyll-theme) 에서 고르면 됨.
	* [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes)가 현재 1위이므로 선택함.

# 2. `remote_theme` 로 설정 최소화.

* `_config.yml` 파일만 고른 테마에서 다운로드해서 repository에 업로드
* `_config.yml` 파일 중 다음을 수정
	* `remote_theme`의 주석을 제거함
		* [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes)의 경우엔 `remote_theme : mmistakes/minimal-mistakes` 인 라인이 주석해제되는 것임.
	* `url` 을  `"https://myname.github.io"`로 설정.
	* `baseurl` 은 Project Blog인 경우에만 `"project_name"`으로 설정.

# 3. `index.html` 생성.

* 고른 테마에서 다운로드해서 사용하면 됨.

# 4. 기타 customizing을 할 파일들을 다운로드하여 수정.

* [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes)의 경우, latex를 지원하기 위해서 다음을 다운로드하여 repository에 업로드한 후 수정함.
* `_include/head/custom.html` 에 latex 지원을 위한 처리함.

```javascript
<script type="text/x-mathjax-config">
MathJax.Hub.Config({
  tex2jax: {
    inlineMath: [['$','$'], ['\\(','\\)']],
    processEscapes: true
  }
});
</script>
<script type="text/javascript" async
	  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>
```

* 위의 코딩을 추가시 mathjax를 통해 latex (inline기능 포함)수행 가능해짐.

# 5. `_posts`에 글 추가하기.

* `yyyy-mm-dd-post_name.md` 의 형태로 파일만들어서 추가.

# 6. 확인.

* `https://myname.github.io/project_name` 주소를 웹브라우저에 입력하고 확인.
* github의 repostiroy에 제대로 push를 해야함.
* push 이후에도 약 5분정도 기다릴 것.(최초의 경우)

# References

* [jekyll-docs](https://jekyllrb.com/docs/home)
* [jekyll-gh](https://github.com/jekyll/jekyll)
* [jekyll-talk](https://talk.jekyllrb.com/)
* [MathJax-zjuwhw's blog](http://zjuwhw.github.io/2017/06/04/MathJax.html)


