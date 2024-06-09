
[[UML]]

Диаграмма деятельности - диаграмма, которая показывает поток управление от одной деятельности к другой

Элементы активити:
- деятельность
- поток управления 
- ветвление (разделение, соединение)
- дорожки
![[Pasted image 20240608195408.png]]

![[Pasted image 20240608195439.png]]

![[Pasted image 20240608195512.png]]

![[Pasted image 20240608195528.png]]

- @startuml
- |Пользователь|
- start
- :Перейти на страницу своих счетов;

- |Система|
- :Открытие страницы счетов пользователя;

- |Пользователь|
- :Создать вклад;

- |Система|
- :Предоставить пользователю выбор вклада;

- |Пользователь|
- repeat :Выбрать вклад;
    - repeat while (Вклад доступен?) is (Нет) not (Да)

- fork
- :Создание вклада;

- |Система|
- fork again
- :Оформление вклада;
- endfork

- |Пользователь|
- :Пополнить вклад;

- stop
- @enduml

//www.plantuml.com/plantuml/png/XL9DJeDW4Dr_fvYblG8kx5L8H2LMQ03ZXWLIVnOqcZHkjV46dwP4B1QkC7CZtn2Rr1PhDysyz-RD-sOOneaR9PSN8vFod1kkPSeV-7zdApcNMgUcqnW7Wb8oW9-WAk8LMv9hoO5P59NSoGG0UXiKjyhTeoDNkqE30Q-0eOV35ziKXYyebf99eOPSRhiLloo8szw0Z_3U4zx1s0RmGa6P4jWbrvYnwCyqroT2tNImXRpIlh-cFy1G2dw3FjlmPhi_LUIDFJSXXsVQB5bFECBlHtPrveyyEk3PcgLrG9bm2y_LqO3y68fdtTQ0WZ11ySHsOCn969rlRa6No-LMrjrDQ1kvfwuVT8UwqGU2gS7t6NZ1iNRySmgbMgNLO_SSSHAEpH1M-22_0G00