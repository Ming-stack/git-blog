# 多媒体

### img & map
> map的name和id一致,img的usemap相当于id选择器

```html
<img usemap="#g" class="fit-picture"
     src="/media/cc0-images/grapefruit-slice-332-332.jpg"
     alt="Grapefruit slice atop a pile of other slices">
<map name="g" id="g" name="primary">
  <area shape="circle" coords="200,250,300" href="another.htm" />
  <area shape="rect" coords="0,0,250,300" href="another.htm" />
  <area shape="default" nohref />
</map>
```
### audio
> 音频

```html
<audio src="">
</audio>
```
### video
> 视频

```html
<video src="">
</video>
```

### track
> 字幕

```html
<video controls
       src="/media/cc0-videos/friday.mp4">
    <track default
           kind="captions"
           srclang="en"
           src="/media/examples/friday.vtt" />
    Sorry, your browser doesn't support embedded videos.
</video>
```