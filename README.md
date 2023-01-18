# CPCB GSA website
This is the public webpage of the CMU-Pitt Computational Biology PhD Program's Graduate Student Association (CPCB GSA). 

### Updating the website (for organization members)
1. Clone this repository: `git clone git@github.com:cpcb-gsa/cpcb-gsa.github.io.git`
2. `cd cpcb-gsa.github.io/`
3. Ensure you have all of the [prerequisites](https://jekyllrb.com/docs/installation/#requirements) (make sure to follow the guide for your OS)
4. `gem install bundler`
5. `bundle install`

If you have issues installing some of the gems, try deactivating anaconda.

The [Jekyll](https://jekyllrb.com/) documentation is useful for setting up the environment and updating the webpage.

### Viewing the webpage locally
Assuming you have followed all of the steps above for properly updating the website, you can also host a local version to see changes as you make them by running:

`bundle exec jekyll serve`

(If using OSX, you may need to set the following environment variable first: `VAGRANT_DISABLE_RESOLV_REPLACE=1`)

Then go on your browser to [http://localhost:4000](http://localhost:4000).

Alternatively, if you would like to check the website on other devices (e.g. phone, tablet, etc.) on your local network you can run

`bundle exec jekyll s -H <your internal IP>`

Then go on your browser on any device on the same network to `http://<your internal IP>:4000`


