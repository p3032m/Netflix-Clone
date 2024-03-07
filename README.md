# Netflix-Clone
Clone of the Netflix website as a light HTML CSS and JS excercise - Take a look

Practice
Eating website for fun... nyom nyom nyom"

![image](https://github.com/p3032m/Netflix-Clone/assets/63456693/d8cd6498-a422-4e5a-a0de-95feeedca830)
What it is
A basic warmup exercise. Simple, practice oriented, clone of the Netflix Homepage. Built with:

HTML
CSS
Vanilla JS - ES6
Awesomeness - Strictly for the love of coding :-)
What it does
Look pretty, that's about it :-)
Learning Points
CSS Grid
Styling Tables
Tabs with Javascript
Positioning
Some cool stuff
Usually, people tend to run to CSS Frameworks to develop and style tabs and switching tabs. But here's a pretty simple, basic way of creating switchable tab content using Vanilla JS:
const tabItems = document.querySelectorAll(".tab-item");
const tabContentItems = document.querySelectorAll(".tab-content-item");

// Select tab content
function selectItem(e) {
  removeBorder();
  removeShow();
  // Add border to current tab
  this.classList.add("tab-border");
  // Grab content item from DOM
  const tabContentItem = document.querySelector(`#${this.id}-content`);
  // Add show class
  tabContentItem.classList.add("show");
}
function removeBorder() {
  tabItems.forEach(item => item.classList.remove("tab-border"));
}
function removeShow() {
  tabContentItems.forEach(item => item.classList.remove("show"));
}
// Listen for tab click
tabItems.forEach(item => item.addEventListener("click", selectItem));
And HTML is all you need 

<!-- Content Pretty Long so I'll add later -->
<!-- But this is the basic gist -->
<div class="tab-item">
  <!-- Selectors for the different tab content -->
</div>
<div class="tab-content-item">
  <!-- Content of each tab item -->
</div>
<!-- Simply add more selectors and corresponding 
tab content for each selector -->

  


Features in Development
I might add the other pages on the Netflix website if I ever come back to refactor ^-^

Contribution
Contributions are highly welcome. Feel free to fork, clone, make pull requests, report issues etc.

Acknowledgments
Many thanks to @bradtraversy for his awesome courses - i will not fail you sensei
Thanks to @torvalds For Making the world a better place
And To anyone reading this... You're awesome!
That being said

To the Front... to the Back... End to End... cut no slack. Making ends meet. lol
