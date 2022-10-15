# CSS - Technical Interview Questions

## Questions:

- [1] What is a CSS selector specificity and how does it work?
- **Explanation:** A CSS selector specificity determines which CSS elements are applied based on the specificity level of the individual selectors.

- **Use:** When an element's styling conflicts, specificity is taken into account and helps control which styles are applied to the HTML element. 

- **Example:** An example would be applying a higher specificity like another class or ID to target an individual element..

- [2] What's the difference between "resetting" and normalizing CSS? Which would you choose, and why?
- **Explanation:** Resetting strips all default browser settings where as normalizing preserves default tyles over non styled.

- **Use:** reset allows us to have a blank canvas so we can add our own customized styles and normalize allows us to perserve basic porperties such as box-sizing border box.

- **Example:** if my page styles don't render on a specific browser then I can use reset to clear all style and normalize to retain all browser settings.

- [3] Describe floats and how they work.
- **Explanation:** Floats are boxes trying to fight their way into a corner, this can be controlled by specifying their parent element/container with the property position: relative;  

- **Use:** you can use floats as a styling technique to position elements on your page within a parent element 

- **Example:** floating text around an image.

- [4] Describe z-index and how stacking context is formed.
- **Explanation:** Z-indexing is stacking your elements on your page to create overlapping effect

- **Use:** you would use this to place your text over an image or buttons on a card to create depth

- **Example:** In 2D gaming you would use z-indexing to overlay design templates on your canvas. 

- [5] Describe BFC (Block Formatting Context) and how it works.
- **Explanation:** block formatting is the same as placing your boxes inside of other boxes in a z indexing format placing floated elements under an image rather than around.

- **Use:** I would use block formatting to prevent margin collapse

- **Example:** when we want to have a navbar that scrolls with the page. triggering this event by using static positioning.

- [6] What are the various clearing techniques and which is appropriate for what context?
- **Explanation:** clear in general is used to specify floating elements that are not allowed to float. we do this three different ways
    1. clear
    2. overflow
    3.  clearfix-hack

- **Use:** 1. clears a speciic side of a floated object with the properties none, right, left, both, initial, and inherit
2. If the element is taller than the element containing it then we would want to use overflow.
3. this is a way for an element to auto clear or fix its elements so that it does not need to add additional markup.

- **Example:** 1. to remove float from the left side of an element we'd use clear: left;
2. to place a tall div/section within a containing element 
3. to pull text to fit an image we'll use clear-fix.

- [7] Explain CSS sprites, and how you would implement them on a page or site.

- **Explanation:** conbine multiple images into one image.

- **Use:** used for logos or to create icons that minimize the number of http requests.

- **Example:** gmail app icons 

- [8] How would you approach fixing browser-specific styling issues?
- **Explanation:** I would use normalize.cs to normalize box sizing and I would use reset to be able to apply my own styles to the page.

- **Use:** normalize would revert the browser to preset styling and reset would clear any styles outside of those preset so that my style will be present on the page.

- **Example:** If my backgruond gradient doesn't load in safari, my normalize and reset stylesheets will fix this issue. 

- [9] How do you serve your pages for feature-constrained browsers? What techniques/processes do you use?
- **Explanation:** we serve our pages with graceful degradatiom and progressive enhancement in a process using autoprefixer for vendor prefix insertions, a modernizr feature detection, or a CSS support query. 

- **Use:** graceful degradation - this is the process of building an app that is functional across new browsers as well as old browsers

progresive enhancement - this is the practice of building an app for the most base level of UX, while also adding functional enhancements when a browser supports it. INO layering the features on with broswer compatibility. 

- **Example:** an example of graceful degradation would be a site that isnt very asethetically pleasing whereas a site that is progressively enhanced is one that layers on the beauty depending on how much bandwith you have. 

- [10] What are the different ways to visually hide content (and make it available only for screen readers)?
- **Explanation:** you can set the width and height to 0 to make the element not take up any space on the screen at all. 
you can also position an item outside of the screen with position:absolute; left: -99999

- **Use:** for mobil development 

- **Example:** adding an ARIA tag on a form so that users know what input is being asked. 

- [11] Have you ever used a grid system, and if so, what do you prefer?
- **Explanation:** yes, I highly prefer grid paired with flexbox to allow more creative abilities.

- **Use:** positioning items on the page in a grid layout controlling columns with grid-template-row and grid-template-clumns then using grid properties to align content.

- **Example:** I used grid to position three cards onto one of my projects, paired with flexbox I was able to position content exactly how I wanted.

- [12] Have you used or implemented media queries or mobile specific layouts/CSS?
- **Explanation:** yes, Media queries allow us to set up our site for mobile development without crowding our page layout.

- **Use:** to make a site responsive I've used media queries to use one fluid design over all devices with specific screen sizes. 

- **Example:** creating a hambuger menu or creating a media scroller. 

- [13] Are you familiar with styling SVG?
- **Explanation:** yes SVG or scalable vector graphic file is a file format used for displaying 2D graphics, c harts, and illustrations on websites. 
- **Use:** coloring shapes, an embedded css section, or an external css files.
- **Example:**

- [14] Can you give an example of an @media property other than screen?
- **Explanation:** @media all - which is used for all media type devices
- **Use:** I would use one of the @media properties to target a specific media
- **Example:** I've used media @ all to target all buttons on a page and styled them with one code block. 

- [15] What are some of the "gotchas" for writing efficient CSS?
- **Explanation:** some gotchas for writing efficient css is writing semantic code with clear identifiers to target when styling elements.
- **Use:**Using css selectors, avoiding universal selectors like tag names, and making your rules as specific as possible. 
- **Example:** Creating a class or id to target a specific section heading 

- [16] What are the advantages/disadvantages of using CSS preprocessor?
- **Explanation:** the advantages of using CSS is that it's more maintainable, easier to write nested selectors, and it includes SASS features likes loops, lists, and maps configuration easier and less verbose.
   - the disadvantages of using CSS is that it requires tools for preprocessing making re-compilation times slow.

- **Use:** can be used to write computational logic within CSS.

- **Example:** one example of using a preprossor is creating css variables to easliy access color values

- [17] Describe what you like and dislike about the CSS preprocessor you have used?
- **Explanation:** I like that it makes selecting color values easier or for example if I wanted to create a site with dark and light mode, I would create a CSS conditional and change the properties within.

- **Use:**
- **Example:**

- [18] How would you implement a web design comp that uses non-standard fonts?
- **Explanation:** Use @font-face which specifies a custom font and define font-family for different font-weights 
- **Use:** uses would be specify a custom font
- **Example:** setting the font-style property to oblique which slightly slants font. Not to be confused with setting to italic. 

- [19] Explain how a browser determines what elements match a CSS selector.
- **Explanation:** Browers match selectors by filtering out all elements in the DOM according to the key selector and traverses up to its parent element via the cascade. 

- **Use:** iF I want to style a span within my pararaph tag then I need to target the specifity of the span so the browser knows where to look.

- **Example:**for my portfolio I have three cards, however, I wanted to style only one of those cards, I could have used nth-child: but instead I targeted the span directly within its parent element.

- [20] Describe pseudo-elements and discuss what they are used for.
- **Explanation:**   Pseudo-elements allow you to insert content onto a page without it needing to be in the HTML. 

- **Use:** Think of this as adding style to any one element on the page
- **Example:** If I want to make the first letter of a paragraph stand out then I want to use the pseudo-element ::first-letter.

- [21] Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
- **Explanation:** The box model is the idea of looking at everything on a page as a box depending on the contents inside of them.

- **Use:** adding additional padding, margin, or even a border on your element moves it around it's parent container or the items within it.

- **Example:** an example would be if I had a section and I wanted to center it without using a float/flex/or grid element, I would change the margin and paddig.

- [22] What does *{box-sizing: border-box} do? What are its advantages?
- **Explanation:** box-sizing:border box sets an elements width and height which will be factored into final renerding of said box, including any border of padding.

- **Use:** You would want to use this to style a section/div container.

- **Example:** I've used content border box for creating a bold header to my portfolio, I didnt want the img to be effected when I styled my nav buttons so I used border box to set the initial height and width of the box then styled my nav within those limits using the space available. 

- [23] What is the CSS display property and can you give a few examples of its use?
- **Explanation:** The display property controls what and how elements will appear on the site. 

- **Use:** If I want to set up a slider, I want to hide any overflow and show only the content that fits inside the specified container (in this case my slider)

- **Example:** 
    - display: none (shows nothing)
    - display: grid ( displays elements in a grid style)
    - display: flex ( displays elemets with flex properties that allow us to remove them from normal web flow.)

- [24] What's the difference between inline and inline-block?
- **Explanation:** the main difference is that inline-block doesn't add a line-break after the element so that the elements can sit directly next to eachother. You would use inline for spans or small one liners.

- **Use:** you would use inline-block when you want to control height and width of items without them appearing on a new line. inline-elements do not start on a new line and only take up as much space as its content.

- **Example:** When you want to include an img in your html next to a paragraph, you can't really do much to change it vs if you were to place it inside of a div/section unless you set the property to inline-block 

- [25] What's the difference between a relative, fixed,, absolute and statically positioned element?
- **Explanation:** relative refers to the parent container, absolute refers to the ability to move freely around a parent element, fixed keeps the item in place no matter how much you scroll it will always be in that spot, static elements flow with normal page flow

- **Use:** I would use these properties to position content on the page.

- **Example:**I would use static to keep things in normal flow, I would use absolute to move items within a parent container freely, I would use relative to act as a containing element for position absolute items.

- [26] What existing CSS frameworks have you used locally, or in production? How would you change/ improve them?
- **Explanation:** I'm familiar with bootstrap and tailwind, I've used tailwind locally with projects 

- **Use:** many companies use tailwind or bootstrap on their merchant sites creating UI for their products.

- **Example:**I used tailwind to quickly add custom UI on a card for a personal project  

- [27] Have you played around with the new CSS Flexbox or Grid specs?
- **Explanation:** yes, I use them interchangably, flex is for modifying columns or rows where as grid modifies columns AND rows.

- **Use:** I would use grid to set the overall layout of the page and flex to place items how I want them to look in place. 

- **Example:** I used grid to set the position of media content on a news site mockup and then flex to control the contents within a parent container. 

- [28] Can you explain the difference between coding a website to be responsive versus using a mobile-first strategy?
- **Explanation:** coding a website to be responsive requires you to do more configuration when minimizing content on your page whereas mobile first allows you to take what is small and expand upon it. 

- **Use:** I would use mobile first strategy when I have a site that I have base main content that I want to include on my site and then gradually build upon, I would use a responsive strategy to condense a larger site down to the bare necessities.

- **Example:** building a portfolio, I want the user to visit my site and know that I provide services, how to contact me, and a little information about myself, as there is more screen size available, I will add more features like an api of a calendar, or a link to all my projects. 

- [29] How is responsive design different from adaptive design?
- **Explanation:** A responsive design can change its layout and appearance based on the screen size of the device being used. An adaptice design requires the creation of a different layout for each device the website will be accessed. 

- **Use:** You would use responsive design works for bigger sites that are designed from scratch. 
an adaptive often works best for smaller sites that are being rredesign and enhancement.

- **Example:** A responsive site example would be creating a site for a product that I'm creating and I want to account for all screen sizes mobile or not. An example of an adaptive site if say a client now needs a mobile layout for an existing website with no intention of changing anything you would adapt your site to be mobile accessible. 

- [30] Have you ever worked with retina graphics? If so, when and what techniques did you use?
- **Explanation:** I'm not familiar with retina graphics, but I do know of them. Basically they are used for including high-res graphics but only for screens that can make use of them

- **Use:** The new apple uses bright colors and high res to intice users into buying their devices but in relaity it's just a regular phone and does all the same things the last upgrade did. 

- **Example:** Let’s say you had three major breakpoints in a design. This design also had a large background graphic and you wanted it looking it’s best on any screen (retina or not) and not waste any bandwidth. You’d set up 6 media queries, one for each breakpoint and one for each one of those breakpoints on retina. Then you’d override the background image all the way down. ***SEE: https://css-tricks.com/snippets/css/retina-display-media-query/

- [31] Is there any reason you'd want to use translate() instead of absolute positioning, or vice-versa? And why?

- **Explanation:** translate() is more efficient and will result in shorter paint times for smoother animations. When using translate(), the element still occupies its original space (sort of like position: relative), unlike in changing the absolute positioning.

- **Use:** you'd use to almost create a ghost effect to an element.

- **Example:** Just as you would edit an element properties using top, bottom, left, and right; you can use translate() paired with transition to move an element around the x y or z axis so like if I want to create an image slider I would use transition:translate() to create an offset image to the left on the x axis say  -45px and up 23px.