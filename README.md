https://www.youtube.com/watch?v=AK6Rf_yjvI0&list=PLUjbZ3hCMnL-7j5Lof2q5S02KwMTeYRIE
at 50 min

# springboot-dynamodb-example
Build CRUD Application using SpringBoot + DynamoDB then Deploy CRUD application to Elastic Beanstalk 


---

## Dependency (Required)

```javascript
<dependency>
	<groupId>com.amazonaws</groupId>
	<artifactId>aws-java-sdk-dynamodb</artifactId>
	<version>1.11.815</version>
</dependency>
```



## Custom Policy

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action":   [ "dynamodb:PutItem" ],
      "Resource": [ "*" ]
    },
    {
      "Effect": "Allow",
      "Action":   [ "sns:Publish" ],
      "Resource": [ "*" ]
    }
  ]
}
```

## Request JSON

```json
{
	"name":"Santosh",
	"email":"santosh@gmail.com",
	"age":30,
	"address":{
		"city":"Bangalore",
		"state":"karnataka",
		"pinCode":"560037"
	}
}

```
