# pdi-docker
A dockerfile for running a carte server for pentaho data integration version 9.0
# Usage
Just run on your console (you can change the exposed port on the config.xml file located at /configs)
```sh
docker run -p 8080:8080
```

## About The Project
A dockerfile for running a carte server for pentaho data integration version 9.0

### Built With
* Docker
* Bash

## Getting Started

### Prerequisites
* Docker
```sh
sudo apt get docker
```
### Installation

1. Clone the repo
  ```sh
  git clone https://github.com/brianamaral/pdi-docker.git
  ```
2. Edit the config.xml located at /configs as you like 
  ```xml
<slave_config>
    <slaveserver>
        <name>Master</name>
        <hostname>0.0.0.0</hostname>
        <port>8080</port>
        <username>cluster</username>
        <password>cluster</password>
        <master>Y</master>
    </slaveserver>
</slave_config>
  ```
 3. Build the Dockerfile
   ```sh
  docker build . -t "putnamehere"
  ```
## Usage
If you changed the variables above correctly, then you are good to go, just go run
```sh
docker run -dp 8080:8080 putnamehere
```

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


<!-- CONTACT -->
## Contact

Brian Bomfim Amaral - [Linkedin](https://www.linkedin.com/in/brian-amaral-29013a200/) - brian.amaralt@gmail.com

Project Link: [https://github.com/brianamaral/pdi-docker](https://github.com/brianamaral/pdi-docker)




