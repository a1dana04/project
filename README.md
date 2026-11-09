# Той & Иш-чара — сайт онлайн-приглашений (Next.js + Supabase)

Витрина шаблонов, демо с музыкой и эффектами, страницы приглашений по ссылке `/i/<код>`,
админ-панель `/admin` (пароль, загрузка фото и музыки), заказы через WhatsApp.

## Запуск за 15 минут

1. **Supabase** (supabase.com, бесплатно): создайте проект -> SQL Editor -> вставьте содержимое `supabase.sql` -> Run.
   Затем Project Settings -> API: скопируйте Project URL, anon key и service_role key.
2. **GitHub**: создайте репозиторий и загрузите в него все файлы этой папки.
3. **Vercel** (vercel.com): Add New -> Project -> выберите репозиторий. До нажатия Deploy откройте Environment Variables
   и добавьте все 7 переменных из файла `.env.example` с вашими значениями.
4. Нажмите Deploy. Сайт откроется на адресе вида `ваш-проект.vercel.app`.
5. Свой домен: Vercel -> Settings -> Domains.

## Как пользоваться
- `/admin`: войти (ADMIN_LOGIN / ADMIN_PASSWORD) -> «Новое приглашение» -> заполнить, загрузить фото и музыку -> «Сохранить».
- «Отправить заказчику» откроет WhatsApp с готовой ссылкой `https://ваш-сайт/i/код`.

## Локально
```
npm install
cp .env.example .env.local   # впишите значения
npm run dev
```
