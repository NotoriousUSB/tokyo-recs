# Tokyo Recs — Real Image Sourcing + Integration

Open the repo at `/Users/mcfly/.openclaw/workspace/tokyo-recs`.

We need **real, place-specific images** for every spot in the Tokyo guide.  
No generic Tokyo filler. No fake stock vibe. No AI images.

## Objective

Source and integrate **real images** for every place in the guide so the site no longer uses generic placeholder photography.

## Places to source

Source **1 strong primary image per place**.  
If a place has multiple good options, save up to **3 candidates**, but make sure at least **1 final chosen image** is ready to use.

### Shopping
1. Kapital
2. NUBIAN
3. GR8
4. Dover Street Market Ginza
5. Omotesando Avenue

### Eat
6. Yoroniku
7. Yakiniku Ushigoro
8. Tofuya Ukai
9. Omakase Sushi
10. Totti Candy Factory
11. INITIAL

### Drink
12. New York Bar
13. Bar Zoetrope

### Experience
14. Shibuya Crossing & Shibuya Sky
15. teamLab Borderless
16. Meiji Jingū
17. Golden Gai
18. Art Archive Gallery Shibuya

## Image criteria

For every place, find an image that is:
- clearly the **actual place**
- visually strong enough to be a **hero/card image**
- not a generic neighborhood shot unless the place itself is the neighborhood/street experience
- not blurry, tiny, over-compressed, watermarked, or obviously scraped junk
- not AI-generated
- not random stock photography pretending to be the location

## Preferred source order

Use sources in this order when possible:
1. Official venue/site/press images
2. Wikimedia Commons
3. Clearly attributable editorial/travel sources
4. Google Maps/business photos only if they are clearly the place and usable

Avoid:
- Unsplash generic Tokyo photos
- Pinterest junk
- suspicious SEO/travel spam sites
- images that will obviously 404 or block hotlinking later

## Special guidance by place

- **Kapital** — storefront/interior/product environment that clearly feels like Kapital Tokyo, not generic fashion retail
- **NUBIAN** — real store interior/exterior, ideally Harajuku or Shibuya PARCO
- **GR8** — Laforet/GR8 interior or storefront, something unmistakably GR8
- **Dover Street Market Ginza** — building/interior that clearly reads DSM Ginza
- **Omotesando Avenue** — architectural street view is okay because the avenue itself is the destination
- **Yoroniku** — actual restaurant interior/course/meat presentation from the real restaurant
- **Yakiniku Ushigoro** — actual restaurant/cut presentation/interior, not generic yakiniku
- **Tofuya Ukai** — garden/exterior/interior with strong atmosphere
- **Omakase Sushi** — use a **real Tokyo omakase counter image**; if this is too generic as a concept, note that clearly
- **Totti Candy Factory** — giant rainbow cotton candy / storefront / real in-shop visual
- **INITIAL** — actual parfait/interior/brand environment
- **New York Bar** — use the actual bar interior if possible, not just skyline/generic cocktail imagery
- **Bar Zoetrope** — actual tiny whisky/cinema bar feel
- **Shibuya Crossing & Shibuya Sky** — can use either one strong combined-feel image or two candidates; final should represent the experience cleanly
- **teamLab Borderless** — actual installation imagery from the real venue
- **Meiji Jingū** — shrine/torii/approach path
- **Golden Gai** — real alley/bar exterior atmosphere
- **Art Archive Gallery Shibuya** — actual gallery image if this place is legit and worth adding; if not, flag it

## File handling

Create/use:
- `/Users/mcfly/.openclaw/workspace/tokyo-recs/assets/`

Save final chosen images there.

## Naming convention

Use predictable lowercase kebab-case filenames:

- `kapital.jpg`
- `nubian.jpg`
- `gr8.jpg`
- `dover-street-market-ginza.jpg`
- `omotesando-avenue.jpg`
- `yoroniku.jpg`
- `yakiniku-ushigoro.jpg`
- `tofuya-ukai.jpg`
- `omakase-sushi.jpg`
- `totti-candy-factory.jpg`
- `initial.jpg`
- `new-york-bar.jpg`
- `bar-zoetrope.jpg`
- `shibuya-crossing-sky.jpg`
- `teamlab-borderless.jpg`
- `meiji-jingu.jpg`
- `golden-gai.jpg`
- `art-archive-gallery-shibuya.jpg`

If source format is png/webp and that’s better, that’s fine, but keep names stable.

## Compression / asset standards

Optimize for web:
- target roughly **1600px wide max** for landscape images
- keep file sizes ideally around **150KB–500KB**
- avoid giant multi-megabyte originals unless absolutely necessary
- preserve enough quality that it still feels premium on mobile
- prefer jpg for photos unless png/webp is clearly better

## Required output

1. Put the final chosen images into `/assets/`
2. Update `index.html` so each place points to its local asset path
3. If a place cannot be sourced confidently, do **not** leave fake filler in place:
   - either use a clearly real but slightly less ideal place image
   - or flag that exact place as unresolved in a short note

## Tracking file

Also create:
`/Users/mcfly/.openclaw/workspace/tokyo-recs/image-log.md`

For each place, record:
- place name
- chosen asset filename
- source URL
- source type
- short note on why it matches
- any rights/hotlink risk note
- unresolved issues if any

## Success criteria

- Every place has a real, place-specific image or a clearly flagged unresolved status
- No generic Unsplash/Tokyo placeholder images remain
- Assets are local in `/assets/`
- Filenames follow the naming convention
- `index.html` points to local assets
- `image-log.md` exists and documents the sources
