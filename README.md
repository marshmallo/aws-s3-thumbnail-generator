# aws-s3-thumbnail-generator
Thumbnail generator using [Serverless Framework](https://serverless.com/).

## Instructions
1. Clone this repository

2. Edit the `serverless.yml` file and replace profile and region name with actual one.

3. The project requires deploying additional dependencies to be packaged along with the code to Lambda. For this, install [Serverless Python Requirements](https://www.serverless.com/plugins/serverless-python-requirements) plugin.
```
$ npm install --save serverless-python-requirements
```

4. The plugin will now bundle the python dependencies specified in `requirements.txt` or `Pipfile` when you run serverless deploy.

5. Deploy the function
```
$ serverless deploy -v
```

6. Invoke the Lambda function
```
$ serverless invoke --function s3_thumbnail_generator --log
```

## Additional Resources
Refer official Serverless Framework documentation [here](https://serverless.com/framework/docs/getting-started).
