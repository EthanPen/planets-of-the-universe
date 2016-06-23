# planets-of-the-universe

Tags: Jekyll

---

**The Planets of the universe:** [https://ethanpen.github.io/planets-of-the-universe/](https://ethanpen.github.io/planets-of-the-universe/)

**The Jekyll tutorial:** [https://www.youtube.com/playlist?list=PLWjCJDeWfDdfVEcLGAfdJn_HXyM4Y7_k-](https://www.youtube.com/playlist?list=PLWjCJDeWfDdfVEcLGAfdJn_HXyM4Y7_k-)


#### Why use Jekyll?

The main reasons for using Jekyll are efficiency, it eliminates lots of copying and pasting in our websites amoung other things:

* Makes use of ☛ Markdown to reduce the overhead of HTML,
* Allows sharing of HTML code between pages,
* Has the ability to automatically write repeated HTML,
* Can be hosted on GitHub using GitHub pages.

jekyll isn’t the only way to get these features, you could use other static site generators or even other languages like PHP, Python, or Ruby.

#### The _site folder

When Jekyll is running and you save one of your files it will be copied to the _site folder. The _site folder is completely temporary, but is also the final, compiled version of your website.

If you delete the _site folder, when you save a file again it will immediately come back.


####Never have the _site folder on GitHub

Since the _site folder is temporary it should never be committed to GitHub.

Git has a method for ignoring files, so that they can never be accidentally committed.

If you create a new file named .gitignore, in the same location as your index.html Git will look here for what files and folders to hide.

Inside the .gitignore file you can write the folder you want to hide, like this:

	_site
	
Commit it into your repository and Git will safely ignore the _site folder from now on.

####Layouts

Jekyll has a feature named layouts that allows designers to put the header and footer in a single file and have them shared between every page on the site—kind of like master pages in InDesign.

This is probably one of the most compelling reasons to use Jekyll.

First open you index.html file and look for stuff that will be common to every page, like headers, footers, DOCTYPE, etc.

Cut that stuff and put it into a new file: default.html. It doesn’t have to be called “default”, that’s just a convention.

Save this file into a folder named _layouts.

	_config.yml
	_layouts/        ⬅︎ The layouts folder
	  └ default.html
	index.html
	
#### local host
If you’re using GitHub as a host then your project is within a folder, when looking at it live on GitHub’s URL. But on your local computer there is no folder.

On your local computer, the URL might look like this:

	http://127.0.0.1:4000/about/
But on GitHub, it will look like this:

http://dinos.github.io/meat-eaters/about/


