```
apt update && apt install -y nano less tree gpg
gpg --full-gen-key
echo "keyid-format 0xlong
    throw-keyids
    no-emit-version
    no-comments" > ~/.gnupg/gpg.conf
gpg -k 
gpg -K
cd /tmp/
echo "Hello world" > /tmp/file.txt
cat file.txt 
gpg -e -a -r some@mail.com file.txt
nano file.txt.asc 
rm file.txt
gpg -d -o file.txt file.txt.asc 
cat file.txt
gpg --export some@mail.com > public.gpg
rm file.txt*
cat public.gpg 
gpg --export -a some@mail.com > public.gpg
gpg --export-secret-key -a some@mail.com > secret.gpg
cat public.gpg 
gpg --export-secret-key -a some@mail.com secret.gpg
gpg --delete-secret-keys some@mail.com
gpg --delete-keys some@mail.com
gpg --import secret.gpg
apt install pass
pass init
pass git init 
pass git remote add origin https://github.com/${user}/${repo}.git
pass git branch -M main
pass git pull
```