# BatchSubSync

## EN

The repository offers bash scripts for batch subtitle timing resync using [ffsubsync](https://github.com/smacke/ffsubsync). Here are the key information about the scripts:

- ffsubsync should be installed and available in the system PATH.
- The scripts should be marked as exectutable and placed in the directory under the PATH.
- There're two scripts for syncing all subtitles (.srt or .ass): one syncs with other subtitles (.srt or .ass) and the other syncs with videos (.mkv or .mp4). 
- Both scripts should be executed from the directory containing the subtitles to be resynced.
- Each script requires a single parameter: a relative path to a directory containing either reference subtitle files or the actual video files.
- The scripts assume that the files in the working directory and the reference directory have identical base names, differing only in their extensions.
- Resynced subtitle files are saved in the ./Retimed directory. Each file is suffixed with _retimed in its name.

Example of usage for subtitle to subtitle sync:

```
cd /home/user/Videos/SampleTVSeries/JP-Subs
batch_sync_subs_to_subs ../EN-Subs
```

Example of usage for subtitle to video sync (videos are located in a directory one level higher):

```
cd /home/user/Videos/SampleTVSeries/JP-Subs
batch_sync_subs_to_videos ../
```



## UA

Репозиторій пропонує bash-скрипти для масової/пакетної синхронізації таймінгу субтитрів за допомогою [ffsubsync](https://github.com/smacke/ffsubsync). Ось ключова інформація про ці скрипти:

- ffsubsync має бути встановлений і доступний у системному PATH.
- Скрипти мають бути позначені як виконувані і розміщені в директорії під PATH.
- Існує два скрипти для синхронізації всіх субтитрів (.srt або .ass): один синхронізує їх з іншими субтитрами (.srt або .ass), а інший синхронізує з відео (.mkv або .mp4). 
- Обидва скрипти слід запускати з теки, що містить субтитри, які потрібно пересинхронізувати.
- Кожному скрипту потрібен лише один параметр: відносний шлях до каталогу, що містить правильні файли субтитрів або самі відеофайли.
- Скрипти припускають, що файли в поточній робочій та еталонній теці мають однакові базові імена, відрізняючись лише розширеннями.
- Пересинхронізовані файли субтитрів зберігаються у каталозі ./Retimed. До назви кожного файлу додається суфікс _retimed.

Приклад використання для синхронізації субтитрів до субтитрів:

```
cd /home/user/Відео/ПрикладСеріалу/Японські-Субтитри
batch_sync_subs_to_subs ../Англійські-Субтитри
```

Приклад використання для синхронізації субтитрів з відео (відео знаходиться в каталозі на рівень вище):

```
cd /home/user/Відео/ПрикладСеріалу/Японські-Субтитри
batch_sync_subs_to_videos ../
```

