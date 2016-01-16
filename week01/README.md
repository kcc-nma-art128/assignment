# Week 1 - Intro to the Course

## Text Editor
*A good text editor is a developer's best friend.*

The text editor is where we'll spend most of our time writing code.
There are many text editors to choose from. To list a few there's [Atom](http://www.atom.io/), [Sublime Text](http://www.sublimetext.com/), [Brackets](http://brackets.io/), [Visual Studio Code](https://code.visualstudio.com/), [Adobe Dreamweaver](http://www.adobe.com/products/dreamweaver.html).
they let you view full directories and open files in different tabs, navigate easily using keyboard shortcuts, highlight different bits of syntax in many languages (very helpful) and have efficiency-gaining code snippets you'll get more familiar with over time.

### Atom
A Hackable Text Editor for the 21st Century.

[![Atom](https://atom.io/assets/screenshot-main-f609d95c29e5190787970f8c83762fcb.png)](https://youtu.be/Y7aEiVwBAdk)

**Features:**
- Built-in package manager
- Smart autocompletion
- File system browser
- Multiple panes
- Hackable/Customizable

Atom is an open source cross-platform editor. There are [builds available for Mac, Windows, and Linux](https://github.com/atom/atom/releases/).


## HTML
HTML (Hyper Text Markup Language) is a markup language for describing web documents (websites). The markup tells the Web browser how to display a website's words and images to the user.

```html
<!DOCTYPE html>               <!-- Tell the browser what type of document they're looking at. -->
<html>                        <!-- html tag is the container for all other HTML elements -->
  <head>                      <!-- head is a collection of metadata for the Document-->
    <meta charset="UTF-8" />  <!-- Specify character encoding for the HTML document -->
    <title></title>           <!-- Title for the document -->
  </head>
  <body>                      <!-- This is the document's body -->
    <h1></h1>                 <!-- Define HTML headings -->
    <h2></h2>
    <h3></h3>
    <p></p>                   <!-- Define a paragraph -->
    <ul>                      <!-- Define an unordered list -->
      <li></li>               <!-- Define a list item -->
    </ul>
    <ol>                      <!-- Define an ordered list -->
      <li></li>
    </ol>
    <a href="#"></a>          <!-- Define a hyperlink -->
  </body>
</html>
```


## Web Hosting

#### Domain Name System
The domain name system, more commonly known as "DNS" is the networking system in place that allows us to resolve human-friendly names to unique addresses.

#### Domain Name
A domain name is the human-friendly name that we are used to associating with an internet resource.

#### IP Address
An IP address is what we call a network addressable location. Each IP address must be unique within its network.

#### Top-Level Domain
A top-level domain, or TLD, is the most general part of the domain. The TLD is the furthest portion to the right (as separated by a dot).

#### Hosts
Web host stores all the pages of your website and makes them available to computers connected to the Internet. Within a domain, the domain owner can define individual hosts, which refer to separate computers or services accessible through a domain.


## FTP
FTP (File Transfer Protocol) is a way to transfer files between hosts over the internet. It is especially helpful as a way to upload or download files to or from a site quickly.

### FileZilla
FileZilla is a free FTP application [available for Mac, Windows, and Linux](http://www.filezilla-project.org/download.php?type=client).

**Set up FileZilla:**

1. Open the Site Manager by clicking the 1st icon on the topbar or navigating `File > Site Manager`.

1. Site Manager window should pop up.

  1. Click the New Site button.
  1. Enter your Host name. (Domain name or IP Address)
  1. Protocol: Select "FTP - File Transfer Protocol".
  1. Encryption: Select "One use plain FTP".
  1. If you're on a public computer, set Logon Type to "Ask for password".
  1. Username can be found by visiting FTP Accounts section of the cPanel.
  1. Click the Connect button.
  1. Enter your password (cPanel password).

  ![Site Manager](http://i.imgur.com/lxpw9aT.png)

1. Once you've logged in, all your files and folders on your server will be viewable. Go into `public_html` folder, which is the web root for your primary domain name.  

1. The easiest way to copy files to and from the server is to simply drag-and-drop into the `public_html` folder.


## Homework:
- Set up your class web page. All students are required to have hosting space to post their designs, assignments, and ultimately their final web site. Students are required to purchase a hosting plan with a third party hosting provider. Past students have purchased hosting plans from [Bluehost](http://www.bluehost.com/), [NameCheap](http://www.namecheap.com/), [HostGator](http://www.hostgator.com/), and [GoDaddy](http://www.godaddy.com/) (these are just a few of many hosting providers available). Plans should include ample disk space (ie. more than 2GB or unlimited), support for CGI, PHP, and MySQL, multiple domain hosting (to host more than one site), one-click install/support for Wordpress, Joomla, and Drupal (popular CMS options), and a low, competitive price (an example rate is around $3-$5/month – this is subject to change based upon current trends for hosting prices).
- Once your class web page is set up, email the url to the instructor.
- Assignments 1 - HTML web page


### Reference
- Hosting
  + [Bluehost](http://www.bluehost.com/)
  + [GoDaddy](http://www.godaddy.com/)
  + [NameCheap](http://www.namecheap.com/)
  + [HostGator](http://www.hostgator.com/)
- [An Introduction to DNS Terminology, Components, and Concepts](https://www.digitalocean.com/community/tutorials/an-introduction-to-dns-terminology-components-and-concepts)
- [ Setting up FileZilla](https://my.bluehost.com/cgi/help/filezilla)
- Text Editors
  + [Atom](http://www.atom.io/)
    * [Atom Editor Cheat Sheet](http://d2wy8f7a9ursnm.cloudfront.net/atom-editor-cheat-sheet.pdf)
  + [Sublime Text](http://www.sublimetext.com/)
    * [Sublime Text 3 Cheat Sheet](http://www.cheatography.com/martinprins/cheat-sheets/sublime-text-3-osx/)
  + [Brackets](http://brackets.io/)
    * [Brackets Cheat Sheet](http://lisacatalano.github.io/brackets_course/)
