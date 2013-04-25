# flasky

This is a Pelican theme [F. Javier Alba](https://github.com/fjavieralba/flasky)
has created for his blog fjavieralba.com

My intension for this fork is a modification to fit my needs. I plan to make
the theme scalable and may add a mobile edition.

DONE:

* scaleable: the width is now scalable.
* blockqoutes are formatted now.
* a site tile is shown with it's one style.

TODO:

* the pygments style is used for code and for normal verbatim blocks. I don't
  know how Pelican distinguish between code and verbatim.

In order to correctly use this theme you will need this variables in your
`pelicanconf.py`:

~~~~~ {.python}
    AUTHOR = u'Your Name'
    SITENAME = u"Your site name"
    SITEURL = 'blog'
    TIMEZONE = "Europe/Madrid"

    #Navigation sections and relative URL:
    SECTIONS = [('Blog', 'index.html'),
            ('Archive', 'archives.html'),
            ('Tags', 'tags.html'),
            ('Projects', 'pages/projects.html'),
            ('Talks', 'pages/talks.html'),
            ('About', 'pages/about-me.html')]

    DEFAULT_CATEGORY = 'Uncategorized'
    DATE_FORMAT = {
    'en': '%d %m %Y'
    }
    DEFAULT_DATE_FORMAT = '%d %m %Y'

    DISQUS_SITENAME = "your_disqus_user"
    TWITTER_USERNAME = 'your_twitter_user_without @'
    LINKEDIN_URL = 'http://es.linkedin.com/in/you/en'
    GITHUB_URL = 'http://github.com/you'

    PDF_GENERATOR = False
    REVERSE_CATEGORY_ORDER = True
    LOCALE = ""
    DEFAULT_PAGINATION = 10

    FEED_RSS = 'feeds/all.rss.xml'
    CATEGORY_FEED_RSS = 'feeds/%s.rss.xml'

    OUTPUT_PATH = '/your/output/directory'

    GOOGLE_ANALYTICS_ACCOUNT = 'UA-00000000-1'

    PIWIK_URL = 'myurl.com/piwik'
    PIWIK_SSL_URL = 'myurl.com/piwik'
    PIWIK_SITE_ID = '1'

    MAIL_USERNAME = 'your_user'
    MAIL_HOST = 'gmail.com'

    # static paths will be copied under the same name
    STATIC_PATHS = ["images"]

    # A list of files to copy from the source to the destination
    #FILES_TO_COPY = (('extra/robots.txt', 'robots.txt'),)
~~~~~

Here is a sample of the current (unfinished and unpolished) state:

![screenshot](https://raw.github.com/joede/flasky/master/screenshot.jpg)
