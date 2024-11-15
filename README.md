# Лабораторная работа №6

Порядок выполнения работы:
1. Создала аккаунт на сайте GitHub.
2. Сделала копию в личное хранилище из https://github.com/Kurtyanik/LR6/ (Fork).
3. Установила Git 
4. После установки настроила клиент git, введя имя пользователя (Группа
Фамилия И.О.) и email.

```
git config --global user.name ""

git config --global user.email ""
```

![image](https://github.com/user-attachments/assets/9e6ca3e8-1fa9-4d17-9c82-1ab3c29dc460)

6. Клонировала свой личный удалённый репозиторий на компьютер (назвала работу gLR6, так как переделывала 2 раза)
   
```
git clone https://github.com/Gordeyko/gLR6

```

   ![image](https://github.com/user-attachments/assets/fe4e37d7-a331-4713-bb55-a3f2d152eedd)

7. Добавила файл через интерфейс GitHub. Подтянула изменения в
локальный репозиторий

```
git pull

```

![image](https://github.com/user-attachments/assets/cb0dc524-a786-48dc-801e-1d57891e4333)

8. Работу продолжила локально, перейдя в папку
   
```
cd gLR6
```

![image](https://github.com/user-attachments/assets/9b994604-0714-43a5-81a0-3609c46adb7c)

9. Получила историю операций для каждой из веток.
    
```
git log --oneline
```

![image](https://github.com/user-attachments/assets/e73f2105-e322-466d-b365-bb3ec998d343)

10. Просмотрела последние изменения.
    
```
git log -p 
```

![image](https://github.com/user-attachments/assets/1fd70fab-feed-4e1e-bbea-2d740f42a90b)

11. Выполнила слияние в ветку master
    
```
git checkout -b branch1
git add .
git commit -m ""
git checkout master
git merge branch1
```

![image](https://github.com/user-attachments/assets/725ea5a0-a26d-4a08-95bd-59ecc2556e5e)
![image](https://github.com/user-attachments/assets/2667083b-8f6a-4c96-9440-131b0d89c2b4)


12. Удалила побочную ветку после успешного слияния (не сохранился скрин)
    
```
git branch -d branch1
```
13. Сделала 2 изменения и зафиксировала их
    
```
git add .
git commit -m ""
```
![image](https://github.com/user-attachments/assets/7e763df9-3726-4312-9ac5-5bcae25fea54)

14. Сделала откат коммита
    
```
git log --oneline
git revert 5351a1d
```
![image](https://github.com/user-attachments/assets/b6a50314-d7a5-49a6-9fc4-750d3c0528e5)

![image](https://github.com/user-attachments/assets/0650de29-fa80-4ab1-ba2b-b8d26955f2d6)

15. Создала ветку для отчёта
```
git checkout -b othet
```

![image](https://github.com/user-attachments/assets/25b3d3a0-6bc1-4ea1-a6ab-0e08610a5beb)

16. Оформила отчёт в файле README.md, используя markdown синтаксис. Файлы снимков экрана разместила в отдельной папке screen

17. Получила историю операций в форматированном виде
    
```
git log --pretty=format:"%h %ad | %s%d [%an]" --date=short
```

![image](https://github.com/user-attachments/assets/97c3eea9-6cf1-4044-8d6a-edfd6edcc574)

18. Отправила локальные изменения в сетевое хранилище GitHub
    
```
git push origin report
```
