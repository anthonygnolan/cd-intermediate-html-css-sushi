## Design some themes

+ Let's design a theme for the Attractions page that's different from the other pages. Go to your stylesheet file and add the following. Be sure to include the dot in front!
   
```css
  .pupleBackground {
      background-color: #9f80ff;
  }
```

The dot makes this into a **class selector**. With a CSS **class** you can apply a set of CSS rules to any element on your website by adding an **attribute** to the element.

+ If you want to, you could pick the colour to match the background of your page!

+ Now go to `attractions.html` \(or the page you're working on if you're using your own project\) and add the following **attribute** to the `article` tag:

```html
  <article class="purpleBackground">
```

You should see the background change around the text on the page.

+ Add the following class to your stylesheet:

```css
  .greenBackground {
      background-color: #48D1CC;
  }
```

+ Back in the **html** file, add the **attribute** `class="greenBackground"` to each of the `section` tags, just like you did for the `article` element. Look at your web page on the right and compare it to the other pages that have `section` elements.

When you use a CSS **element selector** such as `section`, the style rules apply to **all** the elements of that type on your website. With CSS **classes** you're able to just change **some** of them. You can add more than one class to an element too. 

+ Let's make another CSS **class** to give the sections some margin and padding. In `styles.css`, add the following code:

```css
    .sectionSpacing {
      padding: 10px;
      margin-top: 20px;
    }
```

+ In the **html** page you were working on, add the new class to each of the sections like this:

```html
  <section class="greenBackground sectionSpacing">
```

You can add as many CSS classes to an element as you like. Just write the names of all the classes you want to use inside the **class attribute**, and separate them with spaces.

+ How about re-vamping the Food page? \(If you're using your own website, you'll need another page with some **sections** on it\) Add the following classes to your stylesheet:

```css
  .yellowBackground {
    background-color: #FFFFCC;
    color: #A52A2A;
  }

  .solidRoundBorders {
    border-style: solid;
    border-width: 2px;
    border-color: #F5FFFA;
    border-radius: 10px;
  }
```

+ Go to the `food.html` file \(or your own file\) and add the new classes as well as the `.sectionSpacing` class to each section:

```html
  <section class="yellowBackground sectionSpacing solidRoundBorders">
```

Notice how you can mix and match the classes in your element's class attribute? Using CSS classes lets you **reuse** the same set of style rules on lots of elements. You can apply them to any element that has the properties you've set. 

+ Go to `index.html` and add the `solidRoundBorders` class to the picture of Tito.

```html
    <img class="solidRoundBorders" src="tito.png" alt="Tito the dog" width="100px" />
```

+ Why not experiment with some more CSS classes to make the other pages have their own themes? You can name a CSS class anything you like. It's common to give it a name that describes what it does or what it's for!

+ Extra challenge: use CSS **classes** to define a few different picture sizes for the website, for example `.smallPictures` and `.mediumPictures`. Then remove the `width` attribute from each of your `img` elements and add the appropriate class instead.