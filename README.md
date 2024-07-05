# Інструкція

```bash
# Створіть в своєму середовищі новий каталог з назвою "new-project".
mkdir new-project

# Перейдіть до каталогу "new-project".
cd new-project

# Ініціалізуйте новий публічний Git-репозиторій всередині каталогу "new-project".
git init -b main

# Створіть новий файл з назвою "README.md" і додайте до нього початковий текст.
echo "# Інструкція" > README.md

# Підготуйте файл "README.md" до коміту.
git add README.md

# Закомітьте зміни у репозиторій з коміт повідомленням “init”.
git commit -m "init"

# Створіть нову гілку з назвою "development" і перейдіть до неї.
git switch -c development

# Додайте інструкцію до файлу "README.md" і підготуйте їх до коміту.
# echo "this" >> README.md
git add README.md

# Закомітьте зміни у гілці "development" з повідомленням про коміт.
git commit -m "Add instructions to README"

# Об'єднайте зміни з гілки "development" у гілку "main".
git switch main
git merge development

# Перевірте статус, переконайтеся, що все актуально.
git status

# Закомітьте зміни
git remote add origin https://github.com/ihorhrysha/new-project.git
git push -u origin main
```