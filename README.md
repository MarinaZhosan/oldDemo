Описание проекта
Этот проект является тестовым заданием для стажировки в компанию Северсталь.

О проекте
Я реализовала приложение "Заметки" в соответствии с техническим заданием. Приложение разработано с использованием T-SQL, Java и JavaFX.

Функциональные возможности
	•	Создание заметок: Пользователь может создавать новые заметки.
	•	Редактирование заметок: В приложении предусмотрена возможность редактирования существующих заметок.
	•	Удаление заметок: Пользователь может удалять ненужные заметки.
	•	Стилизация текста: Реализованы стилистические возможности, такие как изменение шрифта и выделение текста жирным.
	•	Интерфейс
	•	Созданные заметки отображаются в главном окне в виде списка, где отображается заголовок заметки и дата её создания. Приложение обладает интуитивно понятным интерфейсом, что делает его удобным в использовании.

Хранение данных
Заметки сохраняются и надежно хранятся в базе данных MS SQL Server, обеспечивая их сохранность между сеансами использования приложения.

Особенности
При первом запуске приложения автоматически создается заметка по умолчанию с описанием функционала приложения, чтобы пользователь мог сразу ознакомиться с его возможностями.

Технологии
	•	T-SQL: Для работы с базой данных.
	•	Java: Основной язык программирования приложения.
	•	JavaFX: Для создания графического интерфейса пользователя.

Инструкция по установке БД!
Создание таблицы и БД:

//////////////////////////////////////////////////////////
CREATE DATABASE NotesDB;

USE NotesDB;

CREATE TABLE Notes (
    id INT PRIMARY KEY IDENTITY(1,1),
    title NVARCHAR(255) NOT NULL,
    content NVARCHAR(MAX),
    created_date DATETIME DEFAULT GETDATE()
);
///////////////////////////////////////////////////////////

Для запуска из терминала введите mvn jaсvafx:run


