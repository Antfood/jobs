






## Get live-reaload running

check if npm and node ared installed:

      node -v
      npm -v

install brownser sync using npm. 

     npm install -g browser-sync

While in the directory of the project running the following command:

    browser-sync start --server --files "styles/*.css"

Visit `http://localhost:3000` to see that you are working on.  Everything you make changes to the project it will automatically update the browser.