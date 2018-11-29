docker run -it -p 139:139 -p 445:445 \
    -v /opt/mediadepot/apps/samba:/config \
    -v /media:/media \
    -e SAMBA_USERNAME=depot \
    -e SAMBA_PASSWORD
    mediadepot/samba