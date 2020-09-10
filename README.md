# UCLAbookstack-AWS-delete-optimized-photo-copy

### This is a mini project made as an auxiliary function used for BookStack.
### This function detects when an image is deleted from the main S3 bucket used for storing user's images, and finds that same file in the optimized bucket we use to quickly render the images

### This allows us the simplicity of from the project, simply deleting the image from one bucket and having AWS handle the optimized version

## IMPORTANT
### When we import this function into the lambda functions offered by AWS, we want to zip up the files, not the outer shell directory. If we do not do this, AWS will throw an errorZip up the actual files not the directory
