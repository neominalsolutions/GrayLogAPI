docker-compose-files/graylog terminalde a�al�m

docker-compose up -d 
komutunu �al��t�r�ral�m

s�ras� ile

c_mongo
c_graylog
c_elasticsearch

container kurulacak.


http://127.0.0.1:9000/ 
web portal�n� browserda a�al�m

�stmen�den system inputs men�s�nden Gelf UDP Launch new Input a��lan modaldan.
title alana loglar� yakalamak i�in bir input kanal olu�turual�m. (Tek node oldu�u i�in local input se�ebiliriz)

bind_address: 0.0.0.0
decompress_size_limit: 8388608
number_worker_threads: 4
override_source: <empty>
port: 12201
recv_buffer_size: 262144

a�a��daki gibi localde �al��an bir input ��kt�s� alaca��z.
show received message buttonu ile ilgili input'a ba�lan�yoruz.

api uygulamas�n� �a�l��t�r�p endpointi tetiklersek 2 adet information ve error level log at�lacakt�r.


