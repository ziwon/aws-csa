### S3 has what consistency model for PUTS of new objects
- Read After Write Consistency

### What is AWS Storage Gateway?
- It's an on-premise virtual appliance that can be used to cache S3
  locally at a customers site.

### One of your users is trying to upload a 7.5GB file to S3 however they keep getting the following error message - "Your proposed upload exceeds the maximum allowed object size.". What is a possible solution for this?

- Design your application to use the multi-part upload API for all
  objects.

### What does RRS stand for when talking about S3?
- Reduced Redundancy Storage

### You have been asked by your company to create an S3 bucket with the name "acloudguru1234" in the EU West region. What would be the URL for this bucket?
- https://s3-eu-west-1.amazonaws.com/acloudguru1234

### What is Amazon Glacier?
- An AWS service designed for long term data archival.

### What does S3 stand for?
- Simple Storage Service

### You are a solutions architect who works with a large digital media company. The company has decided that they want to operate within the Japanese region and they need a bucket called "testbucket" set up immediately to test their web application on. You log in to the AWS console and try to create this bucket in the Japanese region however you are told that the bucket name is already taken. What should you do to resolve this?

- Bucketnames are global, not regional. This is a popular bucket name and is already taken. You should choose another bucket name.
Correct

### What is the availability on RRS?
- 99.99%

### What is the durability on RRS?
- 99.999999999%

### What is the minimum file size that I can store on S3?
- 1 Byte

### The difference between S3 and EBS is that EBS is object based where as S3 is block based.
- False

### S3 has eventual consistency for which HTTP Methods?
- overwrite PUTS and DELETES

### You work for a busy digital marketing company who currently store their data on premise. They are looking to migrate to AWS S3 and to store their data in buckets. Each bucket will be named after their individual customers, followed by a random series of letters and numbers. Once written to S3 the data is rarely changed, as it has already been sent to the end customer for them to use as they see fit. However on some occassions, customers may need certain files updated quickly, and this may be for work that has been done months or even years ago. You would need to be able to access this data immediately to make changes in that case, but you must also keep your storage costs extremely low. The data is not easily reproducible if lost. Which S3 storage class should you choose to minimise costs and to maximise retrieval times?

- S3 - IA

### You need to use an Object based storage solution to store your critical, non replaceable data in a cost effective way. This data will be frequently updat
Remove the ability for images to be served publicly to the site and then used signed URL's with expiry dates.ed and will need some form of version control enabled on it. Which S3 storage solution should you use?
- S3

### You work for a health insurance company who collects large amounts of documents regarding patients health records. This data will be used usually only once when assessing a customer and will then need to be securely stored for a period of 7 years. In some rare cases you may need to retrieve this data within 24 hours of a claim being lodged. Which storage solution would best suit this scenario? You need to keep your costs as low as possible.
- Glacier

### You run a meme creation website that frequently generates meme images. The original images are stored in S3 and the meta data about the memes are stored in DynamoDB. You need to store the memes themselves in a low cost storage solution. If an object is lost, you have created a Lambda function that will automatically recreate this meme using the original file in S3 and the metadata in Dynamodb. Which storage solution should you consider to store this non-critical, easily reproducible data on in the most cost effective solution as possible?
- S3 - RRS

### You run a popular photo sharing website that is based off S3. You generate revenue from your website via paid for adverts, however you have discovered that other websites are linking directly to the images on your site, and not to the HTML pages that serve the content. This means that people are not seeing your adverts and every time a request is made to S3 to serve an image it is costing your business money. How could you resolve this issue?
- Remove the ability for images to be served publicly to the site and then used signed URL's with expiry dates.
