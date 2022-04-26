go mod init 00_hello
docker image build -t myhello .
docker container run -p 3000:8888 myhello
http://localhost:3000/
go mod init 00_hello
