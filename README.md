# Koala® Center For Sleep & TMJ Disorders, El Paso: concept redesign

An **unsolicited concept redesign** of the El Paso location page for Koala® Center For Sleep & TMJ Disorders. It is a design preview only. It is not the official website and is not affiliated with or endorsed by Koala® Centers.

**Live preview:** https://rfinlay.github.io/koala-sleep-elpaso/

**Source page being redesigned:** https://www.koalasleepcenters.com/locations-el-paso-tx

## What it is

- A single self-contained `index.html`. No build step, no framework, no dependencies beyond Google Fonts.
- `<meta name="robots" content="noindex, nofollow">` so the preview never competes with the real site in search.
- Mobile-first and responsive. Verified at 375px and 1440px with no horizontal scroll.
- Every clinic fact (address, hours, doctor bio, services, service area, patient review, disclaimers) was taken from the live Koala® site. Nothing was invented.
- All service links point to the real pages on koalasleepcenters.com.

## Phone number provenance

The El Paso clinic number shown, **(915) 301-8387**, comes from Koala's own El Paso appointments page (https://www.koalasleepcenters.com/locations-el-paso-tx-appointments). It appears there in the page's meta description, Open Graph description, and Yoast JSON-LD, paired with the El Paso street address ("6901 Helen of Troy, Ste D-2 El Paso, TX 79911. Call (915) 301-8387"). It was not taken from the general location page, which only exposes the corporate (309) number in its schema markup.

## TODO before this could ever go live

- Replace the "Photo of Dr. Kalish here" placeholder with the practice's own photography.
- Have the clinic confirm the phone number and hours directly.
- Koala's full footer includes additional notices (photo/model disclosure, SMS consent, third-party tracking). This preview carries the four core medical/legal notices only; a production build should carry the complete set.
