# SCIP Accessibility Audit v4

## Table of Contents

## [Promised Deliverables](inkdrop://note/TpFb7nmtQ)

## [Accessibility Audit Checklist](inkdrop://note/y54WgNQxT)

## [URI Metcalf SCIP Accessibility Audit Related Links](inkdrop://note/KS_8XHkQt)

----

## Introduction
Leading production of your site with an accessibility first mindset creates a more richly and empathically functional end user experience overall. A website's accessibility is not just a way to ensure that as many people as possible will be able to visit your site, no matter the physical or cognitive hurdle the user may be experiencing.

The idea that the overall accessibility of a website is the responsibility of the developer creating the website was something that hadn't initially occurred to me when first learning to code them. I was unaware of the needs of many users that are often overlooked. I was also unaware that this is an ongoing issues. This drove a curiosity in me to learn more. After I started considering more and more about accessibility in my projects, planning projects with accessibility at the forefront has become easier and easier, and also rewarding. With ever increasing accessibility, comes richer functionality and smoother experience in the website. Also knowing that fewer roadblocks are left in place with each new accessibiliy minded endeavour and each new skill learned, leaves a more satisfying and complete feeling to the process of creating these digital spaces.

My aim with this document is help shed some light on how to approach a project with an accessibility first mindset. And, at the very least, equip the reader with the tools to be able to approach any webpage, in particular the SCIP website, and be able to evaluate it efficiently and effectively. I understand that the reader is most likely not going to be a programmer or professional web developer, but it is my hope that they are able to be effective at creating considerate and inclusive websites, nonetheless, with the help of this guide.

To begin, a list of Steps is presented to outline general steps that can be taken to consider a webpage accessibility. They don't necessarily need to be in this order, this is just one approach.

Next, these steps are applied to evaluate the SCIP webpages that were present at the start of this project. Any accessibility opportunities that were found are listed and explanations are provided. Most of the time with some form of visual aid, sometimes video.

To wrap things up, the "Steps to Take in Future" walksthrough how to access these tools used along with examples of their use. This is meant to provide further blueprint for continued evaluation. Ensuring your site remains accessible as it grows, or standards change, is a continuous process.

Some extra links with additional information to help expand the reader's knowledge, and offer some additional assistance where relevant, are also provided

## Steps Taken

To evaluate how accessibile a website is, there are a few methods I can utilize.
1. The first set of tools I go to are the Developer Tools, available in every major desktop/laptop browser.
    1. I can use these tools to get a clearer picture of how a browser is showing my site by seeing the overall structure of the site, any styling that is being applied, and any programming associated with the site.
    2. I can also see any accessibility opportunities that the browser may have noticed.
    3. Descriptions on how to find these tools and how to use them are provided in "Steps to Take in Future" section of this document.
2. Next I will go to the Lighthouse feature in the Chrome DevTools to check the browsers accessibility assessment of the page. I will do this for each page, in Desktop and Mobile simulated views.

3. I usually start in Chrome and then go to Firefox to utilize the Firefox Inspector's Accessibility checker to get another view from a different browser. The interface for the accessibility checker is also very helpful in Firefox. The Accessibility Properties of the Firefox Inspector tool shows the structure of the webpage through its semantic roles and how they relate. It also can check the font contrasts, keyboard navigability, and text label clarity of a webpage. It also can simulate various forms of color blindness and how users with those types of vision may see the content of the page. There are multiple built in tools in the browser to get an initial understanding of how accessible your pages are to other users.

4. I will also use the [WebAIM Color Contrast Checker](https://webaim.org/resources/contrastchecker/) to help find more accessible matches for background and foreground when the need arises. However, on the fly, the browser devtools color picker tool will usually provide a helpful WCAG score for the background / foreground color combination. As I describe later, this tool is also integrated into the WAVE Web Accessibility Evaluation Tool suite.

5. The [WAVE WebAIM Accessibility Evaluation Tool](https://wave.webaim.org/) provides a further detailed picture of your page's underlying structure and the impacts on accessibility. WAVE provides increased clarity to each of the highlighted potential points of improvement to the webpage it is analyzing. It is great for seeing all of the accessibility opportunities visually represented on the webpage with some steps on how to incorporate the suggestions. Additional details over this and other tools' features, as well as how to use them, are also available in the "Steps to Take in Future" section of this document.

7. Now that the general accessibility of the page is determined from manual and automatic testing, and visual analysis of the page, it is time to see how many of these features all come together to impact the "sound" of a webpage. The screen reader used by a visually impaired user, and how it reads the site, will completely determine their overall experience of the page. There are many different screen readers, including JAWS and NVDA for Windows, the built-in VoiceOver for Apple and iOS, ChromeVox on Chromebooks and TalkBack for Android devices. They all accomplish the same basic functions and will interpret the structure of your webpage in similar ways. The most popular Windows screen reader is JAWS, but perhaps the most accessible (and free) screen reader for Windows is NVDA **[ADD LINK]**. Non Visual Desktop Access (NVDA) is the screen reader I used for the Screen Reader portion of this assessment.

- There are many ways to assess a user's experience and these tools are just another way to improve the overall function and utility of a webpage. When it is found that there may be things that are hindering or lessening a user's experience, these acquired data are opportunities to build a more complete and inclusive digital space.

## Opportunities Discovered
- [x] **Intro**
  - [ ] **[Touch up Intro if Desired]**
- This section is broken up into various subsections and content within those subsections
  - Within these subsections are information and discussions pertaining to the specific accessibility opportunities that were discovered
  - This includes Chrome and Firefox browsers' built-in accessibility assessments
    - Much of the changes suggested relate to some of the background and foreground color contrasts falling below standards and may cause visual issues for some users.
    - Some heading issues are also highlighted.
  -  Additionally there are some other noted observations, as well as interpreted screen reader results.


### Found in Google Chrome Lighthouse
- Google Chrome Lighthouse is usually my first glance to quickly get a sense of what's going on in my webpage because I don't have to go to another site, let alone another browser, since I'm viewing my webpages on google chrome. It can test for many different aspects of how a website was put together and its presentation to the user. It shares some parallels with other browsers' internal testing features.
  - Below is an example of all that Lighthouse can scan for, not just Accessibility, using the mobile version of the Home Page for reference.
  ![clipboard.png](media/Tll3lEE24-clipboard.png)
  - We will just be focusing on the Accessibility portion, but the other information is interesting to learn about and may be worth a look, however it is easy to get lost down a rabbit hole with much of the information.
  - The performance score is most likely due to the internal functions and practices of WordPress and mostly out of your control, however making sure that the mobile versions of your pages have images that are reduced in size accordingly will also increase the performance on mobile.

#### Home Page Color Contrast
- The color contrast ratio between the text color and background color of most of the links is too low.
  - [x] **Give brief description of what would be shown in gif in case not navigated to linked gif**
    - [ ] Circle Back and see if desire to add anything else
- The following is a gif showing examples of the color contrast issues for the link text found in Chrome Lighthouse.
  - This specific page is the home page, but the light yellow text with white background links, and the inverse, are on every page.
  - [Click to view the gif](https://classy-dragon-6e3245.netlify.app/ECjDiXD03-Home_Accessibility_Color_Contrast.gif)
  - ![Home_Accessibility_Color_Contrast.gif](media/ECjDiXD03-Home_Accessibility_Color_Contrast.gif)
- Below is a gif of the Lighthouse result for the mobile version of the Home page with similar notes on link color contrast.
  - [ ] **Give brief description of what would be shown in gif in case not navigated to linked gif**
    - [ ] Circle Back and see if desire to add anything else
  - The following gif shows same color contrasts noted, just in the mobile version
  - [Click to view the gif](https://classy-dragon-6e3245.netlify.app/hgbGShFAK-Home_Accessibility_Color_Contrast_Mobile.gif)
  - ![Home_Accessibility_Color_Contrast_Mobile.gif](media/hgbGShFAK-Home_Accessibility_Color_Contrast_Mobile.gif)


#### About Page Color Contrast and Heading Elements
- For the About Page, it is also Color Contrast that is highlighted by Lighthouse.
  - [x] **Give brief description of what would be shown in gif in case not navigated to linked gif**
    - [ ] Circle Back and see if desire to add anything else
  - [Click to view the gif relating to contrast](https://classy-dragon-6e3245.netlify.app/GVfHXo_sh-About_Accessibility_Chrome.gif)
  - ![About_Accessibility_Chrome.gif](media/GVfHXo_sh-About_Accessibility_Chrome.gif)
- The sequence of headings on the page is noted at the end of the above gif.
  - The second gif, see below, shows the information in the dropdown.
  - [x] **Give brief description of what would be shown in gif in case not navigated to linked gif**
    - [ ] Circle Back and see if desire to add anything else
  - The jump to h6 headings out of sequence in the About page is shown in the gif below. Using headings in relevant sequential order improves the clarity of the page structure.
  - I also discuss the headings in further detail in the screen reader section.
    - [Click to view the second gif, relating to headings](https://classy-dragon-6e3245.netlify.app/B0MQfzz5I-About_Accessibility_Header_Order_Desktop_Chrome.gif)
    - ![About_Accessibility_Header_Order_Desktop_Chrome.gif](media/B0MQfzz5I-About_Accessibility_Header_Order_Desktop_Chrome.gif)

#### Research Page
- The Research Page in Mobile view has results similar to the desktop view, so I am only showing the mobile version results for sake of brevity.
- The color contrast is only mentioned for the menu button because it is hiding the other nav links that are shown when the button is touched
  - [x] **Give brief description of what would be shown in gif in case not navigated to linked gif**
    - [ ] Circle Back and see if desire to add anything else
  - The below gif shows just the contrast mentioned
  - A Navigation comment from Chrome, seen in this first gif, is expanded on in the second gif
- [Click to see the first gif](4fsRExnA8-Research_Access_Contrast_Chrome_Mobile)

    - ![Research_Access_Contrast_Chrome_Mobile.gif](media/4fsRExnA8-Research_Access_Contrast_Chrome_Mobile.gif)

- [Click to see the second gif, showing the heading suggestion](https://classy-dragon-6e3245.netlify.app/uhBupEq5k-Research_Access_Navigation_Chrome_Mobile.gif)

    - ![Research_Access_Navigation_Chrome_Mobile.gif](media/uhBupEq5k-Research_Access_Navigation_Chrome_Mobile.gif)
  - [x] **Give brief description of what would be shown in gif in case not navigated to linked gif**
    - [ ] Circle Back and see if desire to add anything else
  - h4 element jumps from h1 element "Research"
    - headings should be sequential and define the relative structure of the information of the page
    - You can always just decrease the font size of the relevant heading element to match the desire font size
  - There is also the matter of whether this should even be a heading
  - I talk about this specific situation in the screen reader section as part of the research page discussion

#### Fellowship Page
  - [x] **Give brief description of what would be shown in gif in case not navigated to linked gif**
    - [ ] Circle Back and see if desire to add anything else
  - The Fellowship page had generally the same issue with color contrast of links.
    - The below gif shows the nav bar and 'apply now' button contrast warnings
    - [Click to see a gif of the fellowship page lighthouse results](https://classy-dragon-6e3245.netlify.app/Fellowship_Access_Contrast_Chrome_Desktop.gif)
  - ![Fellowship_Access_Contrast_Chrome_Desktop.gif](media/seL9iyas4-Fellowship_Access_Contrast_Chrome_Desktop.gif)

### Found in Firefox Inspector
- Firefox Inspector Accessibility Properties accomplishes many of the same functions as Chrome's built-in tester, just presenting them in a different way and with some different insight. The two can complement each other well. In the scans, the tester brought attention to many of the same things as Chrome. For this reason I only list a few with some clarified details.

#### Link Text Color
- The colors of the texts associated with links, or anchors, have the following score.

![Link_Text_Color_Contrast.PNG](media/5aMSHvSPi-Link_Text_Color_Contrast.PNG)

#### Search Bar Color Contrast
- The following screenshot is from the score given for the color contrast of the search bar at the top right of each page. As with the above link text color, this low score also indicates the content may be hard to see for some users.

![clipboard.png](media/c9UN6DAsu-clipboard.png)

- As mentioned earlier, the inspector will show the semantic structure of the webpage. More on semantic structuring is mentioned in the Screen Readers subsection.
- [ ] **[Circle Back to the Below]**
- The "Tabbing Order" is also displayable **[Provide Example]**
  - Good for the most part.
- Text labeling issues appear to be on WordPress side and not something you need to worry about **[Double Check That]**
- ~~make a loom video showing the tabbing order and the the double markers on the posts on home page.~~ **[Post-MVP]**
  - also turn on the screen reader to see what is sounding there.
  - make a loom to discuss the text label issue with the wordpress buttons

### Navigation
  - Addition of Footer navigation will greatly increase ease of site navigation
  - Addition of "Home" link in Menu / Navigation will also improved ease of traversal
    - Not obvious that the header at the top is a link back to the home page
      - Could confuse some users
      - Best to have a "Home" link as well
        - Even if the "Home" page is meant as a landing page and may have information that repeats, it still may be helpful to have a "Home" just for clarity's sake

#### Keyboard Traversal
  - When moving through the site by keyboard all the elements that are interacted with by mouse should also be navigable by keyboard. Using the tab key will progress you through the clickable elements. Best to have a visual aid, or box, to tell where the "focus" is. Some of the links have a very subtle focus or none at all
    - make a loom showing the situation and possible fix **[Post-MVP]**
    - The rounded a tags, links/ [only some focus]
    - The dark square links [no focus at all]
      - Submit Application
      - Contact Us

### "Home" or "Landing Page"
  - Missing a First Level Heading "H1"
  - Title of Website at top of page acting as link is also missing
  - [ ] **[Fix or Remove]**

### Screen Readers
   - [ ] **[Perhaps change something between this intro and the information in the "Steps Taken" section]**
     - [x] **[Or just add to this intro a little]**
   - There are a few different screen readers out there that can help users navigate sites by having the content read aloud to them, as well as providing useful keyboard shortcuts, navigation tools, mouse interaction, and also braille feedback for braille devices.
   - The screen reader used for this project is **NVDA**
     - Free Open Source Screen Reader on Windows
       - A great way to understand how screen readers will interact with the site


#### Screen Reader Introduction Video
- I created a quick intro video to describe how the screen reader is used and what to look for and consider.
  - [SCIP - Screen Reader Intro](https://www.loom.com/share/e25e779e70c64b86a4472d432595e615)
  <div style="position: relative; padding-bottom: 72.12885154061624%; height: 0;"><iframe src="https://www.loom.com/embed/e25e779e70c64b86a4472d432595e615" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>

#### Home / Landing Page
- Click the link below for the Full Read of the Home Page as described in the intro video. **Caution**, the Screen Reader starts at **0:13** and will be **much louder** than my voice at the beginning.
  - [Home Page Full Screen Reading (NVDA) [**LOUD after 0:13**]](https://www.loom.com/share/0f793793c6f74cb496855693a1aeaf17)
    <div style="position: relative; padding-bottom: 64.6888567293777%; height: 0;"><iframe src="https://www.loom.com/embed/0f793793c6f74cb496855693a1aeaf17" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>
  - The video shows the Screen Reader reading through the Home Page to give an idea of how a screen reader will walk through a page and how it describes the elements. A user may also skip around the page using hotkeys specific to the screen reader but this first video is meant to paint the full picture of the page.
  - I had previously made a video talking about the benefits of adding a “Home” button to the navigation bar, but noticed that it has already been added since I started.
      - Adding a "Home" link in the navigation bar was definitely a good choice to benefit all users
      -
#### About Page
   - Click the link below to see the explanation of the headings and the screen reader’s interaction with them.
     - [SCIP – About Page - Headings Discussion [**LOUD after 0:07**]](https://www.loom.com/share/e6c7574c900f4c69940a26912b7f655a)
     <div style="position: relative; padding-bottom: 63.817663817663814%; height: 0;"><iframe src="https://www.loom.com/embed/e6c7574c900f4c69940a26912b7f655a" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>
   - In the video, the "Team" section is highlighted
     - I suggest that a new heading level under team member names is unnecessary
       - If keeping additional heading level, it should change to h4, instead of keeping as h6, and modify the font size to get the desired h6 font size
         - The heading level jumps from h3 to h6 and may be confusing to screen reader users.
           - Screen readers read aloud the type of element and this reads as "h3 [name of team member]" and then "h6 [title of team member]". This may be confusing

#### Research
- The discussion about the Screen Readers interpretation of the Research Page can be found in the link below
  - [SCIP - Research Page - Headings and Information Sectioning](https://www.loom.com/share/cdaebdc934e5449dbff6b4288580566a)
  <div style="position: relative; padding-bottom: 61.016949152542374%; height: 0;"><iframe src="https://www.loom.com/embed/cdaebdc934e5449dbff6b4288580566a" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>
  - [x] **Add Brief Description for above video**
    - [ ] **[Circle Back to see if want add anything]**
  - The video highlights:
    - Recommendation of additional headings that could help improve the overall flow and navigability of the Research webpage
    - Changing the h4 blocks at the end of the page to different element types
      - The block information shouldn't be a heading element
      - Recommend a short heading to describe the information instead
      - Recommend change the h4 blocks to paragraph elements
        - Can keep the size and colors if desired but shouldn't be headings
          - Headings should be concise and signal related information to follow
            - It helps screen reader users
              - Also improves flow of webpage

#### Fellowship
- Click the link below to see the discussion about the Fellowship Page screen reading experience
  - [SCIP - Fellowship Page - Heading Structure](https://www.loom.com/share/dc002c9fdd9f4982b798796534d4fb69)
  <div style="position: relative; padding-bottom: 68.06136680613668%; height: 0;"><iframe src="https://www.loom.com/embed/dc002c9fdd9f4982b798796534d4fb69" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>
  - [x] **Add Brief Description for above video**
    - [ ] **[Circle Back to see if want add anything]**
  - The video highlights:
    - Opportunity for h3 subheadings on the Fellowship page
      - Clarification of subsections of information within the "Fellowship Goals & Commitments" section of the Fellowship Page
        - Specifically, making the one word bolded titles, i.e. "Training", "Evaluation", and "Podcasts" into h3 headings
          - This can improve the experience of screen reader users
          - Can keep bolding and slightly increase size
            - Will help group the information better and improve page flow for all users

#### Footer Navigation
- Click the link below for a discussion about the addition of a Footer Navigation
  - [SCIP - Footer Discussion](https://www.loom.com/share/68ea61809a1345738bc987f0ee1d7595)
  <div style="position: relative; padding-bottom: 69.90291262135922%; height: 0;"><iframe src="https://www.loom.com/embed/68ea61809a1345738bc987f0ee1d7595" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>
  - [x] **Add Brief Description for above video**
    - [ ] **[Circle Back to see if want add anything]**
  - In the above video, I suggest the opportunity for a footer navigation
    - The case is made for the addition of internal links within the footer at the bottom of each page
      - These internal links would act the same as the links in the header navigation at the top of each page
        - Reader would be able to easily move to anywhere else in the site at the end of each page.
          - Helpful for Screen Reader users and also ones that aren't
          - Would keep the reader engaged and reminded of the structure of the site
    - Additional external links could also be added
      - Some examples:
        - Ways for readers to reach out or help
        - Fellowship Application Link
          - In case the user decides to apply when not on the fellowship page
        - Social Media if relevant
        - Podcast Link when available
        - Other related projects
        - Other URI links if desired
        - Additional Relevant Information
        - Copyright info if relevant [**See what Evelyn thinks about this one**]
        - Accessibility Statement or link to an Accessibility Statement
    - The addition of some form of site navigation in the footer of each page would greatly increase ease of use of the site
      - Users of all types, including screen reader users would benefit



### Accessibility Statement
  - Accessibility Statements are something that is becoming more common in sites with high user traffic and interaction.
  - These statements put forth a recognition and consideration of the diverse needs of users
    - Accessibility statements act as a sort of pledge to build and maintain sites that are sensitivity to the needs of their users
      - There is usually a way for the user to get in touch with the website's managers to inform them of any issues that they may notice or any information they are struggling to access due to some form of accessibility roadblock
    - They can also sometimes acknowledge areas in a site that need improvement and are currently being worked on
  - An accessibility statement could be added at the bottom of the page in the footer, or in a link to another page, at the bottom of each page with contact information to get in contact if there are any issues or features missing that are impacting the accessibility of users.
    - "Something like: We strive to make our website as accessible as possible to as many users as possible. If you are having any issues accessing our site or notice opportunities to make our site more accessible, in accordance with WCAG 2.0, please reach out at 'help@oursitedomain'."
    - There are many resources available online to give you a good idea as to how best to structure your own Accessibility Statement
    - [ ] **Circle Back to Look Deeper into Examples and links**
      - [ ] Might only need to flesh out example a little and/or add links

### Opportunities Discovered Conclusion
 - What we saw:
   - Results from the Chrome Lighthouse tool
     - Color Contrast for links should be addressed
     - Heading inconsistencies should be addressed
   - Firefox Accessibility Properties Inspector
     - Same recommendations as Chrome Lighthouse Screen Reader
     - It also didn't like the color contrast of the search bar above the navigation
   - NVDA Screen Reader illuminated how the site would be heard
     - Some headings opportunities
       - Some headings need to be changed
       - Some should be changed to different elements
       - Some headings should be added
     - Addition of footer navigation to internal webpages, and external sites if relevant, to footer element at bottom of each page
       - Would maintain clarity of website structure effectively
       - Would offer easier navigation through the site
       - Helps screen reader users more efficiently travel between pages of the site
     - Staying aware of how a screen reader interacts with a webpage is an important and ongoing process as a webpage develops and changes. Information and links are provided in the "Steps to Take in Future" section under "Screen Readers''.
   - Opportunity to add an Accessibility Statement to reflect commitment to inclusivity and acknowledge the diverse needs of the community
 - Overall, the website is showing clearly great care has already gone into constructing this website.
 - [ ] **Circle Back to Clean Up**

## Steps to Take in Future
- Briefly describe what can be done to stay aware of Accessibility on your Webpage
  - How to stay on top of Accessibility needs during development
  - Include key links to resources
- Include the media showing how to access various tools in this section
- [ ] **Turn above into Intro and/or remove**

### How To
#### Chrome DevTools
- [x] **Give brief description of what would be shown in gif in case not navigated to linked gif**
  - [ ] Circle Back and see if desire to add anything else
- [ ] [**WILL NEED TO FIX LINK. GH LINK BROKEN**]
- Below is a gif that will show how to access the Chrome DevTools in the [Google Chrome browser](https://www.google.com/chrome/downloads/)
- [GH Link](https://raw.githubusercontent.com/christopher-ward/SCIP_Audit/main/Gifs/Tools_Tips/Inspect_DevTools/how_to_access_devtools_and_inspect_specific_elements_comp.gif?token=GHSAT0AAAAAABV6ZO2P2BCWGYAJE3NZR6G2YXEJCDQ)
![how_to_access_devtools_and_inspect_specific_elements_comp_40.gif](media/yfn48lNNN-how_to_access_devtools_and_inspect_specific_elements_comp_40.gif)
- The Chrome DevTools can be accessed by right clicking anywhere on the page and selecting "Inspect"
  - Can also be accessed by pressing Command + Option + C on Mac keyboard or Control + Shift + C on Windows, Linux
  - Other methods and more information can be found [here on Google's Open Chrome DevTools page](https://developer.chrome.com/docs/devtools/open/)
- You can change where the DevTools shows in your browser window by changes the "Dock Side" by clicking on the three vertical dots a the top right of the DevTools menu
- The "Elements" pane of the DevTools shows the underlying HTML structure of the webpage that is being interpreted by the browser
  - This is a very important and helpful tool to understand how all the elements are interacting with one another and what properties are attached to them
  - It allows for fine-tuned customization of a webpage and will also help to target specific elements on the page if custom Cascading Style Sheets (CSS) code is desired on a WordPress generated site.
  - This also lets you verify what elements are being presented to assistive technologies and to check that proper [semantic elements](https://developer.mozilla.org/en-US/docs/Glossary/Semantics#semantics_in_html) are being utilized
- The "Styles" pane at the bottom of the DevTools, or right side depending on how the DevTools are docked to your page, shows what styling is being applied to a selected element.
  - These styles are written in a language known as CSS.
    - The styles can be found in a style element in the main HTML document of a webpage like so:
    ```HTML
     <style>
       h2 {
         property-to-modify: value;
       }
     </style>
     ```
    - They can also be in a separate attached stylesheet that ends with .css
    - Or you can see inline styles attached directly to the HTML element, like so:
    ```HTML
      <h2 style="property: value;">Inline Styled H2 Heading Element</h2>
    ```
  - Any property that is associated with a selected element while in the DevTool menu will be displayed in "Styles"

#### Chrome DevTools Lighthouse
- [x] **Give brief description, or images, of what would be shown in gif in case not navigated to linked gif**
  - [ ] Circle Back and see if desire to add anything else
- [ ] [**WILL NEED TO FIX LINK. GH LINK BROKEN**]
- Below is a gif on how to access Lighthouse in the Chrome DevTools in Google Chrome
- [GH Link](https://raw.githubusercontent.com/christopher-ward/SCIP_Audit/main/Gifs/Exhibition/Lighthouse/how_to_access_lighthouse_scan_resized.gif?token=GHSAT0AAAAAABV6ZO2OPNJU2HQC4BKX4XYKYXEMU7Q)
  ![how_to_access_lighthouse_scan_comp_25.gif](media/yJesrsUMy-how_to_access_lighthouse_scan_comp_25.gif)
- Access Lighthouse auditor by opening Chrome DevTools and clicking the "Lighthouse" tab at the top of the open DevTools Dock
  - It may be hidden on your view of the DevTools and can be accessed by first clicking the double arrows ">>" next the available options e.g. "Elements", "Console", etc.
    - You should then see an option for "Lighthouse" from a dropdown menu
  - There are various things that Lighthouse can check for on a webpage, but you can disable those others and just focus on Accessibility if you'd like.
    - I kept some other options enabled here for illustrative purposes and can be informative to explore them as well
  - For additional information on Lighthouse, you can access it [here on Google's Lighthouse Overview page](https://developer.chrome.com/docs/lighthouse/overview/).

#### Chrome DevTools Mobile Responsiveness Simulation AKA "Device Mode"
- [x] **Give brief description, or images, of what would be shown in gif in case not navigated to linked gif**
  - [ ] Circle Back and see if desire to add anything else
- [ ] [**WILL NEED TO ADD LINK**]
- Below if a gif of how to access the Chrome DevTools Device Mode tool on Google Chrome
![Chrome_Mobile_Responsiveness_compressed.gif](media/9TxytjC_K-Chrome_Mobile_Responsiveness_compressed.gif)
- Device Mode can be accessed from the Chrome DevTools menu by clicking the device toggle button at the top left of the menu that looks like two overlapping rectangles
  - After activating, I put the DevTools in separate window mode, and on a second screen, to more easily focus on the mobile view of the site.
    - I also recommend this if possible while exploring this feature yourself
  - There are multiple preset device dimensions that can be selected at the top of the Device Mode window
    - Additional options are available by clicking on the "Edit" button at the bottom of the dropdown menu
    - You can also watch how the page looks as the screen size changes by clicking the "Responsive" button at the top of the dropdown menu
      - Then you can change the vertical and horizontal dimensions by dragging the sides of the simulated
      - This is helpful for learning at exactly which dimensions the page "breaks" or stops looking how you want it to look and can be planned for accordingly
        - This can allow for more precise control of the look of your site as the screen dimension and orientation changes through the use of custom CSS Media Queries.
      - This feature isn't as useful currently but if further customization, or development of a new site is desired, then this feature could be helpful
- More information about "Device Mode" and its features can be accessed [here on Google's "Simulate mobile devices with Device Mode" page](https://developer.chrome.com/docs/devtools/device-mode/#viewport)
- Luckily WordPress themes come with mobile responsive versions already programmed in and can be modified to an extent
  - Additional customizations for multiple desired mobile sizes and orientations may require custom CSS integration
  - The current version of the site is still viewable on most devices as shown in the above gif
- There is a very similar option in Firefox and easy to access once you know how to access it in Google Chrome

#### Firefox Developer Tools and Accessibility
  - [x] **Give brief description of what would be shown in gif in case not navigated to linked gif**
    - [ ] Circle Back and see if desire to add anything else
- [ ] [**WILL NEED TO FIX LINK. GH LINK BROKEN**]
- Below is a gif of how to access the Firefox Developer Tools and Accessibility menu on the [Mozilla Firefox Browser](https://www.mozilla.org/en-US/firefox/)
- [GH Link](https://raw.githubusercontent.com/christopher-ward/SCIP_Audit/main/Gifs/Exhibition/Firefox_DevTools/Firefox_DevTools_resized_compressed.gif?token=GHSAT0AAAAAABV6ZO2PMFUDBC3JDYJ27CZYYXEODJA)
  ![Firefox_DevTools_comp_40d.gif](media/Mo8OzPleN-Firefox_DevTools_comp_40d.gif)
- Firefox Developer Tools, Accessibility Panel
  - To open you can right click and select "Inspect", just like in Chrome.
    - You can also use a slightly different key shortcut:
      - Command + Option + I on macOS, or Control + Shift + I or F12 on Windows, Linux
        - Think of C for Chrome and I for Inspector... or just right click or select from the Tools menu
  - It's very easy to get to the Accessibility Panel in Firefox and will be very apparent upon opening the FF DevTools, as seen in the gif
    - You can also go directly to the Accessibility Panel after right clicking on the browser window
  - The Accessibility Properties can scan for Contrast, Keyboard, Text Labels issues
    - Also simulate various types of color blindness
    - Can also activate visual reference of page keyboard tabbing order
    - Can also see mobile version of site just like in Chrome DevTools just slightly different User Interface
      - Access by hitting the button at top right that looks similar to Chrome (two Mobile Devices, or rectangles, overlapping)
- More information about Firefox Developer Tools available [here in the Firefox DevTools User Docs](https://firefox-source-docs.mozilla.org/devtools-user/#:~:text=You%20can%20open%20the%20Firefox,%2B%20Opt%20%2B%20I%20on%20macOS.)

#### WebAIM Web Accessibility Evaluation Tool
- [WAVE](https://wave.webaim.org/) is a very effective interactive tool for checking the overall accessibility of a webpage.
- This tool is a great approach to understand accessibility opportunities in a webpage and to better understand their significance.
- Has many of the same features as the browser tools, but in a better visual package and easier interaction.
- The information is organized and presented in a very convenient and clear manner.
- Click on the link below to see a short demo of how to use the tool and what is shown.
- [WebAIM Web Accessibility Evaluation Tool Demo](https://www.loom.com/share/7e130b24e0554bf190fc92c187f4d79a)
  <div style="position: relative; padding-bottom: 73.77049180327869%; height: 0;"><iframe src="https://www.loom.com/embed/7e130b24e0554bf190fc92c187f4d79a" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>
- There is also a browser extension that can be installed to evaluate your webpage locally on your computer.
  - No need to have webpage deployed online
  - More information and possible benefits can be found [at this page](https://wave.webaim.org/extension/)

#### WebAIM Contrast Checker
- Contrast Checker is a great tool to quickly troubleshoot color combinations that will work best for you needs while still meeting WCAG contrast ratio recommendations. **[Add Link to Contrast Checker somewhere]**
- You can see a color contrast rating in developer tools, but not as easy to use or as fleshed out.
- The WebAIM Contrast Checker tool is also built into the WAVE tool described above and can explore various color combinations directly on your webpage through the WAVE interface.
[Link to Gif of Tool for PDF readers](https://classy-dragon-6e3245.netlify.app/WebAIM_Contrast_Checker.gif)
![WebAIM_Contrast_Checker.gif](media/gaPFksDYP-WebAIM_Contrast_Checker.gif)

#### Screen Readers
- [x] **Add some info and links for screen reader**
- NonVisual Desktop Access (NVDA) created by [NV Access](https://www.nvaccess.org/) was the screen reader used in this report
  - It is showcased in the previous "Opportunities Discovered" section under the "Screen Readers" subsection, as well as mentioned in the "Steps Taken" section
    - For this reason, I won't go as in depth into the descriptions of the screen reader in this subsection
  - The free, open source screen reader for Windows operating system can be [downloaded at this NVDA page](https://www.nvaccess.org/download/).
  - To understand and effectively use the reader, a very helpful and essential [user guide can be found on this linked page](https://www.nvaccess.org/files/nvda/documentation/userGuide.html)
- I also reference Apple's built-in assistive technology, VoiceOver, in the "Some Additional Links" section under the "Additional Screen Reader Links" subsection
  - Hopefully these links are helpful if you would like to explore this technology in an Apple product.
- Something like the WebAIM Web Accessibility Evaluation Tool (WAVE), referenced previously, will do an effective job of alerting you to obvious screen reader speed bumps
  - However, a more effective way to better understand how a screen reader user would navigate a page, or to determine what conveniences could be implemented to increase ease-of-use, is to experience your site using a screen reader.
    - Even better would be to collaborate with an actual screen reader user to help test your site for screen reader use
      - At the end of the day, they would have the highest expertise in screen reader usage and expected conveniences

## Some Additional Links
- I've put together a few additional links that may be helpful moving forward

### Additional Screen Reader Links
- There is built in assistive technology on all Macs called VoiceOver
  - [WebAIM Docs on Apple VoiceOver Screen Reader](https://webaim.org/articles/voiceover/)
  - [Apple Intro to VoiceOver Screen Reader](https://www.apple.com/voiceover/info/guide/_1121.html)
  - [A potentially helpful Medium Article on Apple VoiceOver Screen Reader](https://lsnrae.medium.com/how-to-use-the-voiceover-screen-reader-70699e2e0f8a)
- [ ] **[ADD LINKS]**

## In Conclusion
Now that you've made it all the way through this document, or jumped around in whatever order suited your needs best, my sincere hope is that you find yourself more informed on the many facets of a websites overall accessibility. And, additionally, that you find yourself more capable to continuously act as the first line of defense in maintaining an inclusive and considerate user experience for your website.

The SCIP website is overall accessible to users of all types, mostly due in part to in relatively minimal complexity (programmatically speaking - the more programming involved, the greater the possibility for reduced accessibility), and also due to the accessibility of the WordPress theme and tools this site is based on.

However, there are some obvious opportunities for improved accessibility that, while relatively small in number, can greatly improve the experience and ease-of-use of the SCIP website for all users.

I hope that this document is able to explain these potential points of improvement well, and also illuminate the tools needed to test effectively. Ultimately I hope that whoever ends up utilizing this document is able to develop an instinct, and maybe even a passion, for continuing to learn and work toward ever more accessible web experiences as possible wherever your projects may take you.

----


## Images
  -


----

## [Promised Deliverables](inkdrop://note/TpFb7nmtQ)

## [Accessibility Audit Checklist](inkdrop://note/y54WgNQxT)

## [URI Metcalf SCIP Accessibility Audit Related Links](inkdrop://note/KS_8XHkQt)

----
