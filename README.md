# navigator-buildpack
The heroku buildpack for the navigator application

navigator buildpack to run the necessary installation of the navigator application the heroku infrastructure.  

## Setup

1. Set Heroku's default Python buildpack for your app, set up Python and install the required python dependencies.

    ```bash
    heroku buildpacks:set https://github.com/heroku/heroku-buildpack-python
    ```

2. Set Heroku's default NodeJS buildpack for your app, set up NodeJS. 

    ```bash
    heroku buildpacks:add https://github.com/heroku/heroku-buildpack-nodejs
    ```

3. Add this buildpack, build the static assets used by the system.

    ```bash
    heroku buildpacks:add https://github.com/uktrade/help-buildpack.git
    ```
