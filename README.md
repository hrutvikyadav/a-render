# a-render

## Demo website for rendering asciinema recordings

### Purpose

Already using asciinema to record terminal sessions. Needed to share those with a co.
Tried converting to `gif` it is terrible (no controls)
Tried gif -> mp4 with `ffmpeg`, need to find supported codecs for windows first
Tried cast -> mp4, previous steps are recommended
*Finally* settled for embedding the asciinema player in our own website
> There are multiple options
> - just use standalone js bundle __( current choice )__
> - npm package

### Standalone bundle

```bash
wget -O asciinema-player.min.js https://github.com/asciinema/asciinema-player/releases/download/v3.6.3/asciinema-player.min.js
wget -O asciinema-player.css https://github.com/asciinema/asciinema-player/releases/download/v3.6.3/asciinema-player.css
```

References
[asciinema documentation](https://docs.asciinema.org/manual/player/quick-start/#standalone-player-bundle)
