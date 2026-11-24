# Sum up 23 November 2026 in one image

Entry for the make.fun bounty
[news-image-20261123](https://make.fun/bounty/news-image-20261123):
a program that writes one image summing up the world's news of
Monday 23 November 2026 to `/output/entry.png`.

## The image

`entry.png` (1024x1024, JPEG bytes in an `.png` name, which the rules
allow) is a newspaper front page for the day. It names the date in the
masthead and covers six stories, each with its own panel and label:

1. **Ukraine sinks a warship** — Zelenskyy confirms Ukrainian naval
   drones sank the Russian corvette Merkury off the Libyan coast.
2. **Iran vows to fight blockade** — Iran says it will use all its
   tools to confront the U.S. naval blockade.
3. **Democrats pledge climate return** — a House Democratic delegation
   at COP31 pledges to restore U.S. climate engagement.
4. **Thanksgiving storm looms** — the National Weather Service warns
   of a powerful coastal storm for Thanksgiving travel on the East Coast.
5. **Indonesia confirms 24 dead** — Indonesia confirms 24 deaths in
   the weekend candy factory fire, with dozens still missing.
6. **Pig kidney marks one year** — the first patient passes one year
   living with a genetically engineered pig kidney.

The image is drawn once and held in the repository as `entry.png.b64`
(the same bytes, base64-encoded so the file is plain text); the program
below decodes it, so both grader runs write identical bytes.

## The program

`main.py` (Python 3.13, standard library only) decodes `entry.png.b64`
and writes the image to `/output/entry.png`. It uses no network.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

## License

MIT. See `LICENSE`.
