# How to use GIF stickers in Telegram

Disclaimer: I am not affiliated with the developers of the tools introduced in this document. I am not responsible for any loss, damage, or anything you did not expect but encounter by following this document.

## Convert to PNG or WEBP format with 512x512px

Install in macOS

```
brew install gifsicle
brew install ffmpeg
```

Resize GIF to 512x512px

```
mkdir Telegram_from_WeChat
find WeChat -name "*.gif" -type f | xargs -I @ bash -c "gifsicle --resize 512x512 -i @ > Telegram_from_@"
```

Convert GIF to WEBP

```
mkdir Webm_Telegram_from_WeChat
find Telegram_from_WeChat -name "*.gif" -type f | xargs -I @ bash -c "ffmpeg -i @ -c vp9 -b:v 0 -crf 40 Webm_@.webm"
```

## Create package 

Add @Stickers account and follow the instruction.

## Add the created package

Click the created package URL.
