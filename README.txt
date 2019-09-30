1) AB requests in 10 seconds with https (concurrency level/requests completed)
1 / 202
2 / 351
4 / 620
8 / 833
16 / 1032
32 / 1128
64 / 1146
128 / 1146
256 / error

2) There are diminishing returns at higher concurrency levels because at a certain point the server will be at its maximum capacity which means that additional requests will have to wait until the server has room to complete another request. If the requests are not being handled concurrently than the number of requests completed will not increase.

3) AB request in 10 seconds with http
1 / 474
4 / 1425
16 / 5548
64 / 10197
256 / error

Http performs significantly better and scales much better with additional concurrency compared to https.

4) Github can respond so quickly because it's web pages are all static which drastically decreases load time.

5) .03 seconds
