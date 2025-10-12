# 🚀 GitBasicTrainer - Swift Playground App

<div align="center">

![Swift](https://img.shields.io/badge/Swift-5.0+-orange.svg)
![SwiftUI](https://img.shields.io/badge/SwiftUI-3.0+-blue.svg)
![Platform](https://img.shields.io/badge/Platform-iPadOS%2015%2B%20%7C%20macOS%2012%2B-lightgrey.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

**Интерактивное приложение для управления задачами и миссиями**

[![Download](https://img.shields.io/badge/Download-Playground-brightgreen)](https://github.com/IrinaMuravyova/gitTrainer/releases/latest)
[![Stars](https://img.shields.io/github/stars/IrinaMuravyova/gitTrainer?style=social)](https://github.com/IrinaMuravyova/gitTrainer)

</div>

## 📱 О проекте

**MGitBasicTrainer** - это полноценное SwiftUI приложение, созданное в Swift Playgrounds. Приложение демонстрирует современные подходы к разработке iOS приложений с использованием архитектуры MVVM, реактивного программирования и кастомных интерфейсов.

<div align="center">
<img src="https://i.ibb.co/DPWXJbNk/git-Trainer.png" alt="App Preview" width="300"/>
</div>

## ✨ Возможности

- 🎯 **Многоуровневая система** - Beginner, Intermediate, Advanced
- 📊 **Категоризация задач** по типам и сложности
- ✅ **Визуальное отслеживание** прогресса выполнения
- 🎨 **Интуитивный интерфейс** с разделением на sidebar и content
- 📝 **Система логов** и детального просмотра задач
- 🔄 **Реактивное обновление** интерфейса

## 🚀 Быстрый старт

### 📥 Скачивание и запуск за 2 минуты

1. **Скачайте последнюю версию**
   ```bash
   # Нажмите на кнопку Download выше или
   # Перейдите в раздел Releases и скачайте .zip файл
   ```

2. **Распакуйте архив**
   ```bash
   # Найдите файл GitBasicTrainer.playground.zip
   # Распакуйте его двойным кликом
   ```

3. **Откройте в Swift Playgrounds**
   - **На iPad**: Откройте Files → Найдите папку → Поделиться → Swift Playgrounds
   - **На Mac**: Двойной клик на `GitBasicTrainer.playground`

4. **Запустите приложение**
   - Нажмите кнопку **"Run MyApp"** вверху экрана
   - Наслаждайтесь! 🎉

### 📋 Требования

- **Swift Playgrounds 4.0+**
- **iPadOS 15.0+** или **macOS 12.0+**
- **Swift 5.0+**

## 🏗 Архитектура

```swift
// Чистая архитектура SwiftUI
@main
struct MyApp: App {
    var body: some Scene {
        WindowGroup {
            ContentView()
        }
    }
}

// Реактивное управление состоянием
class LevelStateManager: ObservableObject {
    @Published var selectedLevel: Level = .beginner
    @Published var levelStates: [Level: LevelState] = [:]
}
```

### 🎯 Ключевые компоненты

- **`MyApp.swift`** - Главная структура приложения
- **`ContentView.swift`** - Корневой view
- **`SidebarView.swift`** - Панель навигации с уровнями
- **`MissionDetailView.swift`** - Детализация миссий
- **`LevelStateManager.swift`** - Менеджер состояния
- **Модели данных** - Mission, Level, TaskType

## 🎨 Интерфейс

<div align="center">

| Sidebar Navigation | Mission Details |
|--------------------|-----------------|
| ![Sidebar](https://i.ibb.co/vCy0rq3V/sideBar.png) | ![Details](https://i.ibb.co/0yNf4L7q/mission-Details.png) |

</div>

## 🔧 Для разработчиков

### Структура проекта
```
GitBasicTrainer.playground/
├── MyApp.swift                    # Главная структура приложения
├── ContentView.swift              # Корневой view
├── ViewMissionDetailView.swift    # Детали миссии
├── ViewMissionRowView.swift       # Элемент списка миссий
├── ViewModelsLevelManager.swift    # Менеджер состояния уровней
├── ModelMission.swift             # Модель миссии
├── ModelLevel.swift               # Модель уровня
├── ModelCommand.swift             # Модель команды
├── ResourcesConstraints.swift      # Константы и настройки
└── ResourcesMissions.swift        # Данные миссий
```

### 🛠 Технологии

- **SwiftUI** - Modern declarative UI
- **Combine** - Reactive programming
- **MVVM** - Architecture pattern
- **ObservableObject** - State management
- **Custom Views** - Reusable components

## 🤝 Участие в разработке

Мы приветствуем вклад в проект! 

1. Форкните репозиторий
2. Создайте ветку для вашей функции (`git checkout -b feature/amazing-feature`)
3. Закоммитьте изменения (`git commit -m 'Add amazing feature'`)
4. Запушьте в ветку (`git push origin feature/amazing-feature`)
5. Откройте Pull Request

## 📄 Лицензия

Этот проект распространяется под лицензией MIT. Смотрите файл `LICENSE` для подробностей.

## 📞 Контакты и поддержка

- 🐛 **Нашли баг?** [Создайте Issue](https://github.com/IrinaMuravyova/gitTrainer/issues)
- 💡 **Есть идея?** Напишите нам!
- ⭐ **Понравился проект?** Поставьте звезду!

---

<div align="center">

### 📊 Статистика

![Downloads](https://img.shields.io/github/downloads/IrinaMuravyova/gitTrainer/total?color=success)
![Last Commit](https://img.shields.io/github/last-commit/IrinaMuravyova/gitTrainer)
![Repo Size](https://img.shields.io/github/repo-size/IrinaMuravyova/gitTrainer)

**Сделано с ❤️ и SwiftUI**

</div>
