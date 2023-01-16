1  apt update && apt install -y nano less tree gpg
2  gpg --full-gen-key
3  echo "keyid-format 0xlong
    throw-keyids
    no-emit-version
    no-comments" > ~/.gnupg/gpg.conf
6  cd
9  cd .gnupg/
11  gpg -k
12  gpg -K
13  cd /tmp/
14  echo "Hello world" > /tmp/file.txt
16  cat file.txt 
18  gpg -e -a -r some@mail.com file.txt
20  nano file.txt.asc 
21  rm file.txt
22  gpg -d -o file.txt file.txt.asc 
24  cat file.txt
26  pass
27  apt install pass
28  gpg --export some@mail.com > public.gpg
30  rm file.txt*
32  cd public.gpg 
33  cat public.gpg 
34  gpg --export -a some@mail.com > public.gpg
36  cat public.gpg 
37  gpg --export-secret-key -a some@mail.com secret.gpg
38  gpg --delete-keys some@mail.com