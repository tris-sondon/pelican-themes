A quick and dirty nodejs website that shows screenshots of Pelican themes.  The screenshots are sourced from https://github.com/getpelican/pelican-themes via the Github api.

The github data is cached in two files, these have had the following git commands applied to them:

    git update-index --assume-unchanged data/pelican-sha
    git update-index --assume-unchanged data/themes.json


You'll need to set an env var called GITHUB_API_KEY to fetch the theme data from github.  This can be done with something like:

    # Github api key used by pelicanthemes.com
    export GITHUB_API_KEY='put your api key here'

Contribution is very welcome.  Thanks :)


Useful links :
https://github.com/getpelican/pelican-themes
https://api.github.com/repos/getpelican/pelican-themes/contents/bootstrap2


Todo:
periodically check for updates (or use hooks?)
get submodule themes
