# Mind Map
```mermaid
mindmap
  root((Информационная система))
    Экспертная оценка неисправностей
      Диагностика
        Программная диагностика
        Аппаратная диагностика
      Исправление ошибок
    Генерация отчетов
      Автоматическая генерация
      Редактирование экспертами
    Уведомления
      Отправка отчетов
      Обратная связь
    Аутентификация
      Регистрация
      Вход
    Сессии
      Инициализация сессий
      Управление доступом
```


```mermaid
journey
  title Путешествие пользователя в системе
  section Авторизация
    Пользователь: Вход в систему: 5: Успешно
    Система: Проверка данных: 4: Успешно
    Система: Создание сессии: 5: Успешно
  section Регистрация неисправности
    Пользователь: Регистрация проблемы: 5: Легко
    Система: Создание задачи: 4: Автоматизировано
    Система: Уведомление эксперта: 3: Прямо
  section Диагностика и отчет
    Эксперт: Диагностика: 5: Удобно
    Эксперт: Редактирование отчета: 4: Гибко
    Система: Генерация уведомлений: 3: Автоматизировано
  section Обратная связь
    Пользователь: Получение уведомления: 4: Быстро
    Пользователь: Подтверждение завершения: 5: Удобно
```



```mermaid
quadrantChart
    title Приоритизация задач информационной системы
    x-axis Low Risk --> High Risk
    y-axis Low Value --> High Value
    quadrant-1 Quick Wins
    quadrant-2 High Priority
    quadrant-3 Re-evaluate
    quadrant-4 Avoid or Simplify
    "Инициализация сессии": [0.3, 0.9]
    "Аутентификация пользователя": [0.4, 0.85]
    "Диагностика ПО": [0.7, 0.8]
    "Диагностика аппаратной части": [0.8, 0.9]
    "Исправление ошибок": [0.6, 0.7]
    "Генерация отчета": [0.5, 0.6]
    "Уведомления пользователя": [0.2, 0.3]
    "Экспертная оценка": [0.7, 0.85]
```



```mermaid
  gitGraph
  commit id: "Начало проекта"
  branch feature/authentication
  commit id: "Добавление аутентификации"
  checkout main
  merge feature/authentication

  branch feature/diagnosis
  commit id: "Добавление диагностики"
  checkout main
  merge feature/diagnosis

  branch feature/reporting
  commit id: "Добавление генерации отчетов"
  checkout main
  merge feature/reporting

  branch feature/notifications
  commit id: "Добавление уведомлений"
  checkout main
  merge feature/notifications
```
