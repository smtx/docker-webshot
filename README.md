# docker-webshot
Webshot is a simple command to take local or remote webpage screenshots.

Webshot is a wrapper around the Webshot library, providing a simple command to take local or remote webpage screenshots. The module is a light wrapper around PhantomJS, which utilizes WebKit to perform the page rendering.

Example

    docker run -v $HOME:/usr/src/app smtx/webshot webshot example.html example.png 

    docker run -v $HOME:/usr/src/app smtx/webshot webshot –shot-size all/all 
    'https://www.slashdot.org/' slashdot.png
