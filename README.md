# Methulan_Maniyam-dt1-23

root@LenovoMidhu:/mnt/c/DT-1#  cd /mnt/c/DT-1/dt1-23
root@LenovoMidhu:/mnt/c/DT-1/dt1-23# ls
Dockerfile  Pipfile  Pipfile.lock  README.md  main.py

root@LenovoMidhu:/mnt/c/DT-1/dt1-23# docker login
Authenticating with existing credentials...
Login Succeeded


![image](https://github.com/MidhuManiyam/Methulan_Maniyam-dt1-23/assets/145026551/2da540da-a936-4cf0-838b-7d49f4d1999d)

Dockerhub and push image:
![image](https://github.com/MidhuManiyam/Methulan_Maniyam-dt1-23/assets/145026551/15f56beb-c60c-459e-a889-2db6c1584685)

Hugging Face Account / Create API Key:
![image](https://github.com/MidhuManiyam/Methulan_Maniyam-dt1-23/assets/145026551/0a929fdb-6e2e-4419-a2d2-589690024745)

Login Google Cloud Platform Account: 
![image](https://github.com/MidhuManiyam/Methulan_Maniyam-dt1-23/assets/145026551/3f4621c7-ce80-4b46-96b9-ddb6bda70386)

Start a new VM: 
![image](https://github.com/MidhuManiyam/Methulan_Maniyam-dt1-23/assets/145026551/9b8f87c1-a5ea-4ca5-9c32-7cb8fbe6b92f)

SSH into VM, Install Docker
methulan_maniyam@instance-2:~$ sudo docker login
Login with your Docker ID to push and pull images from Docker Hub. If you don't have a Docker ID, head over to https://hub.docker.com to create one.
Username: midhumaniyam
Password: 
WARNING! Your password will be stored unencrypted in /root/.docker/config.json.
Configure a credential helper to remove this warning. See
https://docs.docker.com/engine/reference/commandline/login/#credentials-store

Login Succeeded


droot@LenovoMidhu:~# docker login
Authenticating with existing credentials...
Login Succeeded
root@LenovoMidhu:~# docker images
REPOSITORY                   TAG       IMAGE ID       CREATED       SIZE
midhumaniyam/img1            v1        812da8468a29   7 days ago    113MB


methulan_maniyam@vm-dt1:~$ docker ps
permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/v1.24/containers/json": dial unix /var/run/docker.sock: connect: permission denied
methulan_maniyam@vm-dt1:~$ sudo docker ps
methulan_maniyam@instance-1:~$ sudo docker ps
CONTAINER ID   IMAGE                  COMMAND            CREATED       STATUS       PORTS                                       NAMES
6399e2a48729   midhumaniyam/img1:v1   "python main.py"   2 hours ago   Up 2 hours   0.0.0.0:6000->5000/tcp, :::6000->5000/tcp   nervous_stonebraker

methulan_maniyam@instance-1:~$ curl "http://34.125.163.131:6000/chat?model_id=gpt2&huggingface_token=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&input=Life%20is"
{
  "ack": " a great way to get to know your friends and family.\n\nYou can also find"

Pull Docker Image from Docker Hub: 
docker pull midhumaniyam/img1:v1

Run the image: 
docker run -p 8000:5000 midhumaniyam/ img1:v1

Firewall System: 

![image](https://github.com/MidhuManiyam/Methulan_Maniyam-dt1-23/assets/145026551/afc6c78b-7bd3-47bc-887b-fa20d7dee01e)

Create frontend Bubble interface with the appropriate elements
![image](https://github.com/MidhuManiyam/Methulan_Maniyam-dt1-23/assets/145026551/749b515a-4f08-41a3-8faf-c44ea2e18cf6)

Javascript Code with Chatgpt
<script>
    document.getElementById("Button1").addEventListener("click", function() {
        // Get user input from the input field
        var userInput = document.getElementById("Input1").value;
        document.getElementById("Output1").innerText = "http://34.125.163.131:6000/chat?model_id=gpt2&huggingface_token=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&input=" + userInput;

        // Make a POST request to your Flask API
        fetch("http://34.125.163.131:8000/chat?model_id=gpt2&huggingface_token=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&input=" + userInput)
            .then(response => response.json())
            .then(data => {
                // Concatenate input and output, separated by a space
                var result = userInput + " " + data.ack;
                  // Display the result in the output element
                document.getElementById("Output1").innerText = result;
            })
            .catch(error => {
                console.error("Error:", error);
            });
    });
    </script>

Display API Responses to the user in Bubble
1.) ![image](https://github.com/MidhuManiyam/Methulan_Maniyam-dt1-23/assets/145026551/02114d35-e6b0-4bb0-ae56-6fd3ece794d5)
2.) ![image](https://github.com/MidhuManiyam/Methulan_Maniyam-dt1-23/assets/145026551/dde13a04-7c22-4c19-82a1-686dfdafe0a9)

Special Functions in Bubble: 
![image](https://github.com/MidhuManiyam/Methulan_Maniyam-dt1-23/assets/145026551/bda96af3-62cb-4e92-92b3-949f3e06d120)
![image](https://github.com/MidhuManiyam/Methulan_Maniyam-dt1-23/assets/145026551/66b2291f-2f0e-48fa-aa47-5e12d918166d)

Adding Josh and Sid to the GitHub Repository: 
![image](https://github.com/MidhuManiyam/Methulan_Maniyam-dt1-23/assets/145026551/e1777c48-e28e-409b-99db-3e6c7e50f0b8)














  

