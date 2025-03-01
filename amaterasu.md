---
description: offsec (3 hours)
---

# amaterasu

1. python flask to upload own ssh key to user directory
2. get foothold -> ssh login with key
3. found cron
4. create new tar binary
5. set /usr/bin/find to suid 4000
6. privesc -> run find and get root

<figure><img src=".gitbook/assets/image (706).png" alt=""><figcaption><p>nmap</p></figcaption></figure>

<figure><img src=".gitbook/assets/image (707).png" alt=""><figcaption><p>gobuster</p></figcaption></figure>

<figure><img src=".gitbook/assets/image (708).png" alt=""><figcaption><p>gobuster</p></figcaption></figure>

<figure><img src=".gitbook/assets/image (712).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (713).png" alt=""><figcaption></figcaption></figure>

test upload

<figure><img src=".gitbook/assets/image (710).png" alt=""><figcaption></figcaption></figure>

upload own key to alfredo's directory

<figure><img src=".gitbook/assets/image (711).png" alt=""><figcaption></figcaption></figure>

ssh in with own key

<figure><img src=".gitbook/assets/image (720).png" alt=""><figcaption></figcaption></figure>

read local

<figure><img src=".gitbook/assets/image (715).png" alt=""><figcaption></figcaption></figure>

check cron

<figure><img src=".gitbook/assets/image (716).png" alt=""><figcaption></figcaption></figure>

create a tar binary

<figure><img src=".gitbook/assets/image (717).png" alt=""><figcaption></figcaption></figure>

set SUID 4000 to /usr/bin/find

<figure><img src=".gitbook/assets/image (718).png" alt=""><figcaption></figcaption></figure>

run find to get root

<figure><img src=".gitbook/assets/image (719).png" alt=""><figcaption></figcaption></figure>
