---
title: "Bounsky's new blog"

# To set og:image:
# image: ...
---

Hi! Welcome to my new blog!

To set up, we need to do a couple of things:
1. Clone the repo to your computer
2. Install rouge gem in the folder to allow the use of rouge code highlighter
3. ```Bundle install``` and run your blog locally
4. Make the necessary adjustments in ```_config.yml``` file (and maybe add some new posts)
5. Change the repo ```origin``` to your own
6. Push all the changes~

#### Cloning the repo

{% highlight bash %}
$ git clone git@github.com:Ezral/duo.git
$ cd duo
{% endhighlight %}

#### Installing rouge code highlighter

Rouge gem is a neat code highlighter that works with 100 languages. We can install it by simply typing this:

{% highlight bash %}
$ gem install rouge
{% endhighlight %}

Once it's installed, add the following line in the ```_config.yml``` file:

{% highlight yml %}
highlighter: rouge
{% endhighlight %}

How to use **rouge**? Open and close your code block like the following example:

{% highlight sh %}
{% raw %}
{% highlight python%}
def function(x, y):
    if x > y:
        print(f"{x} is larger than {y}")
    elif x < y:
        print(f"{y} is larger than {x}")
    else:
        print(f"{x} is equals than {y}")
{% endhighlight %}
{% endraw %}
{% endhighlight %}

#### Run the blog locally

{% highlight sh %}
$ bundle install
$ bundle exec jekyll serve
{% endhighlight %}

#### Make the blog your own

Edit the ```_config.yml``` file to your liking. Change all entries under ```Customize Options: Must Change``` section.

#### Change the repo's origin

Once you've made all the necessary adjustment locally, change your git repo's ```origin``` before pushing:

{% highlight sh %}
$ git remote set-url origin https://github.com/USERNAME/REPOSITORY.git
{% endhighlight %}

#### Push the changes
After that, commit and push the changes that you've made and let github render your blog for you.

Happy blogging!
