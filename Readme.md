# Simple Animation done using React


## Available Scripts

In the project directory, you can run:

### `npm install`

### `npm start`

## In the workflow script:

* Whenever a new commit done to main branch the pipeline will start to work.
* The main branch will be checked out
* Node environment will be created
* Node dependencies for the react app will be installed using npm install command.
* Then npm run build command will build the react app into a static app by creating static files inside a folder called build.
* After that, the GitHub action workflow will logged into the AWS S3 bucket using the credentials provided in the secrets.
* Then, static files which is inside the build folder will be synced with our created bucket.
* You can able to view the GitHub Actions deployment process as soon as you commit to main branch.