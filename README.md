usshoustondive.com
==================

USS Houston (CA-30) Dive Team website

To generate the website:

    ttree -f ttree.cfg

Jay syncs the Dropbox images over to the website like so:

    rsync -av --progress --delete --max-size=5m \
      ~/Dropbox/Shared/houston\ file/ jays.net:/var/www/usshoustondive.com/assets/

Pull down a local set of production images:

    rsync -av --progress --max-size=5m \
      jhannah@usshoustondive.com:/var/www/usshoustondive.com/assets/ www/assets/

