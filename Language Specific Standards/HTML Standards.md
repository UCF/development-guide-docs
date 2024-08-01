HTML (HyperText Markup Language) is the standard markup language for creating web pages. At times we can think of web pages as applications or sites, but at its core, an HTML page is a document. A website is a collection of HTML documents that have a defined structure and link to each other through the user of hyperlinks.

We may use a programming language to generate our HTML pages, either through a compiled process like a [Static Site Generator](https://en.wikipedia.org/wiki/Static_site_generator) or dynamically like through a [WordPress](https://wordpress.org/) site or [Django](https://www.djangoproject.com/) application. Fundamentally, however, we are still generating HTML documents and delivering them to the end user.

## Semantic Markup

Like a Word document or an XML document, HTML documents are made up of elements, and each kind of element carries with it a specific meaning. Just as Microsoft Word might infer a document outline based on the heading levels you use throughout your document, search engines use the semantic meanings of elements to infer a document's structure, purpose and content. When we refer to "semantic markup", we are referring to using [meaningful and purposeful elements](https://developer.mozilla.org/en-US/docs/Glossary/Semantics#semantics_in_html) in the markup of an HTML page.

The HTML elements you choose to use on a page mean something. The order in which content appears on the page means something. Both will be used to determine the way the document appears to web crawlers and accessibility software. It is important that the elements used on a page are well thought out and convey the same meaning as the content within them.

Resources and tips:
- The [MDN Element Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) is a great resource for finding the purpose of HTML elements.
- Valid, semantic HTML helps computers understand our content. This is critical not only for SEO purposes (defining contents with certain elements to define importance, etc.), but also for cross-browser compatibility (invalid markup can render differently depending on the browser, and can generally cause problems for the user) and web accessibility software (screen readers read off and provide navigation between some elements, depending on the element and/or other element attributes)
- When referencing parts of a page, keep in mind that semantic elements are not named arbitrarily--knowing what these are and using them consistently helps improve communication between designers and developers. (e.g., the "header" is a "header", not "top part").

## Accessibility

An extremely important consideration that should go along with semantic markup is ensuring markup follows accessibility standards. **UCF is committed to applying the [Web Content Accessibility Guidelines version 2.0 AA](https://www.w3.org/WAI/standards-guidelines/wcag/) standard.** All developers should familiarize themselves with the standard and take full advantage of tools with [Site Improve](https://www.siteimprove.com/) for testing accessibility standards on their websites.

Applying accessibility standards to a web page's markup should be a standard practice during the initial markup of the page, and not an afterthought to be corrected after deployment. Usually, applying accessibility standards in the first place will also ensure markup is semantically correct.

### Additional Tips:

- Users with color blindness can have trouble distinguishing between elements with low contrast. When coordinating colors for text, make sure the colors you pick pass the [WCAG color contrast level requirements](http://webaim.org/resources/contrastchecker/) We aim for text to *at least* pass "Level AA".)
- Please keep contrast in mind when using UCF's bright gold color against a white background `#ffc904` against a white background will fail both tests!!
- Avoid using extremely thin font weights unless they are used at very large, legible sizes—even then, consider using a thicker weight.

## Mobile-First Design

Whether using our [Athena Framework](https://ucf.github.io/Athena-Framework/) or a modified version of [Bootstrap](https://getbootstrap.com/), almost all modern CSS Frameworks take a [mobile-first approach](https://www.interaction-design.org/literature/topics/mobile-first#what_is_mobile_first?-0). As of the writing of this documentation, [most users now experience web content on a phone or tablet](https://research.com/software/mobile-vs-desktop-usage) far more often than they do a desktop device. A mobile-first CSS framework orients itself at the mobile breakpoint first, and then must be overwritten for larger layouts.

A mobile first approach also takes into consideration the unique needs of browsing on a mobile phone. Developers should take into consideration:

- Loading times: Reducing the size and number of large assets that need to load for the page to render.
- Data Limits: Reducing the size and number of large assets will reduce the data footprint of the page.
- Lazy loading: Deferring the loading of assets until they are needed will help in preventing the use of data when assets aren't actually needed.



