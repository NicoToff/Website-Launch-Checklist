# Website Launch Checklist

<p align="center">
  <img src="Checklist_Image.png">
   </p>  
   
   <p align="center">
    A checklist of tasks to do before launching a public website.
  
  <br>
  <small> <b><i>Show your support!</i> </b></small>
  <br>
   <a href="https://github.com/MarketingPipeline/Website-Launch-Checklist">
    <img title="Star on GitHub" src="https://img.shields.io/github/stars/MarketingPipeline/Website-Launch-Checklist.svg?style=social&label=Star">
  </a>
  <a href="https://github.com/MarketingPipeline/Website-Launch-Checklist/fork">
    <img title="Fork on GitHub" src="https://img.shields.io/github/forks/MarketingPipeline/Website-Launch-Checklist.svg?style=social&label=Fork">
  </a>
   </p>  


<br>

## Table Of Contents
  * [Checklist](#checklist)
    + [Pre-Launch](#pre-launch)
    + [Post-Launch](#post-launch)
    + [Launch](#launch)
    + [Ongoing](#ongoing)
  * [Suggestions](#suggestions)
  * [Copyright and Attribution](#copyright-and-attribution)

<br>



## Checklist

Launch preparation generally takes a day or more. You should also reserve a day for bugfixing after you have wrapped the last feature. Be sure to plan accordingly!

### Pre-Launch
* [ ] <b> Content and Style </b> 
 
    * [ ] <b> Typography and layout	  </b>
 
      * [ ] Check for incorrect punctuation marks, particularly apostrophes, quotation marks and hyphens/dashes	 
 
      * [ ] Check headings for where you could potentially use ligatures	 
 
      * [ ] Check for widow/orphan terms in important paragraphs	 
 
 * [ ] <b> Spelling and grammar	 </b>
 
* [ ] <b> Consistency	 </b>
 
    * [ ]  Capitalisation (especially of main headings)	 
 
    * [ ]  Tense/Style of writing	 
 
    * [ ]  Recurring/common phrases (e.g. ‘More about X’ links)	 
  
   * [ ]   Variations in words (e.g. Websites vs Web Sites, or UK vs US spelling)	 
  
    * [ ]  Treatment of bulleted lists (e.g. periods or commas at end of each item)	 
 
 
 
 * [ ]  Check for hard-coded links to staging domain (i.e. ensure all links will change to ‘live’ URL/domain when site is launched)
 
 * [ ] Ensure no test content on site	 
 
 * [ ] Check how important pages (e.g. content items) print	 
 
 * [ ] For re-designs, ensure important old/existing URLs are redirected to relevant new URLs, if the URL scheme is changing
 
 * [ ] Check all ‘Hidden Copy’ (e.g. alt text, transcriptions, text in JavaScript functions)	 
 
 
 * [ ] <b> Standards and Validation </b>
    * [ ] Accessibility	 
   * [ ]  HTML validation	 
   * [ ]  JavaScript validation	 
   * [ ]  CSS validation	 
 
 
 * [ ] <b> Search Engine Visibility, SEO and Metrics </b>

     * [ ] Disable Indexing On Development Server 
   
     * [ ] Page Titles are important; ensure they make sense and have relevant keywords in them.	
  
    * [ ]  Create metadata descriptions for important pages.	 
  
    * [ ]  Check for canonical domain issues (e.g. variations in links to http://site.com http://www.site.com http://www.site.com/index.html should be reduced to a single   consistent style)	 
  
    * [ ]  Ensure content is marked-up semantically/correctly (h1, etc.)	 
  
     * [ ] Check for target keyword usage in general content	 
  
     * [ ] Check format (user/search engine friendliness) of URLs	 
  
    * [ ]  Set up Analytics, FeedBurner, and any other packages for measuring ongoing success	 
  
    * [ ]  Create an XML Sitemap	 
  
     * [ ] Configure Google Webmaster Console and Yahoo! Site Explorer	 

   
    * [ ] <b> Sharing & Rich Snippets</b>
        * [ ] Create a share card using [Photopea](https://photopea.com/) or a similar tool

        * [ ] Set up Facebook meta tags & validate [here](https://developers.facebook.com/tools/debug/)
        
        * [ ] Set up Twitter meta tags & validate [here](https://cards-dev.twitter.com/validator)
       
    <b> Facebook Tag </b>   
    ```html
    <meta property="og:type" content="website">
    <meta property="og:site_name" content="${SITE_NAME}">
    <meta property="og:description" content="${SITE_DESCRIPTION}">
    <meta property="og:image" content="${SHARE_CARD_URL}">
    <meta property="og:title" content="${PAGE_TITLE}">
    <meta property="og:url" content="${PAGE_URL}">
    ```
    
   <b> Twitter Tag</b>
    ```html
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:site" content="${SITE_NAME}">
    <meta name="twitter:creator" content="${SITE_AUTHOR}">
    <meta name="twitter:description" content="${SITE_DESCRIPTION}">
    <meta name="twitter:image" content="${SHARE_CARD_URL}">
    <meta name="twitter:title" content="${PAGE_TITLE}">
    <meta name="twitter:url" content="${PAGE_URL}">
    ```
 
 * [ ] <b> Functional Testing </b>
    * [ ] Check all bespoke/complex functionality	 
 
    * [ ] Check search functionality (including relevance of results)	 
    
    * [ ] Check on common variations of browser (Internet Explorer, Firefox, Safari, Chrome etc.), version (6, 7, 2.2, 3.1 etc.) and platform (Windows, OSX, Linux)	 
    
    * [ ] Check on common variations of Screen Resolution	 
    
    * [ ] Test all forms (e.g. contact us, blog comments), including anti-spam features, response emails/text, etc.
    	 
    * [ ] Test without JavaScript, Flash, and other plug-ins	
     
    * [ ] Check all external links are valid	 
    
    * [ ] Run the site through Google's [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/)

    * [ ] Write a script to load test your site
    - Check out [Locust](https://docs.locust.io/en/stable/) for this. See [LA Metro Councilmatic](https://github.com/datamade/la-metro-councilmatic#load-testing) for a basic example.
  
  * [ ] <b> Printer Friendliness </b> 
  
       Dynamic sizing, dark backgrounds, and interactivity don't play well with printers.

       
    * [ ] <b> Pick one option to solve this: </b>
        * [ ] Make a print stylesheet using a `@media print {}` media query, then add it to your site with `<link rel="stylesheet" type="text/css" href="css/print.css" media="print">`

       - <b> OR </b>

        * [ ] Use your browser's dev tools to remove offending elements (like sticky footers), alter colors where needed, and [screenshot the entire page]  (https://stackoverflow.com/a/14830242).
     
    * [ ] Add a link to the printer-friendly version to your website.
    
 * [ ] <b> Browser and mobile compatibility </b>
    * [ ] Use BrowserStack to confirm that your site is compatible with the browsers you wish to support
    
    * [ ] <b> Using BrowserStack's mobile device emulators and/or your own mobile device, confirm that: </b>
        * [ ] Scrolling is easy
    
        * [ ] Nav bar works
    
        * [ ] Hoverable things are tappable
    
        * [ ] Charts and maps look ok
 
 * [ ] <b> Security/Risk </b>
    * [ ]  Configure backup schedule, and test recovery from backup.	 
 
     * [ ] Protect any sensitive pages (e.g. administration area)	 
 
     * [ ] Use robots.txt where necessary	 
 
 * [ ] <b> Security/Penetration test	</b> 
 
    * [ ]  Turn-off verbose error reporting	 
 
     * [ ] Check disk space/capacity	 
 
     * [ ] Set-up email/SMS monitoring/alerts (e.g. for errors, server warnings); consider internal and external monitoring services	 
 
 
 
 
* [ ] <b> Performance </b>
   * [ ]  Load test	 
 
    * [ ] Check image optimisation	 
 
    * [ ] Check and implement caching where necessary	 
 
    * [ ] Check total page size/download time	 
 
    * [ ] Minify/compress static (JavaScript/HTML/CSS) files	 
 
   * [ ]  Optimise your CSS: use short image paths; make full-use ‘cascading’ nature of CSS, etc.	 
 
    * [ ] Check correct database indexing	 
 
    * [ ] Check configuration at every level (Web server, Database, any other software e.g. Content Management System)	
 
   * [ ]  Configure server-based logging/measurement tools (e.g. database/web server logging)	 
 
 
 * [ ] <b> Finishing Touches </b>
    * [ ] Create custom 404 & 500 & other error pages	

    * [ ] <b> Favicons </b>
        * [ ] Create a favicon
    
        * [ ] Add favicons and Apple touch icons (http://www.favicomatic.com/)
 

<br>

 ### Post-Launch
 * [ ] <b> Marketing </b>
    * [ ] Social Marketing: Twitter, LinkedIn, Digg, Facebook, Stumbleupon, etc.	 
 
    * [ ] Submit to search engines	
 
   * [ ]  Set-up PPC/Google Adwords where necessary	 
 
    * [ ] Check formatting of site results in SERPs	 
 
 <br>

 ### Launch
* [ ] <b> Deployment </b>
    * [ ] Create a production deployment

    * [ ] Double check that production-level resources have been provisioned

    * [ ] Purchase your domain and create the DNS record to point it at your production deployment

    * [ ] Ensure HTTPS / SSL is correctly set.
    
* [ ] <b> Web Search Indexing </b>
    * [ ] Allow indexing of your production site
    
    * [ ] Redirect the www subdomain to your root domain
    
    * [ ] [Set a canonical URL](https://developers.google.com/search/docs/advanced/crawling/consolidate-duplicate-urls) to prevent duplicate search results
 
* [ ] <b> Google Analytics </b>
    * [ ] Create a [Google Analytics](http://www.google.com/analytics/) account (if you do not have one)
    
    * [ ] Add [the Google Analytics script](https://developers.google.com/analytics/devguides/collection/analyticsjs) to your site
    
    * [ ] Set up [Google Webmaster Tools](https://www.google.com/webmasters/tools/home?hl=en) and [verify site](https://support.google.com/webmasters/answer/9008080?hl=en)
    * [ ] Link Webmaster Tools to Google Analytics
   
 
<br>

 ### Ongoing
 * [ ] Monitor and respond to feedback (direct feedback, on Social Media sites, check for chatter through Google, etc.)	 
 
 * [ ] Check analytics for problems, popular pages etc. and adjust as necessary	 
 
 * [ ] Update content
 
 * [ ] <b> Optional: </b> Set up relevant Goals and Funnels in Google Analytics
   
 
<br>

# Pre-launch Website Checklist

The following checklist should be actioned after all major development work has been completed.

## Browser Testing

Check the website:

1. Responds to different devices and screen sizes appropriately.
2. The design of the site is displayed as expected.
3. Nothing appears to be broken.
4. __All__ functionality works as expected for all browsers and devices, and to the best of the browser's compatibility at its time.

#### Desktop

- [ ] Chrome(mium)
- [ ] Safari
- [ ] Firefox
- [ ] Microsoft Edge 15
- [ ] Microsoft Edge 16
- [ ] Microsoft Edge 17
- [ ] Microsoft Edge 18
- [ ] Microsoft Edge Latest (Chromium version Windows/Mac)
- [ ] IE11 (if requested)

#### Mobile

For iOS, use Apple's device simulator with various devices (of different screen sizes).

- [ ] Android Chrome
- [ ] iOS Safari 9 (if requested)
- [ ] iOS Safari 10 (if requested)
- [ ] iOS Safari 11 (if requested)
- [ ] iOS Safari 12
- [ ] iOS Safari 13
- [ ] iOS Safari Latest

#### Responsiveness

- [ ] Large desktop (1551 - 1880)
- [ ] Medium desktop (1281 - 1550)
- [ ] Desktop (1025 - 1280)
- [ ] Tablet (801 - 1024)
- [ ] Large mobile (401 - 1024)
- [ ] Mobile (0 - 400)

## General Functionality

#### Links

 - [ ] Links on all pages direct the user correctly
 - [ ] Functional links (e.g. mailto) work correctly
 - [ ] Links styled as buttons are styled anchor tags
 
#### Forms

- [ ] Validation works correctly (if applicable)
- [ ] Submitted data is the format and type
- [ ] Submit to the correct endpoint
- [ ] Forms are consistently styled across the site (where applicable)
- [ ] All fields have labels (with the `for` attribute)
- [ ] Tooltips (if applicable)

#### Images
- [ ] All images are optimised, or sent through a CDN
- [ ] All images have an `alt` attribute
- [ ] All images are the correct size / dimension (test with varying browser widths / heights)

#### Navigation

- [ ] Elements that involve navigating from one place to another should _always_ be an anchor element
- [ ] Browser history behaves as desired e.g. when a user uses the browsers forward/backward buttons

## Coding

- [ ] CSS/JS minified
- [ ] Remove any `console.logs` used during development
- [ ] All code is commented where necessary
- [ ] Ensure all scripts are production versions
- [ ] Check all scripts link from a valid and reputable CDN, e.g. Google APIs, Cloudflare
- [ ] All third-party services and endpoint use the production API keys

## SEO

- [ ] Meta tags have been added (i.e. description, lang, etc)
- [ ] Sitemap created and linked to
- [ ] Page titles are correctly listed
- [ ] Breadcrumb displays accurate page navigation/path
- [ ] Schema tags added for breadcrumbs, products, articles, etc (i.e. ld+json snippets)
- [ ] Google analytics code has been added

## Shopify/Ecommerce

#### Settings

- [ ] Set the store email address to Client's address
- [ ] Updated the store address to that of the Client

#### General

- [ ] Main site search returns products only
- [ ] Search form uses GET and not POST method
- [ ] Article search returns only articles
- [ ] Link to terms and conditions exists
- [ ] Link to privacy policy and/or cookie policy exists
- [ ] Cookie consent popup (https://github.com/ketanmistry/ihavecookies)
- [ ] Menus do not include a link to `#` unless they are parent dropdown options
- [ ] Blank templates created and assigned where necessary

#### Collections

- [ ] Collections list template (`list-collections.liquid`) has been styled or redirected
- [ ] Collections template has had styles applied or redirected

#### Product Page

- [ ] Variant options work as expected
- [ ] Product adds to cart successfully
- [ ] Out of stock/unavailable variants are clearly marked with appropriate messaging

#### Cart

- [ ] Cart displays the correct prices quantities, subtotals and totals
- [ ] Line item quantities update
- [ ] Cart sends correct product details through to the checkout
- [ ] Checkout is styled up to match the brand colours
- [ ] Checkout labels (language file) have been adjusted if necessary
- [ ] Submitted a few test orders

#### Pages/Articles

- [ ] Page templates have styling applied
- [ ] Blog articles are linked via an index
- [ ] Article template has been styled
- [ ] Social media share options have been added to the blog article template
- [ ] 404 page template created and styled
- [ ] Contact form added to contact us page

#### Store Transfer

- [ ] Initiate and complete store transfer 
- [ ] Final invoice sent for the project

## Github Repository

- [ ] All unused templates/files/scripts have been removed to keep the project clean
- [ ] `Readme.md` has been well documented with CSS style guides, instructions, etc
- [ ] Wiki has been documented for projects with complex content management/data requirements (if necessary)
- [ ] All issues for **this release** have been closed (except for this one!)
- [ ] Release has been tagged and created

## Copyright and Attribution

##### Credits To ; 

Copyright (c) 2022 MarketingPipeline. Released under [Creative Commons Attribution-NonCommercial 4.0 International](https://github.com/MarketingPipeline/Website-Launch-Checklist/blob/main/LICENSE).

<small><i><a href='https://github.com/mapiec/checklist'>Original Author Of This Checklist</a></i></small>

