# Bookmarks 2 PDFs

Why? Because other offerings have ridiculous Ads, pay-walls, slow, error-prone,
etc.

Because the internet costs money to run, and unfortunately, private researchers
can't always afford to keep their research online. In that case, all the care
we've taken currating decades of knowledge is at the mercy of time. Thankfully,
great services like Microsoft GitHub and Archive.org exist. Now it is only a 
matter of exposing the greatness in a helpful way.

Drop a bookmarks.html file and check back anywhere between minutes and days 
later for a package of every piece of data you've left lingering out in the wild.

## Technical

bookmarks.html or history.db is encrypted by a public key stored on Github. The private key, encrypted and transfered to a virtual machine by a session key provided by the client.
The contents of your personal browsing history are uploaded encrypted to 
and inaccessible to an isolated server. 
With your permission, the session decryption key is transferred to the private cloud server. That server in the cloud visits each page in the bookmarks
file, and generates a PDF, an image screenshot, and some various metrics we think
you'll enjoy.

The resulting pages are then re-encrypted and stored awaiting download by you.

Alternatively, you can leave a browser tab open and use a plugin to run the PDF
generation automatically in a web-worker on your local system.

ALSO INCLUDES: build.yml Puppetteer test flow in GitHub Actions 
(in-case other devs want to grab that?)

TODO: delete old data

## Short term todo

* wkhtml2pdf in WASM, or Canvas page render? or both?
* Github build.yml with selenium. Interesting, can 
Github Actions pull any Docker? this might be really easy 
given prior work in dark-arts.
* XVNC/Puppetteer in a web-worker? this is getting weird.
* Code-golf like https://www.frontendmentor.io/, easy to use, obvious.




<sup><sub>powered by [rhood](https://github.com/briancullinan/rhood)</sub></sup>