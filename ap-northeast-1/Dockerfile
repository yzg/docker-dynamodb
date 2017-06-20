
FROM openjdk:jre

RUN apt-get update

RUN wget https://s3-ap-northeast-1.amazonaws.com/dynamodb-local-tokyo/dynamodb_local_latest.tar.gz
RUN tar zxvf dynamodb_local_latest.tar.gz

EXPOSE 8000

CMD java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
