## Установка и настройка окружения
📌 Требования:
* Python 3.10 – 3.11
* pip ≥ 23
* Git
* macOS (Apple Silicon (M1/M2/M3)/ Linux / Windows

Проект рассчитан на CPU

Проверка версии Python:  
`python3 --version`

### Установка программы Tesseract OCR
* macOS (Homebrew required)  
`brew install tesseract libomp`  

Проверка:  
`tesseract --version`

* Windows  
`import pytesseract
pytesseract.pytesseract.tesseract_cmd = \    
    r"C:\Program Files\Tesseract-OCR\tesseract.exe"`

### Клонирование репозитория:  
`git clone https://github.com/MazurenkovK/MazurenkovKS_mproject_v1.0.git`  
`cd MazurenkovKS_mproject_v1.0.git`

### Создание виртуального окружения 
* macOS / Linux  
`python3.11 -m venv .venv`  
`source .venv/bin/activate`

* Windows (PowerShell)  
`python -m venv .venv`  
`.venv\Scripts\activate`

После активации должно появиться: (.venv)

### Установка зависимостей:   
`pip install --upgrade pip`  
`pip install -r requirements.txt`


## Запуск проекта
### Тестирование pipeline:  
`python app/main.py`

### Запуск оценки MVP:  
`python app/main_order.py`

### Деактивация окружения:  
`deactivate`




