:::newsheader{data-tags="{'media' : 'news/books.png', 'dateDay' : 15, 'dateMonth' : 'APR', 'description' : 'The birth of Tales Tech Encyclopedia!'}"}

# TTE

:::

TTE is fueled by the Unified toolchain to parse tech documents and news into the website. It supports GFM (Github Flavored Markdown) and multiple others functionalities such as emojis (:joy:), math and custom directives (from commonmark) for media and tag handling.

:::tagging{data-tags="{'media' : 'URL HERE', 'forced' : true, 'versions' : ['All versions of TTE!'], 'timestamp' : 'time', 'todo' : true}"}
In the future, special icons will appear just below this paragraph! To use this special tagging, just follow examples for now.
:::

Project started 12th of April.

:::tagging{data-tags="{'versions' : ['All versions of TTE!'], 'todo' : true}"}

### We can also tag headers! And not use all options!

:::

The toolchain: Unified, esbuild, prettier, npm. Only javascript and css.

## Table of Contents

## TOC Explanations

TTE also has automatic Table of Contents creation. Just add a markdown heading after the Table of Contents header is defined! It also obtains headings from inside custom directives.

> ## Example
>
> This, since it is a block quote, will not enter the ToC.

Due to GFM, task-list can be used to track progress in different topics during documents:

## Task-list for next versions

(!) For bug fixes. Rest for base functionality.

- [x] Basic inspiration. (https://ballsystemgroup.it/it/about/) + design images on TTE folder.
- [x] Start of project.
- [x] Nav bar definition. + Placeholders for section heading and content.
- [x] Logo and icon art. Fonts to be used in the project.
- [x] Interactive logo on nav-bar, used to return to homepage/news. (Also added placeholder search box)
- [x] Tab bar definition.
- [x] Tab bar created with scroll and fade. Tooltips added to buttons.
- [x] Considerations on how to handle tech documents. Needs to be very human readable to allow more contributions. Needs to be able to be digested by JS. Solution: a lightweight markup language.
- [x] Checked different definitions or Markdown. Decided on GFM due to ease-of-use, being modern and able to be read easily while in Github Pages.
- [x] Libraries to treat Markdown. Used Unified due to the possible customizations.
- [x] Research on Markdown and how to use on browser. After a lot of searching esbuild was selected to bundle the dependency code to be used on browser.
- [x] Demo News page created.
- [x] Code reformat to keep things simpler and separate (separate markdown handling from page animations/commands).
- [x] Sample page is injected into content section with unified.
- [x] Research on other possible plugins to help user and content customization.
- [x] TOC, math, proper GFM, and emoji support added.
- [x] Research on tagging methods to add specific icons (version, media, TODO, and time). Either macro blocks, generic extensions or directives. Due to errors on both macros and g.extensions, directives were chosen.
- [x] (!) Tagging while preserving the TOC. (Headers inside custom directives.)
- [x] (!) Tagging multiple pieces to data-\*. (Due to limitations went with a simple JSON object.)
- [x] (!) Fix transparent tab bar borders to be locked with the tab bar. Test with different zoom configurations.
- [x] Sticky Section header and style changes.
- [x] Auto load news on start.
- [x] Styling of text (headers, paragraphs, most of the basic stuff that is returned by unified).
- [x] Automatic button to return to TOC once below a certain point of it. "Sticky" to bottom right.
- [x] Smooth scrolling on TOC.
- [x] ToD Tech doc to GFM. Test. (Update GRM inject function to search for tech file and load.)
- [x] Card system to present News (how to differentiate between different headers of news? Make a folder only for news and a handler?) (make shadow effect when hovering cards)
- [x] Add sidebar to quotes. (markdown)
- [x] Styling update (divide into multiple files, the first file, loaded first, is for global stuff, after that things like nav bar...) + name re-definition.
- [x] Simple Footer
- [x] Code organization, comments and considerations (change to ts? NO).
- [x] Variable names checks and others (JSPrettier).
- [x] Add placeholder files, update package.json and add gitignore
- [ ] Test on GitHub pages.
- [ ] Handle footer pages. (redirect to a document on root folder when using footbar links)
- [ ] Search system on nav bar (checks heading from tech files and present Gamename-bold + headername-italics. Redirects to game and header somehow)
- [ ] Make so that NEWS section up to 3 files from the news folder and sorts them by date on the flex box.
- [ ] Translate ToV documents.
- [ ] Make media some techs.
- [ ] Research proper media format for videos. Convert recorded videos to format.
- [ ] Add icons to tagged elements to represent each information. Forced video means inside the div, non-forced on hover like the other icons. All icons are images that present something on hover (only forced video is special. Look at material design for icons?) **17?**
- [ ] https://developers.google.com/speed/pagespeed/insights/ Test and try to fix. Maybe offloading fonts?
- [ ] Properly tag and test every header. (includes recording new media)
- [ ] Javascript handling of checkboxes.
- [ ] Proper code formating with Highligh.js (how to use it everytime the page updates? require error when I use it in the unifyMethods)
- [ ] Change nav-bar depending on viewport size (so things don't clip into each other). Make so that a drop down list comes on the side? Or just the search? (<-- probably better)
- [ ] (!) XML request async.
- [ ] (!) Cards resize only on one axis (instead of keeping aspect-ratio) when resizing window (x or y).
- [ ] Remake news1 page.
- [ ] Test other OSs and browsers. **18? Take a break?**
- [ ] ... (period to gather feedback)
- [ ] README, License.
- [ ] Footnotes.
- [ ] How to Contribute (+ How to use Github for the project --> Issues can be both bug reports and tech descriptions. Need tags for both.)
- [ ] ... (period of release)
- [ ] Mobile port
- [ ] White theme
- [ ] Full Custom Tab bar (JS)
- [ ] Modifications needed and tutorial on how to fork and use for other game series.

## Autolink literals

Due to using GFM, TTE suports autolink literals that do no require special markdown syntax to work. See the examples below:

www.example.com, https://example.com, and contact@example.com. (P.S. Remember you can use [the default syntax too](http://example.com/)!)

The table of contents also has links created automatically by another part of the unified toolchain (slug).

## Strikethrough and Math

TTE suports other specific syntax (including all of the basic Markdown syntax) such as the above.

~one~ or ~~two~~ tildes.

Lift($L$) can be determined by Lift Coefficient ($C_L$) like the following
equation. :heart:

$$
L = \frac{1}{2} \rho v^2 S C_L
$$

## Tables

Tables are part of the GFM syntax and can be created as the example below:

| Beep |  No.   |   Boop |
| :--- | :----: | -----: |
| beep |  1024  |    xyz |
| boop | 338845 |    tuv |
| foo  | 10106  | qrstuv |
| bar  |   45   |   lmno |