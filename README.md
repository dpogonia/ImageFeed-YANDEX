**Русский** | [English](README.en.md)

# ImageFeed

Лента фотографий для iPhone. Учебный проект курса iOS-разработки Яндекс Практикума.

Задание: [iOS-ImageFeed-Public](https://github.com/Yandex-Practicum/iOS-ImageFeed-Public). Макет: [Figma](https://www.figma.com/design/MujlanK7BDoQRrGci5G6pi/Image-Feed). API: [Unsplash](https://unsplash.com/documentation).

## Назначение

Многостраничное приложение для просмотра изображений через API Unsplash.

Цели:

- смотреть бесконечную ленту картинок из Unsplash Editorial;
- смотреть краткую информацию из профиля пользователя.

## Краткое описание

Вход в приложение идёт через OAuth Unsplash.

Главный экран — лента изображений. Картинки можно смотреть, добавлять в избранное и убирать оттуда.

Каждое изображение открывается отдельно, ссылкой на него можно поделиться за пределами приложения.

В профиле есть избранные изображения и краткие данные пользователя.

В задании две версии: базовая и расширенная. В расширенной появляются избранное и лайк на экране просмотра фотографии.

## Что умеет приложение

Вход через OAuth Unsplash. Токен сохраняется на устройстве, поэтому повторно входить не нужно, пока пользователь сам не выйдет из профиля.

После входа открывается лента Unsplash Editorial. У карточки есть дата и лайк. Фото можно открыть на весь экран, увеличить и отправить через системное меню «Поделиться».

Во вкладке профиля видны аватар, имя, юзернейм и описание из Unsplash. Оттуда же можно выйти из аккаунта.

## Стек

UIKit, URLSession, WebKit, Kingfisher, ProgressHUD, SwiftKeychainWrapper, XCTest. Пакеты подключены через Swift Package Manager. Приложение рассчитано на iPhone с iOS 17, только портретная ориентация.

## Запуск

Нужен аккаунт Unsplash и ключи приложения в `AuthConfiguration`.

```bash
git clone https://github.com/dpogonia/ImageFeed-YANDEX.git
cd ImageFeed-YANDEX
open ImageFeed.xcodeproj
```

Запустите схему **ImageFeed** на симуляторе iPhone.

## Автор

[Dmitrii Pogonia](https://github.com/dpogonia)
