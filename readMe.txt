docker-compose-files/graylog terminalde açalým

docker-compose up -d 
komutunu çalýþtýrýralým

sýrasý ile

c_mongo
c_graylog
c_elasticsearch

container kurulacak.


http://127.0.0.1:9000/ 
web portalýný browserda açalým

üstmenüden system inputs menüsünden Gelf UDP Launch new Input açýlan modaldan.
title alana loglarý yakalamak için bir input kanal oluþturualým. (Tek node olduðu için local input seçebiliriz)

bind_address: 0.0.0.0
decompress_size_limit: 8388608
number_worker_threads: 4
override_source: <empty>
port: 12201
recv_buffer_size: 262144

aþaðýdaki gibi localde çalýþan bir input çýktýsý alacaðýz.
show received message buttonu ile ilgili input'a baðlanýyoruz.

api uygulamasýný çaþlýþtýrýp endpointi tetiklersek 2 adet information ve error level log atýlacaktýr.


