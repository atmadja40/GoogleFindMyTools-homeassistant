# GoogleFindMyTools Home Assistant

This is a fork of https://github.com/endeavour/GoogleFindMyTools-homeassistant which is a fork of https://github.com/leonboe1/GoogleFindMyTools

Correcting bugs such as handling when one of google device position is unreachable.

Read carefully the readme of https://github.com/leonboe1/GoogleFindMyTools for the install process

Then run this script using this crontab :

```*/5 * * * * /usr/bin/pkill -f "^/home/USER/yourPath/GoogleFindMyTools-homeassistant/venv/bin/python /home/USER/yourPath/GoogleFindMyTools-homeassistant/publish_mqtt.py$"; sleep 1; cd /home/USER/yourPath/GoogleFindMyTools-homeassistant && /home/USER/yourPath/GoogleFindMyTools-homeassistant/venv/bin/python /home/USER/yourPath/GoogleFindMyTools-homeassistant/publish_mqtt.py >> /home/USER/yourPath/GoogleFindMyTools-homeassistant/tag.log 2>&1```

