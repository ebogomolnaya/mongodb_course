# mongodb_course
Домашнее задание 1 для курса по MongoDB

1. Разворачиваем виртуальную машину на Ubuntu 24.04.3 LTS (Noble) в VirtualBox.
2. Устанавливаем и запускаем последнюю стабильную версию MongoDB Community Server

![img.png](img/img.png)

3. Запускаем сессию Mongo

![img_1.png](img/img_1.png)

4. Создаем коллекцию со случайным количеством элементов
for ( i = 0; i < Math.random()*100; ++i ) {
   db.docs.insert( { key: i, value: Math.random() } );
}

![img_2.png](img/img_2.png)

5. Считаем количество элементов
db.docs.countDocuments()

![img_3.png](img/img_3.png)

6. Останавливаем MongoDB
sudo systemctl stop mongod

![img_4.png](img/img_4.png)
