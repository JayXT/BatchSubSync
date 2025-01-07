# BatchSubSync

The repository offers bash scripts for batch subtitle timing resynchronization using [ffsubsync](https://github.com/smacke/ffsubsync). Here are the details about the scripts:

- ffsubsync should be installed and available in the system PATH.
- The scripts should be marked as exectutable and placed in the directory under the PATH.
- There're two scripts for syncing all subtitles (.srt or .ass): one syncs with other subtitles (.srt or .ass) and one syncs with videos (.mkv or .mp4). 
- Both scripts should be executed from the directory containing the subtitles to be resynced.
- Each script requires a single parameter: a relative path to a directory containing either reference subtitle files or reference video files.
- The scripts assume that the files in the working directory and the reference directory have identical base names, differing only in their extensions.
- Resynchronized subtitle files are saved in the ./Retimed directory. Each file is suffixed with _retimed in its name.

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
