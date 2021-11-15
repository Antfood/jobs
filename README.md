## get started

All the commands should be executed in the command line. 

Make sure you have git install

    git -v

Use brew in case git is not installed

    brew install git

Navigate to the folder you want to work locally. Clone this repo:

    git clone https://github.com/Antfood/jobs.git


## Get live-reaload running

check if npm and node ared installed:

      node -v
      npm -v

Again, use brew if you need to install node:

     brew install node

install brownser sync using npm. 

     npm install -g browser-sync

While in the directory of the project running the following command:

    browser-sync start --server --files "styles/*.css"

Visit `http://localhost:3000` to see that you are working on.  Everything you make changes to the project it will automatically update the browser.


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