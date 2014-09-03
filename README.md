# OpenTok CodeIgniter 2 Sample

This repository is just a proof of concept for using OpenTok with CodeIgniter 2

## Set up

1. Copy the file `application/config/opentok.php.default` to `application/config/opentok.php` and
   edit the file to include your own API Key and API Secret.
1. Run `composer install` to install the required dependencies.
1. Set your webserver (such as Apache or nginx) to serve the project directory.

## Usage

Once you have the project set up, visit the `/index.php/welcome/opentok` path for the application.
It will print out a new Session ID and Token, which were generated on the server and can be used 
to connect.

**Note**: This example intentionally leaves out setting up a database to store Session IDs and
loading the JavaScript library to connect to the Session. Its just a simple proof of concept that
the OpenTok PHP SDK is in fact compatible with CodeIgniter 2.

## Ideas

If you'd like to further develop this example, feel free to fork and send a Pull Request. You could
start by adding a database, storing the generated sessions and allowing users to actually connect,
publish, and subscribe to those sessions. CodeIgniter also provides a Library architecture, so it would
be interesting to explore how the OpenTok PHP SDK could be encapsulated as a Library.
