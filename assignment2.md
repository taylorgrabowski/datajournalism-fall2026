# Assignment 2: Build onto an Existing Database

## 1. Original database
[Billboard Hot 100 chart](https://www.billboard.com/charts/hot-100/) (and the accompanying [Wikipedia tracking page, "List of Billboard Hot 100 top-ten singles in 2026"](https://en.wikipedia.org/wiki/List_of_Billboard_Hot_100_top-ten_singles_in_2026), used to compile the current top-10 list).

## 2. About the original database
The Hot 100 is Billboard's flagship singles chart, published weekly since 1958. It is compiled by *Luminate Data* and ranks songs using a formula that combines physical and digital sales, radio airplay audience impressions, and official on-demand streaming activity in the United States.

**Scope and limitations:**
- **Geographic scope:** U.S. only — streaming, airplay, and sales are all measured domestically, so it does not reflect global popularity.
- **Date range:** Weekly, ongoing since 1958; I used the chart as of the week of September 5, 2026.
- **Definitions:** "Chart position" is a composite score, not a single measurable quantity like "copies sold" — the exact weighting of streams vs. airplay vs. sales is proprietary to Billboard/Luminate, so two songs with very different streaming numbers can rank the same.
- **Missing information:** The chart itself lists only title, artist, and chart performance metrics (position, weeks charted, peak position). It does not include genre, which is a subjective, industry-assigned classification rather than a chart metric.
- **Collection method:** Automated data feeds from streaming services, Nielsen/Luminate-monitored radio airplay, and retail/digital sales reporting.

## 3. The reporting question
**Which genres dominate the current Billboard Hot 100 top 10, and how much does country music currently dominate the pop mainstream?**

Genre is newsworthy here because the Hot 100 is marketed as an "all-genre" chart, but the industry and audiences often want to know whether that's true in practice — whether one genre (in this case, country) is disproportionately capturing mainstream attention, and whether hit-making has become more genre-blended (e.g., country-pop crossovers, K-pop/psych-rock mashups) rather than sorted into clean genre boxes.

## 4. Expanded dataset
**[assignment2_hot100_genres.xlsx](computer:///mnt/user-data/outputs/assignment2_hot100_genres.xlsx)**

*(Upload this file to Google Sheets or GitHub and swap in that link before submitting — see note below.)*

The new `Genre` column was researched using each song's Wikipedia entry (which lists genre tags sourced from label/press materials) or, where no dedicated song article existed, the artist's general genre classification. Every row includes a `Source` link and a `Notes` field documenting any judgment calls.

## 5. Judgment calls and unusual records
- **Multiple genre tags per song:** Most songs' Wikipedia info boxes list 2–4 genre tags rather than one clean label (e.g., "Hate That I Made You Love Me" is tagged pop, alt-pop, R&B, and synth-pop). I kept all listed tags rather than picking one, since collapsing to a single genre would have been my own editorial call, not a sourced fact.
- **"Dracula" (Tame Impala & Jennie):** The version currently charting is a remix featuring Jennie, but Wikipedia's genre classification is attached to the original 2025 Tame Impala solo release, since the remix doesn't have its own dedicated entry. I noted this in the Notes column rather than guessing at a genre change.
- **"So Easy (To Fall in Love)" (Olivia Dean):** No dedicated Wikipedia song article existed, so I used her artist-level genre classification (Pop Soul / Indie Pop / Neo Soul) instead of a song-specific one — flagged in Notes.
- **Country dominance:** 6 of the 10 songs currently in the top 10 are classified as country or country-pop, including three from Ella Langley alone and two featuring Morgan Wallen — a useful, concrete finding for the reporting question above.

## 6. AI disclosure
I used Claude (Anthropic) to help identify the current Billboard Hot 100 top-10 songs (via web search, since the chart updates weekly and is beyond any static knowledge base), and to research and verify each song's genre classification from Wikipedia and news sources. 
