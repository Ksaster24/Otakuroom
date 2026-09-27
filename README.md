# OtakuRoom Mobile

Мобильный-first фронтенд для сервиса совместного просмотра.

## Уже есть
- адаптив под телефон / планшет / desktop;
- PWA manifest;
- тёмный минималистичный интерфейс;
- мобильная нижняя навигация;
- каталог и поиск;
- обновление каталога через Jikan API с fallback;
- жанры;
- карточки аниме;
- выбор озвучки в UI;
- экраны профиля, друзей и комнат;
- модальные окна регистрации, комнаты и добавления друга.

## Реальный backend
Для production подключаем Supabase:
- Auth: email/password или magic link;
- profiles;
- friendships;
- rooms;
- room_members;
- messages;
- Realtime для чата и синхронизации.

SQL заготовка находится в `supabase.sql`.

Важно: в production обязательно настроить RLS policies. Не вставляй service_role key в браузер.
