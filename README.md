# heroku-buildpack-ffmpeg

## Usage

Run the following from the heroku command line:

```
heroku buildpacks:add --index 1 https://github.com/srobbin/heroku-buildpack-ffmpeg.git
```

Note: This buildpack should be added before the main language buildpack (by using `--index 1`),
since the application process types are calculated from the last buildpack in the list if no
`Procfile` is specified.

## Fork info

This repo is forked from [https://github.com/jonathanong/heroku-buildpack-ffmpeg-latest](https://github.com/jonathanong/heroku-buildpack-ffmpeg-latest), and changed so that it uses a fixed version of [FFmpeg](https://www.ffmpeg.org/). New, compiled versions of FFmpeg can be found at [https://johnvansickle.com/ffmpeg/](https://johnvansickle.com/ffmpeg/).
