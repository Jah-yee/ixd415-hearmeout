# Issues

Brainstorm of places where students can make a visible difference. Each of these gets filed as a GitHub issue. Labels: `good first issue`, `html`, `css`, `js`, `content`, `a11y`.

Roughly ordered easy to hard. The first handful are small enough that someone can finish them in a few minutes once they've figured out the branch/PR mechanics.

## Easy (good first issue)

1. **Give the page a real title** - The browser tab says "Untitled". Change the `<title>` to something sensible. `html`
2. **Fix the typo in the intro** - "presentaton" should be "presentation". Read the rest of the copy while you're there. `content`
3. **Link to the course site** - Add a link to https://ixd415.mattkirkland.com somewhere obvious, probably the header or footer. `html` `content`
4. **Link to the book** - The "Book on loan" is Russell Davies' *Everything I Know about Life I Learned from PowerPoint*. Mention it in the intro and link to it. `content`
5. **Fill in the Rules section** - It currently says "TODO". Pull the rules from the course site: 5 min minimum, 10 max; the deck isn't the deliverable, you are; theme is "hear me out". `content`
6. **Add a 404 page** - GitHub Pages will serve `404.html` if it exists. Make a small one that links back home. `html`
7. **Footer: link to this repo** - Add a link to the GitHub repo in the footer so people can find the issues. `html`

## Medium

8. **Human-readable dates** - Dates are `09-09-2026`. Format them as `Wed, Sep 9` or similar. Do it in the HTML, or in JavaScript if you'd rather. `content` `js`
9. **Make the "no class" week look different** - Week 8 says NO CLASS in two cells. Give that row a class and style it so it reads as a gap, not a presenter. `html` `css`
10. **Explain the "Book on loan" column** - It isn't obvious what that column means. Add a short note under the table or a footnote. `content`
11. **Decide what goes in the empty cell** - Week 16, "Book on loan" is blank. Figure out what should be there (back to Matt? a dash? nothing?) and make it consistent. `content`
12. **Use semantic HTML** - The page uses `<div class="top">` and `<div class="bottom">`. Replace with `<header>`, `<main>`, `<footer>`. Check the table too: it should have a `<thead>`, `<tbody>`, and `scope` on the header cells. `html` `a11y`
13. **Add a table caption** - Screen readers announce captions; the table has none. `html` `a11y`
14. **Make the table work on a phone** - At narrow widths the table is cramped. Make it readable at 375px wide (horizontal scroll, stacked cells, your call). `css`
15. **Pick a typeface and a measure** - It's default serif with no max-width. Choose fonts and a comfortable line length. Keep it plain; this is not a redesign. `css`
16. **Dark mode** - Respect `prefers-color-scheme: dark`. `css`
17. **Print stylesheet** - Someone might print this and stick it on a wall. Hide what doesn't matter, make the table fit on one page. `css`

## Harder

18. **Highlight the current week** - `script.js` has a `highlightCurrentWeek()` stub. Implement it: find the row whose date is this week and add a class. Style the class in CSS. `js` `css`
19. **"Up next" callout** - Add a box near the top that says who presents next and when, computed from the table. `js` `html`
20. **Dim past weeks** - Weeks that have already happened should look done (greyed out, struck through, whatever). Computed in JS, styled in CSS. `js` `css`
21. **Days-until countdown** - "Next presentation in 6 days." Updates based on today's date. `js`
22. **Download the schedule as a calendar file** - Generate an `.ics` file from the table so people can add the dates to their calendar. `js`
23. **Add a "talk title" column** - Presenters can add their talk title once they know it. Start with the column and blank cells; each presenter fills in their own row via a PR. `html` `content`
