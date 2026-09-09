# Koala Center For Sleep & TMJ Disorders
## Website Template Findings Report: All Locations

**Prepared:** September 8, 2026
**Scope:** Public marketing pages only. Nothing touching patient intake, patient communication, or protected health information.
**Method:** Direct measurement of all four live location pages on September 8, 2026. Read-only throughout. No contact was made, no forms were submitted, no systems were accessed.

**Live version of this document:** https://rfinlay.github.io/koala-sleep-elpaso/info.html
**Concept page:** https://rfinlay.github.io/koala-sleep-elpaso/

---

## 1. The Business Problem

**Every Koala location page tells search engines the clinic is in Dunlap, Illinois.**

The four location pages are a single template with the headline text swapped. Everything underneath is shared, including the part that should be different at every location: the business identity itself.

Each page carries a block of machine-readable code that tells search engines who and where this business is. On all four pages that block is identical. It names one street address, one ZIP code, one set of GPS coordinates and one phone number, all belonging to the Illinois clinic.

So the El Paso page publishes El Paso in its visible text and **Dunlap, Illinois** in the code Google actually reads. Bloomington does the same. So does Wausau. Three of the four locations are, in machine-readable form, claiming to be somewhere they are not.

**Why it matters commercially.** Marketing spend on any one location routes patients to a page that quietly contradicts that location's own Google Business Profile. The contradiction is invisible on the page, invisible to automated testing, and repeated everywhere.

**Why it is worth fixing once.** Because it is one template, this is not four repairs. It is one correction that propagates to every location, and to every location added later. The same property that caused the problem is what makes it cheap to solve.

---

## 2. The Existing Vendor, Stated Up Front

The site runs on WordPress under a theme named `patientgain-2021-april`. That is the signature of **PatientGain**, a healthcare marketing platform that sells HIPAA-compliant sites on a recurring per-location contract.

We name them because pretending otherwise would waste everyone's time. There is an incumbent, that relationship presumably exists for good reasons including compliance, and nothing in this document asks anyone to unwind it.

**These findings are handed over as a defect report.** If PatientGain fixes them, the problem is solved and that is a good outcome. Every item below is specific enough to forward and act on directly.

**Scope is deliberately narrow.** Public marketing pages only: structured data, images, page speed, navigation and metadata. Nothing touching patient intake, patient communication, or any system carrying protected health information. That boundary exists so the compliance question never has to be reopened.

---

## 3. The Evidence

All four location pages were downloaded and analyzed on September 8, 2026.

| Finding | Measurement | Pages affected |
|---|---|---|
| Address in structured data | Dunlap, IL 61525, with Illinois GPS coordinates | 4 of 4 |
| Clickable phone links (`tel:`) | **0** | 4 of 4 |
| Phone in structured data | (309) 204-6490, the Illinois number | 4 of 4 |
| Mobile largest contentful paint | **6.2 seconds** (Google's "poor" band starts at 4.0) | 4 of 4 |
| Desktop performance score | 98 to 100 | 4 of 4 |
| Automated SEO score | **100 out of 100** | 4 of 4 |

### 3.1 The El Paso page's main photograph is the Bloomington clinic

The desktop banner on every location page is the same file, `bloomington-header-img-desktop.jpg`. On the El Paso page its alt text reads "Welcome to Koala Center For Sleep & TMJ Disorders in El Paso, TX." The label says El Paso. The photograph is Bloomington.

The mobile version is worse, because it looks localized and is not. The file named `el-paso-mobile-header.jpg` is byte-for-byte identical to the Bloomington file. Same size, same checksum. A copy was renamed and shipped.

**This also governs link previews.** The social share image on all four pages is that same Bloomington photograph. Every time anyone shares any Koala location link, in a text message or on social media, the thumbnail is Bloomington.

### 3.2 "Call Clinic" does not call the clinic

The link appears three times per page. On every location it redirects to one generic corporate contact page, where the only phone number present is the Illinois number, and it is not tappable.

### 3.3 Mobile load time is 6.2 seconds, on all four

Google's threshold for a good experience is 2.5 seconds; above 4.0 is rated poor. Every location page measures exactly 6.2 seconds on mobile. All four landing on the same figure is itself proof of a shared template.

### 3.4 A map downloads on every page and never appears

The Google Maps library is the single largest asset on the page at 378 KB. It loads, throws an error because the element it needs is missing, and no map is ever shown. That weight is paid on every visit for nothing.

### 3.5 The same menu is stamped in three times

Within one page, the sleep apnea link appears eight times, TMJ eight times, snoring eight times, appointments three times. The same inventory repeats in the header, an inline block and the footer.

### 3.6 Automated testing scores this a perfect 100 for SEO

Every location page scores 100 out of 100 on the standard SEO audit while telling Google it is in the wrong state. Automated tools check whether the code is valid, not whether it is true. Desktop performance scores 98 to 100 as well, so a quick test on a laptop shows almost nothing wrong.

**If anyone checks this, ask them to test on a phone.** That is where the 6.2 seconds shows up, and it is where the patients are.

---

## 4. Corrections and What Each One Buys

Ordered by value against effort. Every one is a template-level change, which means it lands at all four locations at once.

| Correction | Outcome |
|---|---|
| **Give each location its own business record** in the structured data: real address, coordinates, and local phone | Your own website stops contradicting your Google Business Profile. Cheapest item on the list, no argument for leaving it |
| **Make every phone number tappable**, at the top of each page plus header and footer | The patient who is ready to call can call, instead of arriving at a contact page for another state |
| **Localize photography and the share image** so each location shows its own clinic | A shared link previews the right place; a prospective patient recognizes the office they will walk into |
| **Remove the map library that never renders** | 378 KB and a JavaScript error removed from every page load. Largest single speed win, and it costs nothing in features because the map never appears |
| **Bring mobile load under 2.5 seconds**: modern image formats, deferred offscreen images, connection hints, unused code removed | Holds the visitor who arrived from a phone search late at night, which is when people research sleep problems |
| **Give the page a hierarchy**: one path from problem to treatment to doctor to booking | A visitor can find the answer to their question without hunting for it |
| **Lead with the doctor's credentials** rather than burying them mid-paragraph | In a city built around a military installation, specialist and service credentials are the reason a patient chooses one clinic over another |
| **Fix the small breakages**: a misspelled internal link, two JavaScript errors per page load, hours that disagree between the location page and the FAQ page | Removes the small signals that nobody is watching |

---

## 5. What This Document Does Not Claim

- **Not a ranking promise.** No rankings, Business Profiles or directory listings were measured. Proximity to the searcher dominates local search and no website change affects it. The defensible claim is narrower: the site contradicts itself, and that is free to fix.
- **Not an accessibility crisis.** Accessibility already scores 99 out of 100. Any work should be held to leaving that score untouched or better.
- **Not a broken site.** Mobile performance scores in the low seventies. That is mediocre, not broken. The unambiguous failures are the 6.2 second load and the wrong location data.
- **Not a criticism of any location.** These are template-level defects that no individual location controls or could have prevented.
- **Not a compliance proposal.** Nothing proposed touches intake, patient communication or protected health information.
- **Not an assumption about the contract.** No knowledge is claimed of any agreement, term, renewal date or scope with the existing vendor.

---

## 6. Path Forward

1. **Verify one finding yourself.** Open any location page on a phone and try to tap the phone number. Then share the link and look at the preview image. Under a minute, and neither requires taking anyone's word for it.
2. **Confirm the correct local phone number for each location.** More than one number appears in public sources for at least one location. This should be settled internally, because it is the one input that has to come from you.
3. **Forward the findings to whoever maintains the site.** Every item is specific enough to act on. The structured-data correction and photography swap are likely a single day of work for whoever already has access.
4. **Decide whether the template gets corrected or refreshed.** Correcting the existing template is the smaller path. The concept page is a reference point for that decision, not a proposal.
5. **Roll the correction across all locations at once**, with mobile load time and the accessibility score used as the before-and-after acceptance test.

---

## 7. Notes on Sourcing

1. Address, coordinates, phone and share image findings taken from the published source of all four location pages on September 8, 2026, and independently reproducible.
2. Image duplication confirmed by file checksum comparison between the Bloomington and El Paso mobile header files.
3. Performance figures measured with Lighthouse 12.8.2 against the live pages under standard mobile throttling. Lab measurements, not field data.
4. Load-time thresholds are Google's published Core Web Vitals bands: 2.5 seconds or less is good, above 4.0 seconds is poor.
5. The platform vendor is identified from the publicly visible theme name in the page source. No contract, term or commercial relationship is known or implied.
6. No rankings, Google Business Profile data, or citation footprint were measured. No claim about search position is made anywhere in this document.

---

*Independent concept and findings report. Not affiliated with, endorsed by, or commissioned by Koala Center For Sleep & TMJ Disorders or any vendor named in this document. The concept page is marked so search engines will not index it, collects no patient information, and contains no working forms.*
