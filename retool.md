### DynamoDB Integration
__Querying Amazon DynamoDB with Retool.__

DynamoDB is Amazon's non-relational managed database. Retool connects with DynamoDB, allowing you to access your data from your internal tools.

__Connecting DynamoDB :__
 - First, go to [IAM](https://signin.aws.amazon.com/signin?redirect_uri=https%3A%2F%2Fconsole.aws.amazon.com%2Fiam%2Fhome%3Fstate%3DhashArgs%2523%26isauthcode%3Dtrue&client_id=arn%3Aaws%3Aiam%3A%3A015428540659%3Auser%2Fiam&forceMobileApp=0&code_challenge=XbOR5Sn6hJFefVi3hSPYRlGcw7IwZPErAUqno4FVYO0&code_challenge_method=SHA-256) and create a new aws account and create a user called retool-dynamodb. Only enable "programmatic access".


<figure>
  <img
  src="/newuser.png"
  alt="New User.">
  <center><figcaption>Fig 1. New User</figcaption></center>
</figure>


- Click next to Configuration screen for DynamoDB as shown in the below figure 
- AWS secret key will be provided by the tech support.

<figure>
  <img
  src="/resource.JPG"
  alt="Resource.">
  <center><figcaption>Fig 2. Configuration screen for DynamoDB</figcaption></center>
</figure>

<br>
### CURD operations :

__Reading the data :__
- To read the data go to Home page, click on your page (on boarding) and edit.
- Go to new and click on resource query and select the resource, table name and method (Scan) and hit run.

<figure>
  <img
  src="/run.JPG"
  alt="Read.">
  <center><figcaption>Fig 3. Read Query </figcaption></center>
</figure>
  
__Displaying the data in a table :__

- In onboarding page, drag and drop the table from insert tab to canvas.
- Go to inspect and in Data field enter the below format  `{{query.data.Items}}` ( Query is the name of the query created in the previous step)
  
<figure>
  <img
  src="/Display.JPG"
  alt="Read.">
  <center><figcaption>Fig 3. Read Query </figcaption></center>
</figure>
  