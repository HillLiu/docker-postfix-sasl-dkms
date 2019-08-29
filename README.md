Alpine postfix + dkms + cyrus-sasl
======

## Docker hub
  * https://hub.docker.com/r/hillliu/postfix-sasl-dkms

## Test auth
  * docker-compose up
  * docker-compose exec mail sh 
  * apk add busybox-extras
  * telnet localhost 25
  * EHLO mail.example.com
  * AUTH PLAIN AHRlc3RfdXNlcgB0ZXN0X3Bhc3N3b3Jk

## Test send mail
  * HELO mail.example.com
  * mail from: test@example.com
  * rcpt to: your@example.com 
  * data
  * .
  * done

