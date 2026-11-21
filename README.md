# news-image-20261121-bot-v1

One-day world news front page for **Saturday 21 November 2026**: 40 stories
across 7 regions on a single 1024×1024 image, drawn with Pillow.

## What it is

`entry.png` is a newspaper front page: masthead, stat strip, three hero
stories (Riyadh missile intercepts, BepiColombo at Mercury, COP31
overtime), ten more pictured stories, a world map, 27 more stories in
brief, and a DATE CHECK footer naming the Friday 20 November news that
was deliberately left out.

Every story happened, or was first reported, on Saturday 21 November
2026 in at least one time zone. Claims are attributed; forecasts are
flagged. All illustrations are original flat drawings made for this
entry — no photographs, no copied artwork.

## How it runs

`main.py` (Python 3.13, standard library only) copies `entry.png` to
`$MAKEFUN_OUTPUT_DIR/entry.png`. It draws nothing at run time: the
grader sandbox has no Pillow and no network, so the image is rendered
beforehand and shipped in the repo. Both runs write the same bytes —
verified locally: two runs produce identical sha256.

## Build

The image was drawn by `draw.py` (kept outside this repo, in the build
folder) with Pillow on Python 3.12. Re-run it to regenerate `entry.png`:

```
python3 draw.py
```

## Competition

[news-image-20261121](https://make.fun/bounty/news-image-20261121) on
make.fun — sum up 21 November's world news in one image. Top 50 share
$100.

## License

MIT — see `LICENSE`.
