
 Setup for S3
  - click on services after login
  - click on storage
  - choose S3
  - click on create bucket
  - fill the bucket name
  - remove the trick on block all public access
  - add tags
  - click on create bucket
  - open aws-class-2-example
  - click on upload
  - upload the file
  - choose the file and click on upload
  - after the upload completed click on file
  - click on url of file
  - if it is showing access denied then
  - go to the properties 
  - go to the static website hosting
  - enable the hosting
  - file index.html
  - click on save changes
  - go to permissions
  - click on edit bucket policy
  - search s3 and choose in add actions
  - choose all actions(s3:*)
  - add resourses ( choose resourses type object and change resourse ARN bucketname- aws-class-2-example and object- * click on add resourses)
  - change the principle: "*" from object to.
  - click on save changes
  - click on again bucket policy and change action from "s3:*" to "s3:GetObject"  
  - after that click on file and go to url of file and now it accessible 
  - upload .html file and open it it is accessible and if .js file of .html file please upload also it.

# work with s3-cicd-project:

- create .github folder
- create workflows folder
- create s3-deploy-main.yml
- create github repository
- git init
- git commit 
- go to setting and setup secrets actions
- like AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY
- after go to the aws 
- create iam user
- got to the user and create new user
- click on Next: Permissions
- create group like developres and choose s3
- click on Next Tags (Name , website cicd)
- click on Preview
- click on create user
- after it update the access_key and secret_key on github from aws
- after it push on github


