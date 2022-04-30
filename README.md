# Testing
Repo for random testing purposes

**Source**: https://mattj.io/posts/2021-02-27-create-animated-gif-and-webp-from-videos-using-ffmpeg/

## webp
[<img src="arts.webp" width="450"/>](arts.webp)

## gif gifski
[<img src="arts.gif" width="450"/>](arts.gif)

## gif ffmpeg 
```
ffmpeg -i "arts.mp4" -vf "fps=60,scale=720:-1:flags=lanczos,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse" -loop 0 arts.gif
```
[<img src="arts2.gif" width="450"/>](arts2.gif)
