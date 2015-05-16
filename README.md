# docker-webshot
[Docker](https://github.com/docker/docker) Image for [Webshot-cli](https://github.com/valeriangalliat/webshot-cli), a simple command to take local or remote webpage screenshots.

[Webshot](https://github.com/brenden/node-webshot) is a wrapper around the Webshot library, providing a simple command to take local or remote webpage screenshots. This module is a light wrapper around [PhantomJS](https://github.com/ariya/phantomjs), which utilizes [WebKit](https://github.com/WebKit/webkit) to perform the page rendering.

The container provides webshot-cli module with [IOjs](https://github.com/nodejs/docker-iojs)

Example

    docker run -v $HOME:/usr/src/app smtx/docker-webshot webshot example.html example.png 

    docker run -v $HOME:/usr/src/app smtx/docker-webshot webshot --shot-size all/all 'https://www.slashdot.org/' slashdot.png
