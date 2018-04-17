# nextcloud
<p>部署方法</p>
<pre><code>
    docker run -d \
    -v /media/pi/macos/nextcloud:/var/www/html \
    -v /media/pi/macos/nextcloud/apps:/var/www/html/custom_apps \
    -v /media/pi/macos/nextcloud/config:/var/www/html/config \
    -v /media/pi/macos/nextcloud/data:/var/www/html/data \
    --name  NextCloud \
    -p 80:80 \
    nextcloud
</code></pre>