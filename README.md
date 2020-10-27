Перед запуском требуется подгрузить flask и psycopg2.

pip install flask

pip install psycopg2

-------------------------------------------------------------------------
Команда для запуска:

docker-compose up -d

-------------------------------------------------------------------------
Переход в режим управления БД:

docker exec -it "id контейнера" bash

Пример: docker exec -it 68e225c5be93 bash

psql -h localhost -p 5432 -U docker -d docker

create table links (link_id SERIAL, link varchar(100));

\dt - просмотр всех таблиц;
