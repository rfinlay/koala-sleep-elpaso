# Koala® Center For Sleep & TMJ Disorders, El Paso

## A concept redesign of the location page, and why it is worth doing

Prepared for Jen | September 8, 2026

**See it first:** [https://rfinlay.github.io/koala-sleep-elpaso/](https://rfinlay.github.io/koala-sleep-elpaso/)

That link works on a phone. Open it there, because that is where most of your patients will find you.

---

## What this is

An independent, unsolicited redesign of the El Paso location page at koalasleepcenters.com. It was built as a working preview rather than a mockup, so what you are looking at is a real page, not a picture of one.

Every fact on it came from Koala's own website. The address, the hours, the services, Dr. Kalish's biography, the patient review, the medical disclaimers. Nothing was invented and nothing was embellished. The service links still point back to the real Koala pages.

It is marked so search engines will not index it, and it says plainly in the footer that it is an independent concept and not the official site. It cannot compete with the practice's own page in search results, and it is not pretending to be anything it is not.

---

## The single most important finding

**The El Paso phone number does not appear anywhere on the El Paso location page.**

This is not a subjective design opinion. It was verified directly against the page's source code:

| Check | Result |
|---|---|
| Clickable `tel:` phone links on the page | **0** |
| El Paso 915 number anywhere in the page code | **Not present** |
| Phone number in the structured data search engines read | **(309) 204-6490** |

That 309 number is the corporate office in Illinois. It is the number Google and other search engines are being handed when they read the El Paso page.

The actual El Paso number, **(915) 301-8387**, does exist on Koala's own appointments page. It is simply absent from the location page a patient is most likely to land on.

The "CALL CLINIC" button does work, but it loads the number through a script after the page arrives. On a slow phone connection, or if that script fails, a patient sees a button that does nothing. There is no plain phone number on the page to fall back on.

**Why this matters more than anything else here:** a person searching "sleep apnea El Paso" at eleven at night, on a phone, exhausted, is trying to do exactly one thing. Call someone. If tapping the obvious button does not immediately produce a phone number, they leave and call the next practice. That is a patient lost at the final step, after the practice already did the hard work of getting found.

In the redesign, the number is plain text at the top of the page, tappable, and repeated in the footer. It works with scripts disabled. It is the first thing on the page.

---

## What else is wrong with the current page

Each of these was measured against the live page, not estimated.

**It carries 203,206 bytes and 28 separate scripts to deliver one page of information.** The redesign delivers the same information in 33,054 bytes with zero scripts. That is roughly one sixth the weight. On the older phones and weaker signal common across El Paso and the surrounding communities the practice serves, that difference is the difference between a page that appears and a page someone gives up on.

**The same navigation block is repeated three times on one page.** The appointments link appears four times, patient reviews three times, sleep apnea eight times. A visitor scrolling the page passes the same fourteen links over and over. It reads as clutter, and it buries the things that actually matter underneath it.

**There is almost no visual hierarchy.** The page uses nine identical second-level headings, so the address, the hours, the directions and the service area are all styled the same way and sit in full sentences of prose. Nothing is scannable. A patient looking for "are they open Friday" has to read paragraphs to find out.

**Dr. Kalish's biography is one undifferentiated block of text.** This is the most costly problem on the page, because the content itself is genuinely strong. Army Advanced Education in periodontology. Two years of humanitarian missions in Asia. Dentist to special operations soldiers with 1st Special Forces Group, Airborne. A three-year Army Periodontic Residency completed alongside a master's degree. Advanced training in treating snoring, sleep apnea and TMD.

In El Paso, a city built around Fort Bliss, that is not just a credential. It is the reason a patient chooses this practice over another one. Right now it is a paragraph a visitor has to work through. In the redesign it leads, with the service history given its own space.

**The directions section is four raw Google Maps links in a row.** Canutillo, Vinton, Prado Verde, Santa Teresa. Useful information presented as a wall of blue text.

**There is no warmth on a page about an intimate problem.** People come to this practice because they cannot sleep, they snore badly enough that it is affecting their marriage, or their jaw hurts constantly. The current page reads like a directory listing. It never once acknowledges what the person reading it is actually going through.

---

## What the redesign changes

**It leads with the patient, not the practice.** The first thing a visitor reads speaks to being exhausted, snoring, or in pain, followed immediately by a phone number and a way to book.

**Phone number in plain text, at the top, tappable, no script required.**

**Services in a scannable grid** instead of a repeated list, each linking to the real Koala pages.

**Dr. Kalish's background gets real design attention**, with his military service and credentials leading rather than buried.

**Location, hours, map link and the four surrounding communities** in one clean card a patient can read in five seconds.

**The patient review presented as a real testimonial**, quoted properly and attributed.

**Built for a phone first.** Verified with no sideways scrolling at 375 pixels wide, which is a standard iPhone.

**Accessible.** Proper heading structure, real contrast, keyboard focus states, alt text on images, and it respects a visitor's reduced-motion setting. This matters on a medical site, and it is also what the ADA notice already in Koala's own footer is promising.

---

## Outcomes this is aimed at

Not traffic. Not rankings. Patients in chairs.

**A phone number that always works.** Every visitor who wants to call can call, immediately, without depending on a script loading. Today that is the single biggest hole in the page.

**Fewer people leaving before the page loads.** Roughly one sixth the page weight means the page arrives quickly on a phone, on a weak signal, in a parking lot, at midnight.

**Search engines seeing an El Paso practice.** Right now the structured data on the El Paso page carries an Illinois phone number. Correcting that helps the practice appear as a genuinely local business.

**Dr. Kalish's credentials doing the work they should.** His Army service and periodontic training are a real competitive advantage in this city and are currently invisible. Making them prominent gives a hesitant patient a reason to choose this practice.

**A page that reaches the whole service area.** Canutillo, Vinton, Prado Verde and Santa Teresa are named clearly rather than hidden in map links.

**A page that feels like it was made for people who cannot sleep.** That is not decoration. It is the difference between a visitor who books and one who keeps looking.

---

## What it would take to bring it live

Deliberately short, because the work is already done.

**1. The practice confirms the facts.** The phone number, the hours, and Dr. Kalish's biography as written. Everything was pulled from Koala's own site, but it should be confirmed by someone at the practice rather than trusted from a scrape.

**2. Real photography.** The page currently has a labeled placeholder where Dr. Kalish's photo belongs. One good headshot, and ideally a few photos of the office, would replace it.

**3. Koala corporate signs off.** This is a franchise location on a corporate website. The El Paso page is one page in a larger site that also covers Peoria, Bloomington and Wausau. Any change to it goes through whoever controls koalasleepcenters.com. That is the real gate here, and it is a conversation, not a technical problem.

**4. The complete footer notices.** The preview carries the four core medical and legal notices: emergency 911, results may vary, not a substitute for medical advice, and ADA accommodation. Koala's real footer also includes photo and model disclosure, SMS consent language, and third-party tracking notices. A live version would carry all of them.

**5. Publish.** Once the above is settled, the page is a single self-contained file. There is no framework, no build process, and no ongoing dependency. It can be dropped in.

---

## The honest part

**This was not requested by Koala.** It is an independent concept built to show what the page could be. It is marked as such, and it is set so search engines will not index it.

**The corporate gate is real.** The El Paso location does not control koalasleepcenters.com on its own. That is the practical obstacle, and it is worth knowing before anyone gets attached to the idea.

**The phone number finding stands on its own regardless.** Even if nothing else here is ever used, the fact that the El Paso location page contains no El Paso phone number, and hands search engines an Illinois one, is worth passing to whoever maintains the site. That is a fixable problem costing the practice real calls right now.

---

## Links

**Live preview:** [https://rfinlay.github.io/koala-sleep-elpaso/](https://rfinlay.github.io/koala-sleep-elpaso/)

**Current page:** [https://www.koalasleepcenters.com/locations-el-paso-tx](https://www.koalasleepcenters.com/locations-el-paso-tx)

Open both on a phone, one after the other. The difference is clearest there.
