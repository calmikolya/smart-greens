# Территориально распределённая ферма витринного типа для проращивания салатных культур

## Описание проекта

Этот проект представляет собой разработку и реализацию автоматизированной установки для проращивания салатных культур прямо в точках продаж. Работа поддерживается акселератором **ФизтехИдея+** и профинансирована в рамках программы **Студенческий стартап**.

## Задача

Создать компактную, полностью автоматизированную и визуально привлекательную установку, способную обеспечить проращивание зелёных культур с автоматическим поливом, системой озонирования и возможностью удалённого управления, подходящую для установки в торговых залах.

## Структура установки

- **Наклонная платформа** из 3 горизонтальных поддонов специальной конструкции, размещённых друг над другом.
- **Автоматизированный полив** методом подтопления по заданной программе.
- **Контейнеры для салатных культур** со встроенными электростатическими решётками (сетки Фарадея) для генерации поля.
- **Управляющий программный комплекс** (АСУ) для настройки режимов проращивания.
- **Система озонирования воздуха**, предназначенная для подавления роста патогенной микрофлоры. Озон подаётся в камеру проращивания по заданному расписанию, при этом соблюдаются санитарные нормы безопасности.
- **Корпус установки**, выполненный с применением технологии фрезеровки оргстекла (пластика) — это обеспечивает эстетичный внешний вид, точную подгонку деталей и возможность интеграции светодиодной подсветки. Все детали конструкции проектировались с учётом возможности промышленного тиражирования.

## Используемые компоненты

- **Микроконтроллер ESP32** — управляет всеми подсистемами (полив, озонирование, освещение, сенсоры). Имеет встроенный Wi-Fi и Bluetooth, что позволяет осуществлять удалённый мониторинг и обновление прошивки.
- **Датчики влажности и температуры** (например, DHT22, грунтовые влагомеры) используются для контроля условий проращивания и передачи информации в управляющую систему.
- **Насос системы полива** — работает по принципу подачи воды в каждый поддон через электромагнитные клапаны. Управляется по времени или по показаниям датчиков. Насос — маломощный, с обратным клапаном, расположенный в баке с водой.
- **Модуль реле на 4 канала** — коммутирует питание насоса, озонатора и освещения.
- **Озонатор промышленного типа** — работает по таймеру, имеет защиту от перегрева.
- **Светодиодная лента с регулировкой яркости** — обеспечивает освещение рассады с возможностью управления по расписанию.
- **Питание системы** — осуществляется от адаптера 12 В с понижающим преобразователем для питания логики ESP32 (5 В / 3.3 В).

## Фото
<img width="522" alt="Снимок экрана 2025-04-12 в 4 59 45 PM" src="https://github.com/user-attachments/assets/075bf3cf-6342-4882-a9c0-42e4e740a350" />

- 📷 *Экспериментальный прототип*
 ![IMG_2261](https://github.com/user-attachments/assets/6c7a7d8b-a668-4ee3-84d2-e794f47fc786)
- 📷 *Финальный образец* — демонстрирует компактный и эстетичный вид устройства, подходящий для установки в магазинах.



https://github.com/user-attachments/assets/1e8f7a2c-7732-49c3-92b9-d88b94270b16


https://github.com/user-attachments/assets/cc5d57b3-87d4-42fc-ae39-6333cebf2ee9
![2025-04-15 21 29 02](https://github.com/user-attachments/assets/c1ae7056-766a-41d4-ae22-97a4b5c5756a)


https://github.com/user-attachments/assets/3c7d06c2-fba9-44f6-b182-fce8e11e6f92



https://github.com/user-attachments/assets/5264c39c-b07e-460d-8c8f-0118f3aacbf4



## Проблемы и трудности


- Обеспечение равномерного полива по всей площади поддонов
- Электробезопасность при генерации электростатического поля
- Интеграция системы озонирования с безопасной периодичностью подачи
- Сложность фрезеровки сложных геометрий и сборки без утечек
- Отладка электроники и защита от сбоев при работе насоса и реле

## Дальнейшие планы

- Интеграция с системой интернет-заказов
- Расширение количества культур
- Добавление датчиков света и расширение набора условий выращивания
- Упрощение конструкции для массового производства
- Создание мобильного приложения для настройки и контроля
"""
