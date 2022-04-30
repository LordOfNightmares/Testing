# Testing
Repo for random testing purposes

**Source**: https://mattj.io/posts/2021-02-27-create-animated-gif-and-webp-from-videos-using-ffmpeg/

## ffmpeg (webp)

<details>
<summary><pre><code>ffmpeg -i rulings.mp4 -vcodec libwebp -filter:v fps=fps=20 -lossless 1 -loop 0 -preset default -an -vsync 1 rulings.webp</code></pre></summary>
  
## Search  
  
[<img src="search.webp" width="450"/>](search.webp)
  
## Rulings
  
[<img src="rulings.webp" width="450"/>](rulings.webp)
  
## Arts
  
[<img src="arts.webp" width="450"/>](arts.webp)
  
</details>


## gifski
<details>
<summary>Animations</summary>
  
[<img src="arts.gif" width="450"/>](arts.gif)
  
</details>

## ffmpeg (gif)

<details>
<summary><pre><code>ffmpeg -i "arts.mp4" -vf "fps=60,scale=720:-1:flags=lanczos,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse" -loop 0 arts.gif</code></pre></summary>
  
[<img src="arts2.gif" width="450"/>](arts2.gif)
  
</details>

