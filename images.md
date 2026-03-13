# Image Manifest — BC Family Trip 2026

Replace gradient placeholders with real photos. For each slot, add an image file to the `images/` folder and update the corresponding `src` or `style="background-image: url(...)"` in the HTML.

## Recommended image sources

- **Wikimedia Commons** — free, verified, CC-licensed. Search at [commons.wikimedia.org](https://commons.wikimedia.org)
- **Tourism BC / Super Natural BC** — official tourism images at [supernaturalbc.com](https://www.supernaturalbc.com)
- **BC Parks** — [bcparks.ca](https://bcparks.ca) for park-specific photos
- **Your own photos** — after the trip, replace placeholders with family shots to make this a travel journal

## Hero images (large, landscape, ~1600px wide)

| Page | Section | Suggested subject | File |
|---|---|---|---|
| index.html | Main hero | Vancouver coastline with mountains | `images/hero-vancouver.jpg` |
| itinerary.html | Hero | Sea-to-Sky Highway view | `images/hero-seatosky.jpg` |
| logistics.html | Hero | BC Ferries on water | `images/hero-ferries.jpg` |
| kids.html | Hero | (Uses CSS gradient — no image needed) | — |
| appendices.html | Hero | Old-growth forest canopy | `images/hero-forest.jpg` |

## Segment cards (index.html, ~600px wide)

| Card | Suggested subject | File |
|---|---|---|
| Downtown Vancouver | Vancouver skyline from Stanley Park | `images/card-vancouver.jpg` |
| Deep Cove | Deep Cove bay with kayaks and mountains | `images/card-deepcove.jpg` |
| Sea-to-Sky & Whistler | Highway 99 with Howe Sound and mountains | `images/card-seatosky.jpg` |
| Vancouver Island | Wild Pacific coast (Tofino or Ucluelet) | `images/card-island.jpg` |
| Sunshine Coast | Pender Harbour from above | `images/card-sunshine.jpg` |
| Vancouver Wind-Down | English Bay or Kitsilano Beach | `images/card-final.jpg` |

## Itinerary segment images (full-width, ~1200px wide)

| Segment | Suggested subject | File |
|---|---|---|
| Segment 1: Vancouver | Vancouver skyline at dusk | `images/seg-vancouver.jpg` |
| Segment 2: Deep Cove | Deep Cove inlet with boats | `images/seg-deepcove.jpg` |
| Segment 3: Whistler | Sea-to-Sky Highway or Whistler village | `images/seg-whistler.jpg` |
| Segment 4: Vancouver Island | Tofino beach or Cathedral Grove | `images/seg-island.jpg` |
| Segment 5: Sunshine Coast | Coastal dock or Pender Harbour | `images/seg-sunshine.jpg` |

## Kids Corner images (mosaic tiles, ~600px wide)

### Beaches section
| Slot | Suggested subject | File |
|---|---|---|
| 1 (span-2) | Rathtrevor Beach sand flats at low tide | `images/kids-rathtrevor.jpg` |
| 2 | Tide pools with sea stars | `images/kids-tidepools.jpg` |
| 3 | Children playing at sandy beach | `images/kids-beachplay.jpg` |
| 4 (span-2) | Chesterman Beach, Tofino | `images/kids-chesterman.jpg` |

### Wow moments section
| Slot | Suggested subject | File |
|---|---|---|
| 1 | Peak 2 Peak Gondola cabin | `images/kids-gondola.jpg` |
| 2 (span-2) | Cathedral Grove giant trees | `images/kids-cathedral.jpg` |
| 3 (span-2) | Mountain lake reflection | `images/kids-lake.jpg` |
| 4 | Vallea Lumina forest lights | `images/kids-lumina.jpg` |

### Animals section
| Slot | Suggested subject | File |
|---|---|---|
| 1 | Bald eagle in tree | `images/kids-eagle.jpg` |
| 2 | Black bear on beach | `images/kids-bear.jpg` |
| 3 (span-2) | Harbour seals on rocks | `images/kids-seals.jpg` |
| 4 | Mountain/forest habitat | `images/kids-forest.jpg` |
| 5 (span-2) | Colourful starfish in tide pool | `images/kids-starfish.jpg` |

### Getting wet section
| Slot | Suggested subject | File |
|---|---|---|
| 1 (span-2) | Kayaking on calm water (Deep Cove or Indian Arm) | `images/kids-kayak.jpg` |
| 2 | Surfing at Cox Bay, Tofino | `images/kids-surfing.jpg` |

### Short walks section
| Slot | Suggested subject | File |
|---|---|---|
| 1 (span-2) | Rainforest boardwalk trail (Pacific Rim) | `images/kids-rainforest.jpg` |
| 2 | Shannon Falls or Brandywine Falls | `images/kids-waterfall.jpg` |

## How to add images

1. Save your image to the `images/` folder with the filename from the table above
2. In the HTML file, find the `<div class="img-placeholder"` or `<div class="card-img"` or hero `<div class="hero-bg"` for that section
3. Replace the gradient `style` with an image reference:

**For hero backgrounds:**
```html
<!-- Before -->
<div class="hero-bg" style="background: linear-gradient(...);">
<!-- After -->
<div class="hero-bg" style="background-image: url('images/hero-vancouver.jpg');">
```

**For card images:**
```html
<!-- Before -->
<div class="card-img" style="background: linear-gradient(...);">Vancouver</div>
<!-- After -->
<img class="card-img" src="images/card-vancouver.jpg" alt="Vancouver skyline">
```

**For kids mosaic tiles:**
```html
<!-- Before -->
<div class="img-placeholder span-2" style="background: linear-gradient(...);">🏖️ Sandy Beach</div>
<!-- After -->
<img class="span-2" src="images/kids-rathtrevor.jpg" alt="Rathtrevor Beach" style="border-radius: 8px; width: 100%; height: 200px; object-fit: cover;">
```

## Wikimedia Commons quick-start

To find a specific image on Wikimedia Commons:

1. Go to [commons.wikimedia.org](https://commons.wikimedia.org)
2. Search for the location (e.g., "Shannon Falls")
3. Click an image you like
4. Click "Download" → choose a size (800px or 1024px width is good)
5. Right-click the preview → "Save image as..." → save to your `images/` folder
6. Attribution: note the author and licence for the README credits section

---

*This manifest was generated alongside the BC Family Trip 2026 site. All gradient placeholders work as-is — images are an enhancement, not a requirement.*
