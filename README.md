BLOG
---
by 20213064 이창조
<br>

##  Features
- Jekyll
- 템플릿 적용
- 댓글 기능 구현
- favicon
<br>

### Jekyll 설치
----
지킬 설치

> gem install bundler jekyll

프로젝트 생성
> jekyll new MyBlogName

<br>

### 테마 적용
----
mediator 테마를 적용

`URL` : <https://github.com/dirkfabisch/mediator#mediator>

테마 적용 후 필수 gem 설치
>bundle install

로컬 호스트에서 템플릿 테스트
> bundle exec jekyll serve

<br>

### 댓글 기능 구현
----
**Disqus를 이용하여 댓글 기능 추가**

Disqus 사이트에서 블로그 주소 추가후 _config.yml 수정
```html
comment:
    provider: "disqus"
    disqus:
        shortname:  "changjo"
```
_layouts/post.html 수정
```html
{% if page.comments %}
    <h2>Comments</h2>
    <div id="disqus_thread"></div>
    <script>
    let PAGE_URL = "{{site.url}}{{page.url}}"
    let PAGE_IDENTIFIER = "{{page.url}}"
    var disqus_config = function () {
        this.page.url = PAGE_URL;
        this.page.identifier = PAGE_IDENTIFIER;
    };
    
    (function() {
    var d = document, s = d.createElement('script');
    s.src = 'https://changjo.disqus.com/embed.js';
    s.setAttribute('data-timestamp', +new Date());
    (d.head || d.body).appendChild(s);
    })();
    </script>
    <noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
{% endif %}
```
이후 post 작성시 댓글 기능을 넣고 싶다면 다음을 추가
> comments: true

<br>

### favicon 기능
----
템플릿에 favicon이 적용 되어있음
assets/images/favicon.png를 수정하여 바로가기 이미지 교체
