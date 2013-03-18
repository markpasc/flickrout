# flickrout #

`flickrout` is a command line tool for exporting a Flickr to local files.


## Installation ##

Install `flickrout` as any other Python program:

    $ python setup.py install

If you don't want to install its dependencies system-wide, try installing it in a [virtual environment](http://www.virtualenv.org/).


## Configuring ##

First, you'll need a Flickr API access token. Follow these steps to create an application with an API key:

1. Go to [the App Garden page of www.flickr.com](http://www.flickr.com/services/).
2. Click “Create an App”.
3. Click “Request an API Key” on the right.
4. Click “Apply for a non-commercial key”.
5. Enter “flickrout” for the name and “An application to back up my photos.” for the description. Check the boxes and click “SUBMIT”.
6. Click “Edit auth flow for this app”.
7. Change “App Type” to “Desktop Application” and click “Save Changes”.
8. In the “Admin” section on the right click “View the API Key for this app”.

Then, on the command line where you installed `flickrout`, run the `configure` command and enter your key. After entering the secret, your web browser will open to a Flickr API page. Approve the app, copy the verifier code, and paste it at the “Verifier:” prompt.

    $ flickrout configure
    API Key: 3sJE5btgFco5kh4HGR1b
    API Secret: TfuunBJjZNo3phB47p7an0n53M40e6eGq18821u

    Verifier: 102-400-321

    Configured!

Boom, solutionized.


## Usage ##

See `flickrout --help` for supported commands.

    $ flickrout -v verify
    INFO: Set log level to INFO
    INFO: Verified!

    $
