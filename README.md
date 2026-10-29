# Project 2: *Spread*

This website sets Bruno Munari’s [“The Shape of Words” and “Poems and Telegrams”](https://readings.design/PDF/Bruno-Munari-The-Shape-of-Words-and-Poems-and-Telegrams-in-Design-as-Art-1971.pdf) as a responsive webpage for mobile, desktop and print. Munari argues that every word has a shape of its own, and that how a word is set changes how quickly, and how, it gets read. We wanted the page to work the same way, so instead of only describing his examples, we set them.

Our type choices come from Munari and the design culture around him. We based our headings on a page from the May 1970 issue of [*Domus*](https://domusweb.it/en/from-the-archive/2012/03/24/bruno-munari-art-director-1943-1944.html) (no. 486), the Italian design magazine where Munari had been art director and designer. The page repeats “eurodomus 3” in a heavy, tightly spaced lowercase sans serif, so we used Archivo Black in lowercase with tight letter-spacing for our headings, and Archivo for the body text for a similar feel. For the word experiments, we wanted to recreate the look of Munari’s own illustrations in the book. We used Julius Sans One for MAMMA and HULL / LIVERPOOL because its thin, even strokes are close to his hand-drawn lines, Permanent Marker for DAMO to match his marker lettering, and Archivo Black for jazz to get the same heavy, blocky shapes.

Our red and yellow come from Munari’s 1953 poster for Pirelli’s Coria soles. We use them to highlight the words Munari gives as examples, and the colour stays at the top in the sticky navigation, which links to the second reading and the original reading (PDF of the book).

On mobile the page is one column and reads in order. On desktop it becomes a two-column spread: each word experiment sits in the left column beside the paragraph that talks about it, like an illustration next to its caption. Most of the type sizes are built from one body size and one spacing unit, and `clamp()` lets the headings, the experiments and the text grow and shrink smoothly with the window. Lines like “slow down,” “onecanalsoeliminatethespacesbetweenthewords:” and the oversized punctuation are set the way they describe, so the layout slows you down where Munari says reading should slow down.

We also made sure the visual experiments don’t get in the way of screen readers. The decorative experiments, including DAMO and the row of punctuation marks, are hidden from screen readers so they don’t read out symbols or repeat words. Everything that changes how a word looks is done in CSS, while the HTML keeps the words as normal text: headings are typed normally and set in lowercase with CSS, Munari’s example words are typed in lowercase and shown in capitals with CSS, and the spaced-out HULL is a single word with letter-spacing added. We used `<mark>` for the words Munari gives as examples, so they’re marked for meaning, not just colour.

The print version keeps the colours, darkens the yellow so it still reads in grayscale, keeps the two-column spread, uses a fixed body size for paper, and starts “Poems and Telegrams” on a new page.

We worked on this together from start to finish. We sketched the mobile and desktop layouts side by side in Figma, then built the page through pair programming, taking turns writing the HTML and CSS. Along the way we got help from a tutor with the grid structure, and from our professors’ feedback on scaling, overflow and our type system, which we cite in comments in our CSS.

By Crystal Lam and Natay.

Based on [Project 2: Spread](https://typography-interaction-2627.github.io/project/2/).
