﻿# Offline Messenger
Проект, шоб понять "как там все устроено"
# Основные правила в работе над проектом
1) Перед коммитом обновлять все файлы из общей репозитории
2) Все новые переменные/функции добавленные с текущим коммитом вносить в README.md
3) Придерживаться корпоративного стиля
4) Придерживаться структуры проекта
5) Комментировать как минимум названия переменных и функций.
6) Любой кусок кода повторенный более одного раза вынести в отдельную функцию.
# Структура проекта
*ожидает появления*
# Корпоративный стиль
1) Названия переменных: только английские(никакого транслита); camelCase; максимум информативности в как можно более коротком названии.
  Пример:
  Переменная отвечает за имя юнита и имеет класс QString.
  Идеально: QString unitName; //Имя юнита
  Нормально: QString unitName;
  Нельзя: QString unit_name, name, nameOfUnit, imyaYunita, unitNameWasCreatedInMainBodyYesterdayInVersion0.9.
2) Названия функций: только английские(никакого транслита); camelCase; максимум информативности в как можно более коротком названии.
  Пример:
  Переменная отвечает за получение имени юнита(где юнит это класс) и возвращает QString.
  Идеально: QString getUnitName; //Возвращает имя юнита
  Нормально: QString getUnitName;
  Нельзя: QString get_unit_name, unitName, poluchitImyaYunita, getUnitNameWasCreatedInMainBodyYesterdayInVersion0.9;
3) Классы: все переменные *private*; для каждой переменной get- и set- функции; обязательное наличие конструктора и деструктора; конструктор и деструктор всегда *public*; деструктор РОВНО 1; требования к названию аналогичные как и к переменным, но первая буква должна быть заглавной; название класса совпадает с именем файла(class Unit(); Unit.h, Unit.cpp); наличие заголовочного файла с описанием всех функции и переменных; реализация всех функций в *.cpp* файле.
4) Табуляция: tab = 4 пробела; табуляция только tab; фигурные скобочки на новой строчке; между важными кусками кода вставлять
*//-------------------------------------------//*; пробелы после запятых.
# Документация(пример)
Документация проекта должна иметь вид:
Unit.h //Заголовочный файл класса Unit
  Переменные:
    QString unitName; //Имя юнита
    int unitHealth; //Здоровье юнита
  Функции:
    QString getUnitName(); //Возвращает имя юнита
    void setUnitName(QString newUnitName); //Присваивает unitName значение типа QString указанное в newUnitName
    int getUnitHealth(); //Возвращает здоровье юнита
    void setUnitHealth(int newUnitHealth); //Присваивает unitHealth значение типа int указанное в newUnitHealth
    Unit(QString newUnitName); //Присваивает unitName значение типа QString указанное в newUnitName, присваивает unitHealth значение типа int, равное 100; Конструктор класса
    ~Unit(); //Деструктор класса
main.cpp //Основной файл проекта
  Переменные:
  double screenAspectRatio; //Дробь, обозночающая соотношение сторон устройства


