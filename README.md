# docker-webshot
Webshot is a simple command to take local or remote webpage screenshots.

[Webshot](https://github.com/brenden/node-webshot) is a wrapper around the Webshot library, providing a simple command to take local or remote webpage screenshots. The module is a light wrapper around PhantomJS, which utilizes WebKit to perform the page rendering.

The container provides webshot-cli module with [IOjs](https://github.com/nodejs/docker-iojs)

Example

    docker run -v $HOME:/usr/src/app smtx/webshot webshot example.html example.png 

    docker run -v $HOME:/usr/src/app smtx/webshot webshot –shot-size all/all 
    'https://www.slashdot.org/' slashdot.png
