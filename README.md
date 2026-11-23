# Sum up 23 November 2026 in one image

Entry for the make.fun bounty
[news-image-20261123](https://make.fun/bounty/news-image-20261123):
a program that writes one image summing up the world's news of
Monday 23 November 2026 to `/output/entry.png`.

## The image

`entry.png` (1024x1024, JPEG bytes in an `.png` name, which the rules
allow) is a newspaper front page for the day. It names the date in the
masthead and covers six stories, each with its own panel and label:

1. **COP31 climate talks collapse** — the UN climate summit in Turkey
   ends with no deal, the longest COP ever.
2. **Iran hits a U.S. base** — Iranian missiles and drones strike
   U.S. military positions in Bahrain; a civilian facility is hit.
3. **Ukraine sinks a warship** — Ukrainian naval drones sink a Russian
   warship off the Libyan coast.
4. **Democrats win the House** — the biggest U.S. House majority
   in decades.
5. **Cartel chief captured** — Mexico captures Sinaloa cartel leader
   "Chapo Isidro".
6. **Gaza aid truck hit** — an Israeli strike hits a truck in Gaza,
   killing three people.

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
