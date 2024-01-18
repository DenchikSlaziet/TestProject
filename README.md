Автор проекта
---
Кочетков Денис Александрович

База данных
---
MSSQL

Рекомендации по установке
---
1) Перейдите в класс TestProjectContext (TestProject.Context)
2) Откройте консоль диспетчера пакетов
3) Выполните 4 команду указанную в классе TestProjectContext
4) В случае ошибки выполните 1 команду далее 4
5) Программа готова к работе

SQL скрипт для добавления начальных данных
---
```
USE TestProjectDB

INSERT INTO [dbo].[Orders]
           ([Number]
           ,[SenderCity]
           ,[SenderAddress]
           ,[RecipientCity]
           ,[RecipientAddress]
           ,[Weight]
           ,[PickupDate]
           ,[CreatedAt]
           ,[CreatedBy]
           ,[UpdatedAt]
           ,[UpdatedBy]
           ,[DeletedAt])
     VALUES
           ('1b4543bd-e4cf-421a-9762-c473fd96eb17'
           ,'Москва'
           ,'Пример Адреса'
           ,'СПб'
           ,'Пример Адреса'
           ,300
           ,'01.01.2023'
           ,GETDATE()
           ,'Insert'
           ,GETDATE()
           ,'Insert'
           ,null),
		    ('75185c94-fc8c-478d-9e89-169fdbda0709'
           ,'СПб'
           ,'Пример Адреса'
           ,'Москва'
           ,'Пример Адреса'
           ,500
           ,'03.03.2023'
           ,GETDATE()
           ,'Insert'
           ,GETDATE()
           ,'Insert'
           ,null),
		   ('b65943ec-0a09-4824-8a57-e2b63b7e3b1c'
           ,'Краснодар'
           ,'Пример Адреса'
           ,'Владимир'
           ,'Пример Адреса'
           ,5000
           ,'05.05.2023'
           ,GETDATE()
           ,'Insert'
           ,GETDATE()
           ,'Insert'
           ,null)
```
