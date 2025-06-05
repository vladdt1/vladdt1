<p align="center">
  <!-- Анимационный GIF-баннер в шапке -->
  <img src="https://media.giphy.com/media/26ufdipQqU2lhNA4g/giphy.gif" alt="Welcome Animation" width="600" />
</p>

## 🛠 Технологии и Инструменты

<p align="center">
  <!-- Шильдики (badges) с указанием версий -->
  <img src="https://img.shields.io/badge/PHP-8.1-blue.svg" alt="PHP 8.1" />
  <img src="https://img.shields.io/badge/Symfony-6.x-purple.svg" alt="Symfony 6.x" />
  <img src="https://img.shields.io/badge/Doctrine-2.x-green.svg" alt="Doctrine ORM" />
  <img src="https://img.shields.io/badge/Twig-3.x-orange.svg" alt="Twig" />
  <img src="https://img.shields.io/badge/Redis-^6.0-red.svg" alt="Redis Cache" />
  <img src="https://img.shields.io/badge/SQLite-3.x-yellow.svg" alt="SQLite" />
</p>

- **Язык:** PHP 8.1  
- **Фреймворк:** Symfony 6  
- **ORM:** Doctrine 2  
- **Шаблонизатор:** Twig  
- **Кэширование:** Redis (PSR-6)  
- **СУБД (по умолчанию для dev):** SQLite  
- **Тестирование:** PHPUnit  
- **CI/CD:** GitHub Actions  

---

## 📜 Описание Проекта

Этот репозиторий содержит **великолепное приложение** на основе Symfony 6, демонстрирующее:

1. **Чистую архитектуру** (DDD/Service-ориентированный подход).  
2. **Продвинутую конфигурацию Doctrine** (методы кеширования, ленивые соединения, L2 кэш).  
3. **Гибкую систему ролей и прав** (Symfony Security + Voter).  
4. **Адаптивный фронтенд** с анимациями через CSS/Twig и пользовательские компоненты.  
5. **Примеры команд-скриптов (Console Commands)** для фоновых задач (Cron).  

---

## 🎨 Анимации и Демонстрации

### 1. Анимация загрузки

```twig
{# Пример Twig-шаблона с CSS-анимацией «курсионок» #}
<div class="loader">
  <div class="dot dot-1"></div>
  <div class="dot dot-2"></div>
  <div class="dot dot-3"></div>
</div>

<style>
.loader {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 2rem;
}
.dot {
  width: 12px;
  height: 12px;
  margin: 0 6px;
  background-color: #4CAF50;
  border-radius: 50%;
  animation: bounce 0.6s infinite alternate;
}
.dot-2 { animation-delay: 0.2s; }
.dot-3 { animation-delay: 0.4s; }

@keyframes bounce {
  to { transform: translateY(-15px); }
}
</style>
