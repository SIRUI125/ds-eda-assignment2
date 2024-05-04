# EDA Assignment - Distributed Systems.
Name: Sirui Yao

YouTube Demo link - https://youtu.be/7MoyTWw0GBA


## Phase 1
+ The Confirmation Mailer lambda is now a direct subscriber to this topic.
+ Send an email after uploading a picture.
  + Confirmation Mailer - Fully implemented.
  + Lambda function: confirmMailer.ts


+ Send rejection emails when file do not have the right format.
  + Rejection Mailer - Fully implemented.
  + Lambda function: rejectionMailer.ts

+ Extend the Process Image lambda to include writing an item to a DynamoDB table.
  + Process Image - Fully implemented.
  + Lambda function: processImage.ts

## Phase 2
+ In topic2, user can delete an object (image) from the bucket or add a description for an image using the AWS CLI.

+ Confirmation Mailer - Fully implemented.
+ Rejection Mailer - Fully implemented.
+ Process Image - Fully implemented.
+ Update Image - Fully implemented(Inculding the filter).
  + Lambda function: updateImage.ts
  + Only the 'Update Table' function should receive these messages.
+ Delete Image - Fully implemented(Inculding the filter).
  + Lambda function: deleteImage.ts
  + The 'Process Delete' function should receive only the delete image requests. 

## Phase 3 (if relevant)

+ All user-initiated events are now published to one SNS topic, all the subscribers use filter out those messages of interest to them using attribute or message body filtering techniques.

+ Confirmation Mailer - Fully implemented.
+ Process Image - Fully implemented.
+ Update Table - Fully implemented.
+ Delete Mailer - Fully implemented.
+ Lambda function: deleteMailer.ts

