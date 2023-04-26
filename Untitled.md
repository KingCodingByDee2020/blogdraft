## 1. Folder structure

As best practice, we should organize our files into sub-directories:

- All stylesheets should be in a `css` folder
- All script files should be in a `js` folder
- All images should in an `images` folder
- index.html should be in the topmost level of the project folder

Make sure you update your file paths after modifying the folder structure. 

## 2. One of the requirements of this project is to use CSS `@import`

In CSS, the `@import` rule allows you to include one CSS file inside another. This can be useful when you want to split CSS code into smaller, more manageable files or when you want to reuse CSS code across multiple pages or projects.

Identify the different sections or modules of your CSS code that have a logical grouping or a clear separation of concerns. For example, you might have a separate section for typography, layout, navigation, forms, etc.

Then, create a new CSS file for each module that you identified in the previous step. Copy the CSS rules that belong to each module into the appropriate file, making sure to include any related styles such as media queries or pseudo-classes.

In the main CSS file that will be used on your website, use the `@import` rule to include each of the module files. You can use relative or absolute URLs to specify the file paths. For example:

```css
@import url('typography.css');
@import url('layout.css');
@import url('navigation.css');
@import url('forms.css');
```

## 3. No inline styling!

Make sure you move any inline styling to the external stylesheet!

### 4. Duplicate lines of code

Go back and review each `<link>` in your HTML files. You have a lot of duplicated code. For example, you've linked the following library more than once:

```
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
```

You only need one instance of each library.

## CSS

You have to split your CSS into smaller files and import it in your main stylesheet using @import and then link the main stylesheet to your HTML file.
You can easily do it by further splitting your CSS file into the following files:

main.css - Use only import statements here.
core.css - Add all the basic CSS common for all pages here
home.css - Add CSS related to the home page here
post.css - Add CSS specific to the blog-post page here
responsive.css - Add all the media queries here
Or alternatively on the basis of functionalities like this:

footer.css - Add CSS specific to the footer here

header.css - Add CSS specific to the header here
and similarly other parts of the page.
Just remember that you must have at least 3 imported files in the main CSS file and importing URLs doesn't count.

## HTML

Make sure to also use bold, italic, quotes and underline in your webpages as you have done for the other selectors.:pray:
You have to include <b> or <strong> for bold, <em> or <i> for italic, <q> or <blockquotes> for quotes and <u> for underline properties inside your paragraph tag.

Please make sure the homepage and blog post page follow the expected pattern mentioned in the specification.

Be sure to have cards and image captions in your webpages.

