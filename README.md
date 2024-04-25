# HandlePost
API Gateway: [Customers](https://us-west-1.console.aws.amazon.com/apigateway/main/apis/i9ry743iq0/resources?api=i9ry743iq0&region=us-west-1)

## Route: 
/customers/

## Input: 
JSON body containing the record data to be inserted.

## Output: 
Object representing the inserted record, identified by its ID.

## Function Mapping:
Lambda Function: 
[handleDelete](https://us-west-1.console.aws.amazon.com/lambda/home?region=us-west-1#/functions/handlePost?tab=code)

## Data Flow:
1. Client sends a POST request with JSON body to {root_url}/people.
2. Amazon API Gateway triggers the createPerson Lambda function.
3. Lambda function processes the request, inserts the record into the database, and retrieves the inserted record.
4. Lambda function returns the inserted record as the response.
5. Amazon API Gateway sends the response back to the client.
