---
layout: post
title:  "Func - Action - Predicate"
date:   2017-01-01 12:35:13 +0300
categories: CSharp
tags: func action predicate generic delegate
comments: 1
---
Bu kavramlara değinmeden önce delegeler ile ilgili biraz bilgi vermek istiyorum.

Delegeler metodları referans eden ve referans ettikleri metodlarla aynı imzaya sahip olan yani aynı tipte parametrelere ve dönüş değerlerine sahip olan yapılardır.

Delegeler için metot referansını tutar deriz, bu tanım herkese çok açıklayıcı gelmeyebilir. Kısaca bu tanıma da değinelim. Öncelikle geri dönüş tipi ve alacağı parametreleriyle bir delege tanımlarız. Tanımladığımız bu delegenin bir instance’ını aldığımızda çağıracağı metodu söyleriz. Çağıracağı bu metot delegenin dönüş tipi ve aldığı parametreler ile aynı olmak zorundadır. Son olarak da instance’ını aldığımız delege’ye parametreleri geçeriz. Buradaki teorik bilgiyi bir örnek ile pekiştirelim.

Öncelikle delegeyi aşağıdaki gibi tanımlıyoruz. Generic bir tip alan ve void olan bir delege oluşturduk.

{% highlight csharp linenos %}
public delegate void SampleDelegate<in T>(T param);
{% endhighlight %}

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby linenos %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/