🏠 [Home](README.md)

# Website Audit Checklist

It may be necessary to run through the list below multiple times
to ensure new problems are not introduced as problems are corrected.

|     | **Importance Rating** |
| --- | --------------------- |
| 🟥  | Critically Important  |
| 🟧  | Very Important        |
| 🟨  | Important             |
| 🟩  | Do If Possible        |

## 👶 Very Easy Tests

A website **MUST** at minimum pass the following tests.

### ⭐ Validate the HTML ⭐

Using valid HTML is the best way to ensure the website will function properly
on all web browsers.

[W3C Markup Validation Service](https://validator.w3.org/)

|     | Success Criteria                               |
| --- | ---------------------------------------------- |
| 🟧  | Ensure there are **zero validation errors**.   |
| 🟨  | Clear as many validation warnings as possible. |

### Ensure the Security Certificate is Valid

Invalid certificates result in very scary messages for end users.
Many browsers make it difficult for users to load websites with certificate errors.

|     | Success Criteria                          |
| --- | ----------------------------------------- |
| 🟥  | Ensure the security certificate is valid. |

### Load Properly in Multiple Web Browsers

Websites should not require a specific web browser, operating system, or resolution to work.

**Browsers**

|     | Success Criteria                                               |
| --- | -------------------------------------------------------------- |
| 🟥  | Ensure the website works in Google Chrome (or Microsoft Edge). |
| 🟧  | Ensure the website works in Mozilla Firefox.                   |

**Resolutions**

|     | Success Criteria                                                           |
| --- | -------------------------------------------------------------------------- |
| 🟥  | Ensure the website works well in a maximized window on a desktop computer. |
| 🟧  | Ensure the website works well in a narrow window, like a mobile screen.    |

### Pass Google's Lighthouse Test

Lighthouse is a website testing tool built into the Google Chrome web browser
that can identify website performance and accessibility issues.

Press <kbd>F12</kbd> in Google Chrome to open the Chrome Dev Tools.
Navigate to the Lighthouse tab.

**Mobile Scans**

|     | Success Criteria                                                                            |
| --- | ------------------------------------------------------------------------------------------- |
| 🟧  | Achieve a perfect score (100%) in Accessibility.                                            |
| 🟧  | Achieve a passing score (50% or better) in Performance.                                     |
| 🟧  | Achieve a passing score (50% or better) in Best Practices.                                  |
| 🟩  | Implement any recommendations that would improve the Performance and Best Practices scores. |

**Desktop Scans**

|     | Success Criteria                                                                            |
| --- | ------------------------------------------------------------------------------------------- |
| 🟧  | Achieve a perfect score (100%) in Accessibility.                                            |
| 🟧  | Achieve a passing score (50% or better) in Performance.                                     |
| 🟧  | Achieve a passing score (50% or better) in Best Practices.                                  |
| 🟩  | Implement any recommendations that would improve the Performance and Best Practices scores. |

### Cut the Junk!

**Files**

|     | Success Criteria                                                                            |
| --- | ------------------------------------------------------------------------------------------- |
| 🟩  | Avoid subpages for content that could easily be included on the parent page.                |
| 🟩  | Avoid PDFs and other non-webpage documents for content that could be included on a webpage. |

**Language**

|     | Success Criteria                                                                           |
| --- | ------------------------------------------------------------------------------------------ |
| 🟨  | Ensure that all content can be reasonably understood by a person with a Grade 9 education. |
| 🟩  | Ensure all abbreviations are defined.                                                      |

## 🖐 Easy Hands-On Testing

### Check for Browser Errors

When a browser encounters an error loading a website, it may not behave as expected.

Press <kbd>F12</kbd> to open the web browser's Dev Tools.
Press <kbd>F5</kbd> to refresh the web page.

|     | Success Criteria                                               |
| --- | -------------------------------------------------------------- |
| 🟧  | Check the Console tab.  Ensure there are no errors.            |
| 🟨  | Check the Network tab.  Ensure all files are loading properly. |

### Check the Page Structure

|     | Success Criteria                                                                              |
| --- | --------------------------------------------------------------------------------------------- |
| 🟧  | Ensure that headings are properly marked and properly ordered with `<h1>`, `<h2>`, etc. tags. |
| 🟨  | Ensure that lists are properly marked with `<ul>` or `<ol>` tags.                             |
| 🟨  | Ensure all form fields are properly labelled.                                                 |
| 🟨  | Ensure tables are only used for table data.                                                   |

## 💡 Advanced Hands-On Testing

The tests below require somewhat more expertise,
but are valuable in the website auditing process.

By correcting items identified in the easier sections,
the significance of evaluating many of the items in the advanced section will be lessened.
For example, valid HTML will be interpreted better by screen readers.
Also, the Lighthouse accessibility score is based on a subset of the success criteria
outlined in the Web Content Accessibility Guidelines (WCAG) 2.1.

### Browse the Entire Website with a Keyboard

Use the <kbd>Tab</kbd> key to move between focusable areas.
Use <kbd>Enter</kbd> or <kbd>Space</kbd> to activate focused areas.

|     | Success Criteria                                                                                     |
| --- | ---------------------------------------------------------------------------------------------------- |
| 🟧  | Ensure all interactive elements (i.e. links, form fields) can be accessed with the keyboard.         |
| 🟨  | Ensure there is visual feedback (i.e. colour change, highlighted border) when elements are in focus. |

### Browse the Entire Website with a Screen Reader

Some operating systems have built-in screen readers.
JAWS is a popular commercial screen reader.
[NVDA](https://www.nvaccess.org/) is a free screen reader for Windows.

|     | Success Criteria                                                   |
| --- | ------------------------------------------------------------------ |
| 🟧  | Ensure all of the content is read sensically by the screen reader. |

### Check the Website for WCAG 2.1 Compliance

The [Web Content Accessibility Guidelines (WCAG) 2.1](https://www.w3.org/TR/WCAG21/) document
describes success criteria for building accessible websites.

Although it's not the official document,
WebAIM offers a [WCAG 2 Checklist](https://webaim.org/standards/wcag/checklist)
that can assist with interpreting and implementing the document's recommendations.

|     | Success Criteria                                        |
| --- | ------------------------------------------------------- |
| 🟥  | Ensure compliance with all Level A recommendations.     |
| 🟧  | Ensure compliance with all Level AA recommendations.    |
| 🟨  | Wherever possible, implement Level AAA recommendations. |

## ➰ Do the Very Easy Stuff Again!

If significant website changes were made while auditing,
it would be worthwhile to validate the HTML again, and ensure the website still passes Lighthouse tests.
