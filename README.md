find . -path ./backups -prune -o -type f -name '*.html' -exec cp {} ./backups \; -print0 | xargs -0 perl -pi -e 's|(?<title>)(ШРИ)|ТИК|g' 
