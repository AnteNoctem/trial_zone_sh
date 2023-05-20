#!/bin/bash

mkdir /etc/bkp/
mv /etc/cron* /etc/bkp/
cd /etc/bkp/
TMP=$(date +"%y-%m-%d_%T")
echo "#!/bin/bash" >> temp
echo "rename 's/cron/$TMP cron/' cron*" >> temp
chmod 755 temp
bash temp
rm temp
