bandit15@melinda:~$ echo cat /etc/bandit_pass/bandit15 | openssl s_client -connect localhost:30001       
CONNECTED(00000003)

depth=0 CN = localhost

verify error:num=18:self signed certificate

verify return:1

depth=0 CN = localhost

verify return:1

Server certificate

-----BEGIN CERTIFICATE-----

MIICpDCCAYwCCQDDVcPYicjxQjANBgkqhkiG9w0BAQUFADAUMRIwEAYDVQQDEwls
b2NhbGhvc3QwHhcNMTMwNjA2MTM1ODM3WhcNMjMwNjA0MTM1ODM3WjAUMRIwEAYD
VQQDEwlsb2NhbGhvc3QwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQDF
Id/8XRfPayS8u+XfqkXQq3QawTEmxcxQw4TiLKlnqLqsl02U3dUIBqSJu1LQE8lf
/eez2KF9Nse9cXqty6M6J9/515b+xaLfkAV1q97JwO1BfciJDiWqjPerMcikUb0d
zTnDFSpWpnrTjLqlquSWrgRxMffmGi+6x7lsWp8EOAIrFhxadYgTskVUslsgtwBP
dVtDG3OZSa8uyD6LJMCgMpaIs0nI1AS8yWWRnBPP6tujJV9x5JI8GYuC1OB9hsYT
+J7ZMkQ5soOXi9TIuyQSfavH27z44uMF3g4fB6i9l2KNFeKkuq1JVM+HbrXfSlf3
+Gtm/+hO/jlKzGw+pmobAgMBAAEwDQYJKoZIhvcNAQEFBQADggEBAF0ah9QUPxRM
cCNaZ2Bb+IkBXbj1esk92Hv7H4uYIionJl2f+8M6/YgGNhBI4C1r82Hwbi9DwVYs
kztth6DQIBw3KnNLyoKfYmEz6+Azko5rIefeJoHEBdD41tMqmBd8jWi5+hUbkeLr
8A0wzwi/mVQP4xBZ5cELDEaC2MFCi20X4APFFYeXEMjEYwTwADdADiQ52ezle0zr
iSZ10PUmxqjE4NCYo8feZ7emRcAozZElyF9JjoHfXSSiEViELPU2Wb9ygljYz2Hy
AGDcpE2FIGZRiHk+PT2tHD92bp4BeyZsh52pYvItJie3owdIQoQASfperclRvcyn
mNrjHPUubAc=

-----END CERTIFICATE-----

subject=/CN=localhost

issuer=/CN=localhost

No client certificate CA names sent

SSL handshake has read 1272 bytes and written 375 bytes

New, TLSv1/SSLv3, Cipher is DHE-RSA-AES256-SHA

Server public key is 2048 bit

Secure Renegotiation IS supported

Compression: NONE

Expansion: NONE

SSL-Session:

    Protocol  : SSLv3
    Cipher    : DHE-RSA-AES256-SHA
    Session-ID: 39D149A21A2A56D90DC51A0BE4EBC9888DD3DB16A8645BB4D3C6B12B53B8795A
    Session-ID-ctx: 
    Master-Key: 4ED46FF6D414DE2C0AFD0283521A5141FBBB0D8048924E6AE31C6C65053F5ABB35B27F8D61775FE6F01DC3F084E1F7DA
    Key-Arg   : None
    PSK identity: None
    PSK identity hint: None
    SRP username: None
    Start Time: 1406837006
    Timeout   : 300 (sec)
    Verify return code: 18 (self signed certificate)

---

HEARTBEATING

DONE

bandit15@melinda:~$ echo `cat /etc/bandit_pass/bandit15` | openssl s_client -connect localhost:30001 -quiet

depth=0 CN = localhost

verify error:num=18:self signed certificate

verify return:1

depth=0 CN = localhost

verify return:1

Correct!

cluFn7wTiGryunymYOu4RcffSxQluehd

read:errno=0
