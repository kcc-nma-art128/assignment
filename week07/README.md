# Week 7 - Sub Pages
Continuing coding Company Name site #1 with the goal of continuing the last step, sub pages.

### About sub page
1. Make a copy of `index.html` & rename it to `about.html`.

1. Change your page title in `<head>` to `<title>Company Name 1 | About</title>`.

1. Remove all contents of `.section01` & `.section02` from `<body>`. This should
   leave you with your `.header`, `.main-nav`, & `.footer`.

1. Add a `<main>` HTML5 tag which will hold the main content of our sub page.

1. Within `<main>`, add a container `<div class="container row">` which will contain our Article
   & Sidebar to fit our 960 grid. Don't forget `row` which is our clearfix to
   clear our floats.

1. Within `<div class="container row">`, add `<article>`(content of our article) & `<aside>`(sidebar). Lets give `<article>` a class of `article`, so we can style it using the class selector rather than an element selector, this way we'll be able to reuse the `<article>` tag elsewhere & have more control over styling. Same for the `<aside>` give it a class of `sidebar`. Your HTML should look like:

   ```html
   <main>
     <div class="container row">
       <article class="article">
         ...
       </article>
       <aside class="sidebar">
         ...
       </aside>
     </div>
   </main>
   ```

1. Grab the article contents from the PSD file. Wrap them in HTML tags where it makes sense. `<h1>` for our main heading, `<h2>` for sub heading, `<h4>` for the date, & `<p>` for our paragraphs.

   ```html
    <article class="article">
      <h1>Title of the Main Article</h1>
      <h2>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi semper, nunc quis euismod porta. Cras volutptat neque eget neque volutpat in congue diam eleifend.</h2>
      <h4 class="date">Date of Article MM/DD/YYYY</h4>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus scelerisque condimentum leo in porta. Pellentesque ac mauris diam, et scelerisque tortor. Cras volutpat neque eget neque volutpat in congue diam eleifend. Donec aliquam accumsan urna, volutpat semper augue lobortis eget. Maecenas condimentum est eu urna consectetur vestibulum. Curabitur eget purus massa, non lobortis ipsum. Nulla mollis rhoncus vehicula. Pellentesque nunc metus, posuere et pellentesque non, faucibus ut dui. Ut rhoncus iaculis est eget pulvinar. Mauris consectetur ornare quam, congue vehicula tortor pharetra et.
      </p>
      <p>
        Maecenas ac lacus massa, ac sodales velit. Nullam viverra felis quis mi volutpat non posuere lacus tempor. Aliquam erat volutpat. Curabitur pellentesque, nunc sed ornare ultricies, libero nibh convallis odio, sit amet pretium ante massa et erat. Nulla facilisi. In hac habitasse platea dictumst. Suspendisse non metus justo. Cras sapien turpis, convallis ac fringilla quis, aliquam egestas dui. Suspendisse mollis fringilla eros tempus congue.
      </p>
      <p>
        In hac habitasse platea dictumst. Vestibulum orci urna, egestas sit amet luctus eu, ullamcorper varius libero. Vivamus in diam mauris. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae.
      </p>
    </article>
   ```

1. Grab the sidebar contents from the PSD file. Our sidebar has two widgets, Sub Nav (Unordered List) & Testimonials (Blockquote/Paragrpah).

   ```html
    <aside class="sidebar">
      <div class="widget">
        <h3>SubNav</h3>
        <ul>
          <li><a href="#">Sub Section 1</a></li>
          <li><a href="#">Sub Section 2</a></li>
        </ul>
      </div>
      <div class="widget">
        <h3>Testimonials</h3>
        <p>
          “Curabitur a nunc at arcu elementum tincidunt. Sed sit amet turpis sed tortor venenatis lacinia. Suspendisse ut felis in tortor porttitor euismod.”
          - John Doe
        </p>
      </div>
    </aside>
   ```

1. Now onto our styles.

   ```css
    /* ABOUT PAGE */
    main {
      background: #fff; /* Bring back our white background so our text is readable again */
      padding: 3em 0; /* Give our main section space */
    }

    .article {
      width: 62%; /* 580px / 940px * 100 = 61.7% */
      float: left; /* First column is floated left. This is to align our .article & .sidebar into a two column layout. */
    }

    .article h1 {
      margin-bottom: 0.15em;
    }

    .article .date {
      margin-top: 3em;
      margin-bottom: 1.5em;
    }

    .sidebar {
      width: 30%; /* 280px / 940px * 100 = 29.7% */
      float: right; /* Second column is floated right. This is to align our .article & .sidebar into a two column layout. */
    }

    .widget {
      background: #ccc; /* Set our widget background to light gray */
      padding: 2.1em; /* Add space around the content & expand the background  */
      margin-bottom: 1.5em; /* Push down anything under a .widget, in this case it will push down the second .widget to give it a space in between. */
    }

    .widget h3 {
      border-bottom: 4px solid #000; /* Add a black 4px border bottom */
      padding-bottom: .2em; /* Give space in between content & border. This will push down the border-bottom. */
      text-transform: uppercase; /* Make all the text uppercase */
    }

    .widget ul {
      list-style: none; /* Remove disc (filled circle) on unordered list. */
      margin-bottom: 0;
    }

    .widget li {
      margin-left: 0; /* Remove default margin left on list items */
    }

    .widget p {
      font-size: .75em; /* 12px / 16px = .75em */
      line-height: 1.6em; /* 20px / 12 = 1.6em */
      margin-bottom: 0;
    }
   ```

1. Make it responsive. On mobile we'll want to make it one column rather than two.

   ```css
    /* MOBILE */
    /* Anything below 767px */
    @media only screen and (max-width: 47.9999em) {

      .section01 .col-1,
      .section01 .col-2,
      .section02 .col,
      .footer .col,
      .footer .col:last-of-type,
      .article,                   /* Add .article */
      .sidebar {                  /* Add .sidebar */
        width: 96%;               /* width 96% + margin-left 2% + margin-right 2% = 100% */
        float: none;
        margin: 1em 2%;
      }

    }
   ```


## Homework:
- Finish Site #1 (Company Name 1) by completing Step #6. Be sure to work in a new (separate) folder.
- Update your Art 128 website, make sure you have Company Name 1, steps 1-6.
- Get familiar with GitHub, go through [GitHub tutorial](https://guides.github.com/activities/hello-world/). You should have a hello-world repository under your github account. Your hello-world repository should have a branch, commits, & a pull-request which they go over in that tutorial.
- Download [GitHub Desktop](https://desktop.github.com/) & go through their git tutorial, the tutorial should start the first time you open the app.
