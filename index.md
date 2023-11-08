---
title: Home
layout: home
nav_order: 0
---
<p><button class="btn js-toggle-dark-mode">Preview dark color scheme</button></p><script> const toggleDarkMode = document.querySelector('.js-toggle-dark-mode'); jtd.addEvent(toggleDarkMode, 'click', function(){ if (jtd.getTheme() === 'dark') { jtd.setTheme('light'); toggleDarkMode.textContent = 'Preview dark color scheme'; } else { jtd.setTheme('dark'); toggleDarkMode.textContent = 'Return to the light side'; } }); </script>


To have all the information about rge Breed School application in one place and allow people involved to contribute to the documentation, this iste is set up.

We explain about the purpose and the working of the site, links to the code and where it is deployed can be found here.

We are in the process of setting up a stagiong environment which wil function as a test environment as well. Every role within the application wil have a demo login, so evreyone interested can have a look.
We are also setting up a small apllication that logs in as a User with a certain role, visits all the pages within that role and takes a screenshot and stores it.
You can see the results [here](https://wijnandb.github.io/screenshots_automated/)

Before we can launch that application properly, we need to fill the staging environment with fake data. To do this, we can either manually create fixtures, or have them created by Faker.

