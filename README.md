# Analogue Sound World

Analogue Sound World is a website for a musical equipment store, specialising in an analogue synthesisers. Website should give visitors an insight of available instrument choices, including portable low cost options to try generation of analogue sounds.

## Rationale

The website is built taking in account potential user needs. Before creating the site I wrote a few user stories from which I took user needs.

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

## Design choices

* The website has a Bootstrap grid layout to provide resposivenes for different screen sizes.
* As the site isn't text-heavy I have  chosen dark mode.
* Content sections are short and they are aligned across the page width with the links to each section in navbar. Products sections and vintage instruments section with enquiries form has separate pages.

## Typography

* For main content I used inter font with sans-serif as a fallback font.
* Heading elements have quantico font and serif as a fallback. Headings are in light gray colour with less contrast than smaller text.
* Navbar and footer have bright background colour and dark font colour as main content background.
* Links are set inconspicuously in surrounding text using websites custom colors.

## Site features

* Navigation fixed on the top of the screen with a toggle button for smaller screen sizes.
* Products list consisting of cards with representative images for visual engagement. Where applicable links to producers' websites are embedded in card headers.
* Information about reselling vintage instruments with contact form for enquiries.
* Contact details section with opening times and links to social media sites.

## Technologies used

* HTML, CSS, Bootstrap, Javascript.
* Squoosh to resize and compress images for web use.
* To generate a colour palette from the uploaded image I used  <http://colormind.io> . As some results lacked acceptable contrast I used <https://mycolor.space/> generator to expand the colour palette.
* For checking contrast I used <https://webaim.org/resources/contrastchecker/> .
* Visual Studio Code as an IDE. I used some Copilot suggestions, but noticed it's limitations leading to errors (e.g. using “\” instead of “/” in links).

## Testing

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
