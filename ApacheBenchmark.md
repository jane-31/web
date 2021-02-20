h1 БЕЗ БАЛАНСИРОВКИ

> Цитата
This is ApacheBench, Version 2.3 <$Revision: 1879490 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/



Benchmarking localhost (be patient)
Completed 1000 requests
Completed 2000 requests
Completed 3000 requests
Completed 4000 requests
Completed 5000 requests
Completed 6000 requests
Completed 7000 requests
Completed 8000 requests
Completed 9000 requests
Completed 10000 requests
Finished 10000 requests


Server Software:        nginx/1.18.0
Server Hostname:        localhost
Server Port:            443
SSL/TLS Protocol:       TLSv1.2,ECDHE-RSA-AES256-GCM-SHA384,2048,256
Server Temp Key:        X25519 253 bits
TLS Server Name:        localhost

Document Path:          /api/v1
Document Length:        Variable

Concurrency Level:      10
Time taken for tests:   27.761 seconds
Complete requests:      10000
Failed requests:        0
Non-2xx responses:      10000
Total transferred:      3970000 bytes
HTML transferred:       1780000 bytes
Requests per second:    360.22 [#/sec] (mean)
Time per request:       27.761 [ms] (mean)
Time per request:       2.776 [ms] (mean, across all concurrent requests)
Transfer rate:          139.66 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        7   24  10.7     21      99
Processing:     0    4   4.3      3      47
Waiting:        0    3   4.2      2      47
Total:          7   28  11.8     25     105

Percentage of the requests served within a certain time (ms)
  50%     25
  66%     31
  75%     34
  80%     37
  90%     44
  95%     50
  98%     57
  99%     62
 100%    105 (longest request)


h1 С БАЛАНСИРОВКОЙ
> Цитата
This is ApacheBench, Version 2.3 <$Revision: 1879490 $>
Copyright 1996 Adam Twiss, Zeus Technology Ltd, http://www.zeustech.net/
Licensed to The Apache Software Foundation, http://www.apache.org/

Benchmarking localhost (be patient)
Completed 1000 requests
Completed 2000 requests
Completed 3000 requests
Completed 4000 requests
Completed 5000 requests
Completed 6000 requests
Completed 7000 requests
Completed 8000 requests
Completed 9000 requests
Completed 10000 requests
Finished 10000 requests


Server Software:        nginx/1.18.0
Server Hostname:        localhost
Server Port:            443
SSL/TLS Protocol:       TLSv1.2,ECDHE-RSA-AES256-GCM-SHA384,2048,256
Server Temp Key:        X25519 253 bits
TLS Server Name:        localhost

Document Path:          /api/v1
Document Length:        Variable

Concurrency Level:      10
Time taken for tests:   27.481 seconds
Complete requests:      10000
Failed requests:        0
Non-2xx responses:      10000
Total transferred:      3970000 bytes
HTML transferred:       1780000 bytes
Requests per second:    363.89 [#/sec] (mean)
Time per request:       27.481 [ms] (mean)
Time per request:       2.748 [ms] (mean, across all concurrent requests)
Transfer rate:          141.08 [Kbytes/sec] received

Connection Times (ms)
              min  mean[+/-sd] median   max
Connect:        7   23  10.6     21      73
Processing:     0    4   4.3      3      44
Waiting:        0    3   4.2      2      44
Total:          8   27  11.7     25      92

Percentage of the requests served within a certain time (ms)
  50%     25
  66%     30
  75%     34
  80%     36
  90%     44
  95%     50
  98%     57
  99%     60
 100%     92 (longest request)
