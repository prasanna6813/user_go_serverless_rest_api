# user_go_serverless_rest_api
API Gateway + Lambda + DynamoDB Comlpete serveless stack

cmds

go mod tidy

GOARCH=arm64 GOOS=linux go build -tags lambda.norpc -ldflags="-s -w" -o bootstrap main.go && zip -jrm bootstrap.zip bootstrap