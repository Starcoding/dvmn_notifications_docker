# dvmn_notifications_docker  
Данный код был взят из проекта [dvmn_notifications](https://github.com/Starcoding/dvmn_notifications) для деплоя на Heroku с помощью Docker.

## Деплой  
Для размещения бота на Heroku необходимо:  
- Создать новый проект на Heroku ```heroku create```  
- Клонировать код данного проекта ```git clone https://github.com/Starcoding/dvmn_notifications_docker```  
- Перейти в папку с проектом  
- Запушить ```heroku container:push dvmn_notifications -a *Название вашего Heroku App*```
- Зарелизить ```heroku container:release dvmn_notifications -a *Название вашего Heroku App*```
- Прописать переменные окружения в настройках Heroku App

### Переменные окружения 
- TELEGRAM_TOKEN - Секретный ключ телеграм бота
- TELEGRAM_CHAT_ID - Id чата, в который бот будет отправлять оповещения
- DVMN_TOKEN- Секретный ключ сайта dvmn.org
