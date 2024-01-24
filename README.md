# Инициализация на локално хранилище
git init

# Създаване на нов файл и подготовка за запис
echo "Hello, this is a sample file." > sample.txt
git add sample.txt
git commit -m "Initial commit - add sample.txt"

# Създаване на нов клон
git checkout -b нов-клон

# Промени в новия клон
echo "New content in the new branch." >> sample.txt
git add sample.txt
git commit -m "Add new content in the new branch"

# Връщане в основния клон
git checkout master

# Допълнителни промени
echo "Additional content in the main branch." >> sample.txt
git add sample.txt
git commit -m "Add additional content in the main branch"

# Сливане с новия клон
git merge нов-клон


# Изтриване на новия клон
git branch -d нов-клон

# Създаване на README файл
echo "# My Git Project" > README.md

# Добавяне на значки и кратко описание
echo "![Build Status](https://img.shields.io/badge/build-passing-brightgreen)" >> README.md
echo "This is a sample Git project." >> README.md

# Добавяне и комитване на README
git add README.md
git commit -m "Add README file with badges and description"

# Клониране на хранилището
git clone https://github.com/вашето-потребителско-име/вашето-хранилище.git

# Влизане в директорията на проекта
cd вашето-хранилище

# Стартиране на проекта (по ваш избор)
