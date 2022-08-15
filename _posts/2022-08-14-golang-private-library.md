In order to be able to import private Golang repositories from Github, you must follow these steps:

1. Generate Github personal access token. Follow this instructions:
https://docs.github.com/en/enterprise-server@3.3/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token

3. export the personal access token in environment variable on your system:

{% highlight bash %}
GITHUB_TOKEN=ghp_AHUKB…
{% endhighlight %}

When set, will use "https://${GITHUB_TOKEN}:x-oauth-basic@github.com/" to download dependencies from github. Allowing access to private repos.

2. Change access method to Github repositories:
{% highlight bash %} 
git config --global [url.git@github.com](mailto:url.git@github.com):.insteadOf [https://github.com/](https://github.com/)
{% endhighlight %}


3. Add private repository to GOPRIVATE environment variable (comma separated list):
{% highlight bash %} 
export GOPRIVATE="[github.com/getritmo/](http://github.com/getritmo/country)"`
{% endhighlight %}

4. Get dependencies with:

{% highlight bash %} 
go mod tidy
{% endhighlight %}

{% highlight bash %} 
go get 
{% endhighlight %}


