
# Open Actuarial Textbooks Project Goal

The goal is to have the actuarial community author our textbooks in a collaborative fashion. The text *Loss Data Analytics* represents our first book. 

## Life Contingencies: The Mathematics, Statistics, and Economics of Life Insurance

This respository is focused on a new text, currently titled *Life Contingencies: The Mathematics, Statistics, and Economics of Life Insurance*. A summary of the book is available [online](https://openacttextdev.github.io/LifeCon/index.html), code for the book is available above. 


### DOWNLOAD AND EDIT A LOCAL COPY OF THE BOOK

1.  Optional - Get reasonably recent versions of R and Rstudio. Sometimes, there can be conflicts if you are running very old versions these products. (Probably best to do this step at a later stage in case you run into problems that you can't debug.)
2.  Optional - Update packages. We have discovered conflicts between some of the advanced graphics/RGL and javascript in chapter 3 with old versions of some packages. Surprisingly, the one exception is the package bookdown. We found that an old version (0.21) works best. So, use this code:
    *  require(devtools)
    *  install_version("bookdown", version = "0.21", repos = "http://cran.us.r-project.org")
3.  Download a copy of the book. Go to Github, https://github.com/OpenActTextDev/LifeCon, hit the green "Code" button, download a .zip file and uncompress it.
4.  Open R-studio, go to "File==>Open Project". From the folder you just downloaded and uncompressed, select "LifeCon.Rproj".
5.  In R studio, open the file "PackagesLifeCon.Rmd" (but do not knit it). These are the packages that will be called when you compile the book, so install them now if needed.
6.  In R-studio, go to the upper right tab, hit "Build". This brings up a "Build Book" tab. Click the down arrow to the right and select "bookdown::gitbook". This starts the compile process.
7.  Upon successful compile, you should see a preview of the book. If it gets lost, go to the "docs" subfolder and open "index.html" in a browser, hopefully you see the compiled book.
8.  As you edit the book, go to the file "_bookdown.yml". This allows you to select the .Rmd files (and the order) that you wish to appear in the book.

### UPLOAD YOUR BOOK VERSION TO GITHUB

1a.  Start by getting a (free) Github account.
1b.  Install Git on your local machine (https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).
1c.  Get a personal access token that you will need when you communicate between Rstudio and Github. (https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token)
2.  We are going to follow the process documented at https://happygitwithr.com/existing-github-first.html, so you might want to look over this excellent resource before beginning.
3.  16.1 Make a repo on GitHub
    *  Go to https://github.com and make sure you are logged in.
    *  Click the green “New repository” button. Or, if you are on your own profile page, click on “Repositories”, then click the green “New” button.
    *  Pick a repository name that actually reminds you what the project is about! But try to be concise.
    *  Public = YES Initialize this repository with a README
    *  Click the big green button “Create repository.”
    *  Copy the HTTPS clone URL to your clipboard via the green “Clone or Download” button. 
4.  In R-studio, open a new project. 
    *  "File==>New Project==>Version Control==>Git". In the “repository URL” paste the URL of your new GitHub repository. It will be something like this https://github.com/jennybc/myrepo.git.
5.  Close R studio and copy the existing project onto the one you just created.
6.  Open R studio with the newly created project. I have had a little trouble getting the first commit done on my machine. So, I have to do it by hand:
    *  Tools==>Shell
    *  git status
    *  rm -f .git/index.lock
    *  git add . --all
(The rm command is from:
https://stackoverflow.com/questions/38004148/another-git-process-seems-to-be-running-in-this-repository)
7.  Now, we can leave the shell
    *  Git tab ==> Commit ==>Provide a short descriptive name
    *  Then hit the push (up arrow)
Hopefully everything goes up to Github.
8.  Finally to get the world to see your page:
    *  Settings ==> GitHub pages ==>Check it out here! ==> 
    *  Source Change "None" to "main". Change "/root" to "/docs" . Then save.

May need to wait a couple minutes. Then, you can view your new book at, for example, https://ewfreesres.github.io/TestActMatch/



## Loss Data Analytics

### Book Description

*Loss Data Analytics* is be an interactive, online, freely available text.

* The online version contains many interactive objects (quizzes, computer demonstrations, interactive graphs, video, and the like) to promote deeper learning.
* A subset of the book is available for offline reading in pdf and EPUB formats.
* The online text will be available in multiple languages to promote access to a worldwide audience.

To see our progress, a current version of the book is available at [Online Version](https://OpenActTexts.github.io/Loss-Data-Analytics/index.html)

## Github Resources

*GitHub* provides a natural development environment to achieve this goal.

*  The more stable version is available through the ["Production" Github Landing Site](https://OpenActTexts.github.io) - designed for students and classes. 
*  The more frequently updated  version is available through the first ["Development" Github Landing Site](https://ewfrees.github.io) - designed for instructors and developers.
*  We are now porting resources to a newer, second ["Development" Github](https://github.com/OpenActTextDev/LifeCon) center - designed for instructors and developers.

Code, data, offline versions and more are available through these portals.

## Other Resources

See the [Open Actuarial Textbooks Project Site](https://sites.google.com/a/wisc.edu/loss-data-analytics/) for more information about this project.

