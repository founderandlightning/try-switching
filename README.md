### TrySwitching

> TrySwitching is a serrvice enabling users to switch their providers.

We are using switching providers for:
- Broadband (done)
- Energy (done)
- Charging electric cars (work in progress)

### Project desc F+L template

1. Main technologies/frameworks/languages used for developing the project
	- JavaScript
	- RestAPI
2. Code Quality
	- Modularity of components
3. Code Review
	- Review on special custom pages. Before pushing on production for example the “page_name” page, create a “page_name_test” page and push it live. However do not link it anywhere so only a tester can access it.
4. Managing Credentials
	- Managing Credentials in HubSpot Setting
5. Hosting
	- Hosting by HubSpot
6. Environments
	- IDE by HubSpot
7. CI and deployment
	- no CI in the project
8. Error handling
	- Handling error in Code Review process written in point 3.
9. Performance monitoring
	- Not implemented
10. Log monitoring
	- Not implemented
11. Backups
	- Backups by HubSpot
12. Tests
	- Automated tests not implemented
13. Git workflow
	- Not implemented

### Tech

The tool for creating the product is [HubSpot](https://www.hubspot.com/)
The project id is 8966293.

You can downland the project locally and open it in your IDE or you can open it in HubSpot's IDE.
To do this navigate to Marketing -> Files and Templates -> Design Tool.

### Project structure

To get into project's theme go to 'try-switching' folder in project's root.

#### Assets 
Folder consist fonts, css files and js files.
If you want to add a css file you must remember to style.css.
Fonts are declared in main.css.

- Styles -> Components - folder consist reusable elements used in different modules. 
- Styles -> Modules - folder consist styling for global modules
- Styles -> Templates - folder consist styling for dynamic themes
- Styles -> Utils - folder consist mostly 3rd party css rules
- JS folder consist subfolder for every template with JS functionality named by page's template ( f.e. JS -> homepage ).
- JS -> step_two and ste_three flies are responsible for 'Help me choose' functionality in main modal component. 
- JS -> addressPopup - file consist validation and cashing user's postcode input in main search form.
- JS -> getBlogs - file consist HubSpot's API function for receiving blogs.
- JS -> graphQL - file consist POST call to 3rd party StickeeAPI for receiving broadband deals for specific postcode.
- JS -> postcoderAPI - file consist GET call to 3rd party PostCoderAPI for receiving addresses for specific postcode.
- JS -> postcoderEmail - file consist POST call to HubSpots submissions.


#### Layouts
In this folder are located html templates for most outer components for pages.
Here you can edit <head> and <body> tags. 

#### Themes 
In this folder are themes for pages with dynamic content (blog listing and blog post)

#### Other
The files outside of any of those folers should have .html extension (Despite the theme.json which is a config file).
These files are custom static pages templates.

