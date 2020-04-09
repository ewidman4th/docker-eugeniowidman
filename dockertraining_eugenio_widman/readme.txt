docker build -f "C:\Users\eugenio.widman\source\repos\dockertraining_eugenio_widman\dockertraining_eugenio_widman\Dockerfile" --force-rm -t s6assignmenteugeniowidman "C:\Users\eugenio.widman\source\repos\dockertraining_eugenio_widman"

docker run --name site1_eugeniowidman -p 8085:80 a93152f4db56

docker run --name site2_eugeniowidman -p 8086:80 -e AppSettings:Storename="Plano" a93152f4db56

docker tag s6assignmenteugeniowidman:latest dockertraining2020/dockertrainingeugeniowidman:latest

docker push dockertraining2020/dockertrainingeugeniowidman:latest