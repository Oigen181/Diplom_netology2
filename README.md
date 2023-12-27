# Дипломная работа по профессии «`Системный администратор`» Андреев Евгений.

=======================================================================

### Решение

---

### 1. Создание чистой инфраструктуры и настройка Nginx на web сервера

---

Для решения данной задачи использовал Ubuntu 22.04. Первым делом создаем файл main.tf для terraform с созданием всех условий для данной задачи.


На данном скриншоте представлен итог создания чистой инфраструктуры - 6 ВМ и балансировщика.

![Скриншот 27-12-2023 123747](https://github.com/Oigen181/Diplom_netology2/assets/126493876/39770e48-ae01-4057-a7e9-a2269ad2819d)



Целевые группы:



![Скриншот 27-12-2023 123915](https://github.com/Oigen181/Diplom_netology2/assets/126493876/2ca27818-e4ca-44b2-8701-3a26c021893c)



Backend group



![Скриншот 27-12-2023 124014](https://github.com/Oigen181/Diplom_netology2/assets/126493876/6f3461af-26c6-4b92-9d92-ddfea9900050)



HTTP Router



![Скриншот 27-12-2023 124150](https://github.com/Oigen181/Diplom_netology2/assets/126493876/3f6dc8b7-e348-4a83-872a-1d3258bce9ce)



Application load balancer



![Скриншот 27-12-2023 124303](https://github.com/Oigen181/Diplom_netology2/assets/126493876/f8475ec1-6b71-42f4-a030-59bdcd710e8b)



Тест сайта через баоансировщик 158.160.139.41:80


http://158.160.139.41



![Скриншот 27-12-2023 124733](https://github.com/Oigen181/Diplom_netology2/assets/126493876/12c17e3b-b11f-4722-92a3-4adb8bc58bb3)



---

### 2. Мониторинг 

----

Zabbix

http://51.250.37.61:8080/zabbix.php?action=host.list

![Скриншот 27-12-2023 124559](https://github.com/Oigen181/Diplom_netology2/assets/126493876/9a9219b5-c96d-432c-9bc0-d6aada4d0bd3)


![Скриншот 27-12-2023 142422](https://github.com/Oigen181/Diplom_netology2/assets/126493876/d769f6d1-50fb-46eb-8806-2a608003ede2)



Данные для авторизации:

Логин: Admin

Пароль: zabbix

---

### 3. Логи

---

KIbana

http://51.250.44.165:5601/app/discover


![Скриншот 27-12-2023 125207](https://github.com/Oigen181/Diplom_netology2/assets/126493876/d1cc6c83-d262-48ac-9f81-62ff85e93a84)


Elasticsearch на виртуальной машине


![Скриншот 27-12-2023 203402](https://github.com/Oigen181/Diplom_netology2/assets/126493876/10c27c08-74fd-4108-b92c-7f191d476a97)



---

### 4.Сеть

---

Группы безопасности


![Скриншот 27-12-2023 125534](https://github.com/Oigen181/Diplom_netology2/assets/126493876/3b3b27cb-c23e-4e84-b136-9df174242d11)

Резервное копирование

![Скриншот 27-12-2023 125814](https://github.com/Oigen181/Diplom_netology2/assets/126493876/0e8072c2-2f08-48c3-8d6f-aa22de7aaa1f)

![Скриншот 27-12-2023 130521](https://github.com/Oigen181/Diplom_netology2/assets/126493876/f4cf92f5-d9d8-499e-8209-9b3682b9304c)


