---
layout: post
title:  "Feb 28 study"
date:   2016-02-28 02:34:25
categories: jekyll update
tags: featured
image: /assets/article_images/2014-08-29-welcome-to-jekyll/desktop.jpg
---

### vmware workstaion pro 설치
 - workstations 12 pro trial 설치 후에는 serial key를 넣어야 하는데 이건 인터넷에 치면 나온다.
 - 설치할때 바로 iso 이미지로 시작하지 말고 없는 걸로 한다음에 하드웨어 설정에서 cd-rom 에 iso 파일을 넣어 주자. 그래야 설치할 때 한글로 하기 편하다.

### 우분투 언어
 - 우분투를 설치할 때 한글로 해서 나중에 영어로 바꾸는게 키보드 설정에 훨씬 편하다. hangul이 없을 때도 있다.

### vmware tools 설치 방법
 - 언어 설정을 끝내고 나면 vmware tools를 설치해야하는데 이건 https://www.youtube.com/watch?v=0U8mnEg7nEw 동영상 참고 

### 우분투 설치 직후 설치할 것(zsh git-core vim ruby rbenv)

 - 우분투를 설치한 직후에는 sudo apt-get install git-core vim zsh 부터 하자
 - 우분투에 oh my zsh 설치하는 방법은 https://gist.github.com/tsabat/1498393 참고
 - ruby를 까는 것은 조심해서 해야한다. .zshrc 파일로 경로 바꾸는 것 잊지말고 다음 사이트를 참고할 것 https://cbednarski.com/articles/installing-ruby/
 - 이건 확실하진 않지만 그 외 하드웨어적인 세팅을 하면 성능이 향상된다고 한다. http://programmingsummaries.tistory.com/301 참고할 것
 -  

### Git global config and time caching

 - https://help.github.com/articles/which-remote-url-should-i-use/ 참고할 것.
 -

### 최초의 git init  후에 풀하기
 - 첫번째 방법은 아예 깨끗한 데에 디렉터리 통쨰로 받아오는 방법 이떈 upstream 이 자동으로 설정된다.
 - 두번째 방법은 git fetch 를 한 후에 git merge origin/master를 하고 git branch --set-upstream-to=origin/master master 이라고 하면 된다.
 - master branch 가 없다는 에러는 아마 init을 하고 나면 master branch 조차 없다고 인식해서 인듯 함. 
 - git clone 으로 받은 후에도 로컬 디렉터리 이름은 변경 가능


You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve --watch`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

{% highlight js %}

<footer class="site-footer">
 <a class="subscribe" href="{{ "/feed.xml" | prepend: site.baseurl }}"> <span class="tooltip"> <i class="fa fa-rss"></i> Subscribe!</span></a>
  <div class="inner">a
   <section class="copyright">All content copyright <a href="mailto:{{ site.email}}">{{ site.name }}</a> &copy; {{ site.time | date: '%Y' }} &bull; All rights reserved.</section>
   <section class="poweredby">Made with <a href="http://jekyllrb.com"> Jekyll</a></section>
  </div>
</footer>
{% endhighlight %}


[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help
