# Nmap 7.94SVN scan initiated Fri Apr 12 05:59:41 2024 as: nmap -sC -sV -Pn -T4 -oN nmap.txt -vvv 10.10.11.240
Nmap scan report for napper.htb (10.10.11.240)
Host is up, received user-set (0.24s latency).
Scanned at 2024-04-12 05:59:41 EDT for 80s
Not shown: 997 filtered tcp ports (no-response)
PORT    STATE SERVICE  REASON  VERSION
53/tcp  open  domain   syn-ack (generic dns response: SERVFAIL)
| fingerprint-strings: 
|   DNSVersionBindReqTCP: 
|     version
|_    bind
80/tcp  open  http     syn-ack Microsoft IIS httpd 10.0
|_http-title: Did not follow redirect to https://app.napper.htb
| http-methods: 
|_  Supported Methods: GET HEAD POST OPTIONS
|_http-server-header: Microsoft-IIS/10.0
443/tcp open  ssl/http syn-ack Microsoft IIS httpd 10.0
|_http-generator: Hugo 0.112.3
| tls-alpn: 
|_  http/1.1
| ssl-cert: Subject: commonName=app.napper.htb/organizationName=MLopsHub/stateOrProvinceName=California/countryName=US/localityName=San Fransisco/organizationalUnitName=MlopsHub Dev
| Subject Alternative Name: DNS:app.napper.htb
| Issuer: commonName=ca.napper.htb/countryName=US/localityName=San Fransisco
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2023-06-07T14:58:55
| Not valid after:  2033-06-04T14:58:55
| MD5:   ee1a:dff8:9a6f:5ddd:1add:9d22:0408:58dc
| SHA-1: f134:fe38:31f5:0c74:9a26:d441:63a8:232d:a67a:782b
| -----BEGIN CERTIFICATE-----
| MIIDzTCCArWgAwIBAgIJALM7fwOVfMaCMA0GCSqGSIb3DQEBCwUAMD0xFjAUBgNV
| BAMMDWNhLm5hcHBlci5odGIxCzAJBgNVBAYTAlVTMRYwFAYDVQQHDA1TYW4gRnJh
| bnNpc2NvMB4XDTIzMDYwNzE0NTg1NVoXDTMzMDYwNDE0NTg1NVowfTELMAkGA1UE
| BhMCVVMxEzARBgNVBAgMCkNhbGlmb3JuaWExFjAUBgNVBAcMDVNhbiBGcmFuc2lz
| Y28xETAPBgNVBAoMCE1Mb3BzSHViMRUwEwYDVQQLDAxNbG9wc0h1YiBEZXYxFzAV
| BgNVBAMMDmFwcC5uYXBwZXIuaHRiMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIB
| CgKCAQEAqkM19E9lbE476qF6RBriuwNHdCgjwLybb9pXWIgtPen6hNCBvzp0XLlY
| ZWJ3NNszYH7Z6pgDJHCDIrSZXtkAEHh7AdoN7ZFLWScHwz/qWesBjH2DYHfBABkm
| qorv3dS6MqpZXJK81e1bQdS9IlRiPmJTYHX17+vfd7FBP2XaARtpgDIkDEPyPIIe
| GfTbtk3/E3N/EjZX7lR7lgAMhZmpEpmb7AoQ1btPraFwH/PXG5r020vfC+fCzgAK
| X3BmCfSzUI2AXz/2GJrRsSSdjKTCLJgn5Cau9bI+IO9pH3HOkfXDiWLB4ip++dGK
| hxYMEc5xwrcF3ZsE6s42cisD8pNipwIDAQABo4GPMIGMMFcGA1UdIwRQME6hQaQ/
| MD0xFjAUBgNVBAMMDWNhLm5hcHBlci5odGIxCzAJBgNVBAYTAlVTMRYwFAYDVQQH
| DA1TYW4gRnJhbnNpc2NvggkA4xs9TVmYevYwCQYDVR0TBAIwADALBgNVHQ8EBAMC
| BPAwGQYDVR0RBBIwEIIOYXBwLm5hcHBlci5odGIwDQYJKoZIhvcNAQELBQADggEB
| ABuy5lV920FJXR4j0dWSAqpEPCXj3jVc7vbozP24sFAocNCzodYiuKV10NyhXxJ+
| rxgu5HgmWk47yaz17eYwMDWYnfoIGRVMl4IkSve/9wr1+ReiywIPGyCG/GCxk3KI
| OG/IyX9j8KR7bhTnlMPixVVqkAu0E2CwZ8I0WmjBdQzEs4wBmpmRO5Eqodxf/jkM
| 3a7CU0Q3m9+SKwOnvarn0Wp++UmlD4/y+O8+j9+URXtD7RElZfrcv9wknVGD7H0s
| U98Kn5WCVanMjGtaQmBjCNdTX/6rif90qiTgyw3mGw8IyatfXAwF75jkvB4vTAHk
| ziVXyfoozsWvOoF8/YiMKsI=
|_-----END CERTIFICATE-----
| http-methods: 
|   Supported Methods: OPTIONS TRACE GET HEAD POST
|_  Potentially risky methods: TRACE
|_http-title: Research Blog | Home 
|_ssl-date: 2024-04-12T10:01:00+00:00; 0s from scanner time.
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port53-TCP:V=7.94SVN%I=7%D=4/12%Time=66190648%P=x86_64-pc-linux-gnu%r(D
SF:NSVersionBindReqTCP,20,"\0\x1e\0\x06\x81\x82\0\x01\0\0\0\0\0\0\x07versi
SF:on\x04bind\0\0\x10\0\x03");
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
|_clock-skew: 0s

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Fri Apr 12 06:01:01 2024 -- 1 IP address (1 host up) scanned in 80.26 seconds
