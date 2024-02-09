# usshoustondive.com

USS Houston (CA-30) Dive Team website

Clone the site:

    git checkout git@github.com:jhannah-netlify/usshoustondive.com.git
    git checkout git@github.com:jhannah-netlify/usshoustondive.com.git usshoustondive.com-gh-pages
    cd usshoustondive.com-gh-pages
    git checkout gh-pages
    cd ../usshoustondive.com

Re-generate the website:

    ttree -f ttree.cfg
    cp -r assets ../usshoustondive.com-gh-pages/
    cd ../usshoustondive.com-gh-pages
    git diff
    git commit -a
    git push

## Deprecated

We moved to Netlify hosting, so this doesn't apply anymore:

Jay syncs the Dropbox images over to the website like so:

    rsync -av --progress --delete --max-size=5m \
      ~/Dropbox/Shared/houston\ file/ usshoustondive.com:/var/www/usshoustondive.com/assets/


