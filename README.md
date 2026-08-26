# FurEver Care - Responsive NextGen Pet Care Website

A custom single-page pet care portal built for the supplied SRS. It is not based on a ready-made website template.

## Technologies used
- HTML5 semantic layout, forms, Canvas, FileReader, Geolocation and Speech Synthesis
- CSS3 responsive design, gradients, transitions and keyframe animations
- Bootstrap 5.3.6 (layout/forms/modal utilities)
- JavaScript (SPA navigation, state, clock, geolocation, filtering, sorting, search, Canvas chart)
- jQuery 3.6.1 (XML AJAX, fades/animations and form interaction)
- JSON (products, adoptable pets, veterinarian case studies)
- XML (emergency contacts and shelter events)
- TXT (scrolling ticker updates)

## How to run
Because browsers block AJAX/fetch requests from `file://`, run the folder through a tiny local web server.

### Option 1 - VS Code Live Server
1. Open the `FurEverCare_Project` folder in VS Code.
2. Install/use the Live Server extension.
3. Right-click `index.html` and choose **Open with Live Server**.

### Option 2 - Python
Open a terminal inside this folder and run:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000` in a modern browser.

## Main user flows
### Pet Owner
1. Enter first name and choose Pet Owner.
2. Fill the pet profile form.
3. Dashboard provides Pet Profile, Feeding Guide, Grooming Video, Health Tips audio, Training Tips audio/text, Products with JSON search/filter/sort, Emergency XML data, Feedback UI, Contact/Google Map, About page, real-time clock, geolocation and simulated visitor counter.

### Veterinarian
1. Enter first name and choose Veterinarian.
2. Fill veterinarian profile; optional image preview uses FileReader and is never uploaded.
3. View profile, booked/available time slots and static JSON case studies.

### Animal Shelter / Rescue
1. Enter first name and choose Animal Shelter / Rescue.
2. View adoptable pet gallery with client-side type/age/search filtering.
3. View success stories, XML event announcements and shelter contact/Google Map.

## Data / storage rule
No data is written to a server. Form data is held only in browser session state. Static display content is loaded from JSON/TXT/XML files as required by the SRS.

## Internet assets
The design references pet photographs from Wikimedia Commons and Unsplash and embeds one YouTube grooming video. If the internet is unavailable, image elements fall back to a generated paw placeholder.

To make the photos local on a machine with internet access, run `python tools/download_images.py`; it downloads the configured image URLs into `assets/images/` and rewrites the matching project references to those local files.

## Important academic note
The supplied SRS itself states that ready-made templates should not be used and also says students should not copy code/content from GPT or other AI tools. If this is for formal assessment, review every file, understand the code, adapt it in your own style, and follow your institution's rules before submitting.

## Included demonstration
A short visual walkthrough is included at `docs/FurEverCare_demo.mp4`, together with `docs/preview.png`.


## Requested revision notes
The current build bundles its `<img>` assets locally, uses local Bootstrap Icons instead of emoji UI glyphs, removes the technology list from the footer, and applies stricter complete-email validation to the veterinarian and feedback forms. An updated demonstration clip is included at `docs/FurEverCare_demo.mp4`.
