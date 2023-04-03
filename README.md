![output5](https://user-images.githubusercontent.com/67295757/229635990-6b35533d-2278-4ecd-b8fb-77cfe0a06cf7.gif)

---

## Running local

Install http-server  
`npm install --global http-server`  
or  
`brew install http-server`

Generate certs with openssl:  
`openssl req -newkey rsa:2048 -new -nodes -x509 -days 3650 -keyout key.pem -out cert.pem`

Run http-server in the project directory with the cert  
`http-server -S -C cert.pem`

Go to https://localhost:8080
