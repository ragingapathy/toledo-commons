# Toledo commons

Short, kind observations about places in Toledo, Ohio, written by the people who go there, for anyone who might want to go.

> “You can browse without buying.”
>
> “There’s seating where you can stay a while.”
>
> “This stretch of the river is quiet.”

It is a small public repository carried by GitHub, for [Orient](https://github.com/ragingapathy/orient), a personal map for getting to know a city. Orient is not required: every observation is plain JSON that anyone can read and reuse.

**Observations are about places, not people.** Nothing that names or identifies an employee, a customer, or a neighbour.

## Add an observation

In Orient, open a place, expand **People & notes**, and choose **Share this note**. Trim it to the part that would help someone else, tick the box, enter this repository as `ragingapathy/toledo-commons`, and press **Open on GitHub to finish**. GitHub opens with your contribution filled in; sign in as yourself, press **Propose new file**, then **Create pull request**. Your private note stays private.

You do not need Orient. A pull request that adds one new file under `contributions/` works too: see [CONTRIBUTING.md](CONTRIBUTING.md).

A check runs automatically and shows the maintainer a table of what you proposed. Observations are read by a person before they are merged, and you may be asked to change or drop one.

## Follow the commons

In Orient, open **Field kit → Place commons** and paste

```
https://raw.githubusercontent.com/ragingapathy/toledo-commons/main/snapshot.json
```

You choose which observations to bring onto your own map. Nothing is added until you accept it.

The same file is a plain [Orient commons bundle](https://github.com/ragingapathy/orient/tree/main/commons) (format `orient-commons`, version 1), so other tools can read it. If the commons grows past what one file can hold, it continues in `snapshot-2.json` and onward.

## Seed bundles

`contributions/seed-toledo-food-specials.json` is the maintainer's seed: the October 2026 Toledo food-specials research as a public bundle — 30 venues, 39 map pins, 46 recurring listings (58 claims; venues with more than one address get one claim per pin). Every claim carries its provenance: the published guide it was drawn from and the retrieval date. Two national-chain listings from the research are left out because a commons place needs a pin and they have no fixed Toledo address.

Specials change, so confirm with the venue before heading out. To correct a listing, contribute a new file that repeats its claim id with the new text, the same as any other correction.

## Corrections and removals

Contributions are never edited. To correct an observation, add a new contribution that repeats its id with the new text. To take one back, repeat it with `"status": "retired"`; the snapshot keeps it, marked as retired. If an observation names a person or is wrong about a place, open an issue and it will be retired.

## Licence

Observations, place names and pins are shared under [CC BY 4.0](DATA-LICENSE.md). Credit is to the commons name and contributor named in each file. The tools in `tools/` come from Orient under the [PolyForm Noncommercial License 1.0.0](LICENSE).

The maintainer's notes on running this repository are in [MAINTAINING.md](MAINTAINING.md).
