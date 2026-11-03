[Русский](README.md) | **English**

# ImageFeed

A photo feed for iPhone. A project from the Yandex Practicum iOS course.

Brief: [iOS-ImageFeed-Public](https://github.com/Yandex-Practicum/iOS-ImageFeed-Public). Design: [Figma](https://www.figma.com/design/MujlanK7BDoQRrGci5G6pi/Image-Feed). API: [Unsplash](https://unsplash.com/documentation).

## Purpose

A multi-screen app for browsing pictures through the Unsplash API.

Goals:

- browse an endless feed of pictures from Unsplash Editorial;
- see a short summary of the user profile.

## Summary

Sign-in uses Unsplash OAuth.

The main screen is an image feed. Pictures can be viewed, added to favorites, and removed from favorites.

Each picture opens on its own, and a link to it can be shared outside the app.

The profile holds favorite pictures and a short description of the user.

The brief has two versions: a basic one and an extended one. The extended version adds favorites and a like button on the full-screen photo.

## What it does

Sign-in uses Unsplash OAuth. The token stays on the device, so the next launch skips the login until the user logs out of the profile.

After sign-in the Unsplash Editorial feed opens. A card shows the date and a like button. A photo can be opened full screen, zoomed, and sent through the system share sheet.

The profile tab shows the avatar, name, username, and bio from Unsplash. The account can be logged out from there.

## Stack

UIKit, URLSession, WebKit, Kingfisher, ProgressHUD, SwiftKeychainWrapper, XCTest. Packages come through Swift Package Manager. The app targets iPhone on iOS 17, portrait only.

## Run

An Unsplash account is required, and the app keys belong in `AuthConfiguration`.

```bash
git clone https://github.com/dpogonia/ImageFeed-YANDEX.git
cd ImageFeed-YANDEX
open ImageFeed.xcodeproj
```

Run the **ImageFeed** scheme on an iPhone simulator.

## Author

[Dmitrii Pogonia](https://github.com/dpogonia)
