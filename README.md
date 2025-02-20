# Analogue Sound World

Analogue Sound World is a website for a musical equipment store, specialising in an analogue synthesisers. It gives visitors an insight of available instrument choices, including portable low cost options to try generation of analogue sounds.
Website is deployed here: <https://andiskrams.github.io/Analogue-Sound-World/>

## Rationale

I wanted to use my knowledge of HTML and CSS to create a website for a musical instruments shop, showing accessibility of analogue synthesizers with examples of modern analogue synthesisers. It must demonstrate that analogue synths nowadays are not wall to wall equipment and small devices have a lot of functionality.
The website must show stores location, easy to find for visitors.
I started to create the project taking in account potential user needs. Before creating the site I wrote a few user stories from which I took user needs.

### User stories

* As a site visitor I need easy navigation and a user-friendly design, with a responsive layout for my device, so I can find information easily.
* As a musician I need to know what equipment is available in the shop.
* As a Prospective Customer, I need to find essential information such as location, contact details, and opening hours, so I can easily plan my visit or get in touch with the shop.
* As a vintage instrument owner, I need to get in touch with the shop about reselling my gear.
* As an amateur musician, I need to know about low cost options to try analogue synthesisers.
  
### Site owners goals

* To show prospective customers the range of products available in the shop.
* Clearly show location and opening times.
* To help interessents get in touch via contact form.

According to those needs I decided what features to include.

### Site features

* Navigation fixed on the top of the screen with a toggle dropdown button for smaller screen sizes. On left side are logo image with link to homepage. At the end of homepages content there are links to other pages embedded in text.
* Separate page with products list consisting of cards with representative images for visual engagement. Where applicable links to producers' websites are embedded in card headers. Although products page don’t have a lot of information, dedicated page allows for future development to add more product groups. It might become especially useful if implementing an e-commerce option.
* Information about reselling vintage instruments with pop-up contact form for enquiries.
* Footer with stores address, contact details and opening times; links to social media sites.

### Potential features left to implement

* Product image cards footers can have dropdowns with technical details. Some of currently existing footer content can be moved to dropdowns, reducing card height.
* Another modal which appears after submission of the form, showing confirmation of submission.
* “About” page telling more about the shop

## Design choices

* The website has a Bootstrap grid layout to provide resposivenes for different screen sizes.
* As the site isn't text-heavy I have  chosen dark mode.
  Colours used: ![colour palette](assets\documentation\colors.JPG)
* Content sections are short and they are aligned across the page width with the links to each section in navbar. 

## Typography

* For main content I used inter font with sans-serif as a fallback font.
* Heading elements have quantico font and serif as a fallback. Headings are in light gray colour with less contrast than smaller text.
* Navbar and footer have bright background colour and dark font colour.
* Links are set inconspicuously in surrounding text using websites custom colors.

## Technologies used

* HTML, CSS, Bootstrap, Javascript.
* Squoosh to resize and compress images for web use.
* To generate a colour palette from the uploaded image I used  <http://colormind.io> . As some results lacked acceptable contrast I used <https://mycolor.space/> generator to expand the colour palette.
* For checking contrast I used <https://webaim.org/resources/contrastchecker/> and on website preview I used inspect inspect tool to check contrast of particular elements.
* Visual Studio Code as an IDE. I used some Copilot suggestions, but noticed it's limitations leading to errors (e.g. using “\” instead of “/” in links).

## Testing

### Manual

Initial testing showed products cards aligned left. ![card alignment](assets\documentation\card-alignment.JPG)

Using the inspect tool I found that those image cards lack justify-content-center class. Moving the closing tab of div with that class below products cards solved an issue.

At the very end of testing I noticed a small blue line after the Youtube icon. ![blue line](assets\documentation\blue-line.JPG)

I tried to change the icon to square one, but it didn't look good with current styling. Instead I changed the order of social media icons with Youtube at the end. That removed the appearance of the blue line.

I tested the deployed website on Chrome, Edge and Firefox browsers. It looks good and is responsive for various screen sizes. Navigation links work and external links open in a new window.

### Lighthouse

Early testing showed some issues with performance.

![Lighthouse Home](assets\documentation\home_lighthouse.JPG) ![Lighthouse Products](assets\documentation\products_lighthouse.JPG)

Closer look at the code revealed some unnecessary sub-divs with repeating classes. Cleaning of the code significantly improved performance with scores close to 100%.

![Home Lighthouse Final](assets\documentation\home_lighthouse1.JPG) ![Products Lighthouse final](assets\documentation\products_lighthouse2.JPG) ![Vintage Lighthouse final](assets\documentation\vintage_lighthouse_final.JPG)

Although testing of Products page is inconsistent, often showing NO_LCP Error and needs repeated tests to get performance score.

### Validators

#### HTML

<https://validator.w3.org> showed lot of errors apparently originating from code formatting and Copilot suggestions.

![HTML errors](assets\documentation\errors.JPG)

I fixed indicated errors.

![Fixed HTML](assets\documentation\no_errors.JPG)

#### CSS

<https://jigsaw.w3.org/css-validator/> showed one error:

![css jigsaw](assets\documentation\css.JPG)

I fixed it replacing value with 0.

![corrected css validator](assets\documentation\css-corrected.JPG)

### Unsolved bugs

Products page needs javascript code to collapse navbar on small screens, when navigating to same page sections.

![Non-collapsing navbar](assets\documentation\non-collapse.JPG)

## Deployment

* The site was deployed to GitHub pages. The steps to deploy are as follows:
  * In the GitHub repository, navigate to the Settings tab
  * From the source section drop-down menu, select the Master Branch
  * Once the master branch has been selected, the page will be automatically refreshed with a detailed ribbon display to indicate the successful deployment.

The live link can be found here - <https://andiskrams.github.io/Analogue-Sound-World/>

## Credits

### Media

* Favicon [Icon by Freepik](https://www.freepik.com/icon/sound-waves_555253#fromView=search&page=5&position=66&uuid=bc04230f-45ca-4ea9-a74f-55951ca2b7e8). I created it here: <https://favicon.io/favicon-converter/>
* Image on navbar is from <https://pngtree.com/>.
* Hero image croped from image by Daniel Spils. License: <https://creativecommons.org/licenses/by-sa/2.0/>
* Vintage page image by Mack Male. License: <https://creativecommons.org/licenses/by-sa/4.0/>
* Images in products section are from <https://www.pexels.com/> keyboard.webp by TStudio, modular.webp by Carlos Santos, sound-equipment.webp by Pok Rie. Drum-machine.webp by Ashley Pomeroy, license <https://creativecommons.org/licenses/by-sa/4.0/>
* Mini section images are from Behringer and Korg websites.

### Content

* On homepage introductory text are from <https://www.pmtonline.co.uk/>.
* Products cards footer text are from Behringer and Korg websites.
* The rest are written by myself. On vitage page large parts of text are built from Copilot suggestions.

### Code

* For responsive layout, navbar, image cards and pop-up modal with contact form I used components from <https://getbootstrap.com/> and modified them for the sites content.
* JavaScript code for Bootstrap mobile navbar collapse is from Code Institute "Boardwalk Games" walkthrough project.

### Fonts

Fonts from <https://fonts.google.com/>

* Inter by Rasmus Andersson
* Quantico  by MADType
