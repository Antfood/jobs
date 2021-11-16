## get started

Pushing to github will enable us to collaborate.  Let's make sure you are able to do so using git.

**note:** All the commands should be executed in the command line. In vscode, you can open a terminal window with ``ctrl + ` ``.

Make sure you have git install

    git -v

Use brew in case git is not installed

    brew install git

Navigate to the folder you want to work locally. Clone this repo:

    git clone https://github.com/Antfood/jobs.git


## Get live reload running
 
 Live reload makes your life much easier when working with html and css. It will basically reload the page in the browser whenever you hit save in the document you are editing.

check if npm and node are installed:

      node -v
      npm -v

Again, use brew if you need to install node:

     brew install node

install brownser sync using npm. 

     npm install -g browser-sync

While in the directory of the project running the following command:

    browser-sync start --server --files "./*.html" "styles/*.css" "fonts/*"

Visit [http://localhost:3000](http://localhost:3000) to see that you are working on.  Everything you make changes to the project it will automatically update the browser.

Alternatively, I include a shell script so you don't need to type in this huge command to start the server. First you need to set the permissions for the script.

        chmod u+x start

And then run:

        ./start


## Pushing your work

Once your are done working run the following command to add your changes to git:

    git add -A

then:

    git commit -m "a short message with what you've done!"

push the code to github:

    git push origin main

## Unistall Browser sync

Browser sync is installed globally in your computer. If you wish to remove it after this project execute the below command:

    npm uninstall -g browser-sync
