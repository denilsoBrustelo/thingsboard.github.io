<<<<<<< HEAD
<<<<<<< HEAD
## Instructions for Contributing to the Docs/Website

* [Fork this repository](https://help.github.com/articles/fork-a-repo/)
* [Deploy the site locally](#deployment-of-the-site-locally)
* Add your changes
* [Create Pull Request](https://help.github.com/articles/creating-a-pull-request/)

## Deployment of the site locally

The below commands setup your environment for running GitHub pages locally. 
Any edits you make will be viewable on a lightweight webserver that runs on your local machine.

Install Ruby 2.2 or higher. If you're on Linux, run these commands:

    sudo apt-get install software-properties-common
    sudo apt-add-repository ppa:brightbox/ruby-ng
    sudo apt-get update
    sudo apt-get install ruby2.2
    sudo apt-get install ruby2.2-dev

* If you're on a Mac, follow [these instructions](https://gorails.com/setup/osx/).
* If you're on a Windows machine you can use the [Ruby Installer](http://rubyinstaller.org/downloads/). During the installation make sure to check the option for *Add Ruby executables to your PATH*.

Install the GitHub Pages package, which includes Jekyll:

	gem install github-pages

Clone our site:

	git clone https://github.com/thingsboard/thingsboard.github.io.git

Make any changes you want. Then, to see your changes locally:

	cd thingsboard.github.io
	bundle exec jekyll serve

Your copy of the site will then be viewable at: [http://localhost:4000](http://localhost:4000)
(or wherever Jekyll tells you).
=======
# Thingsboard IoT Gateway
[![Join the chat at https://gitter.im/thingsboard/chat](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/thingsboard/chat?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
=======
# ThingsBoard IoT Gateway
The Thingsboard **IoT Gateway** is an open-source solution that allows you to integrate devices connected to legacy and third-party systems with Thingsboard.  
>>>>>>> 51e1695654275fefe4c54a6e1567ede9925e2c2b

Thingsboard is an open-source IoT platform for data collection, processing, visualization, and device management. See [**What is Thingsboard?**](https://thingsboard.io/docs/getting-started-guides/what-is-thingsboard/) if you are new platform user.  

[**What is ThingsBoard IoT Gateway?**](https://thingsboard.io/docs/iot-gateway/what-is-iot-gateway/)  

![ThingsBoard IoT Gateway architecture](http://thingsboard.io/images/gateway/python-gateway.png)

### Gateway features

Thingsboard IoT Gateway provides following features:  

 - **OPC-UA** connector to collect data from devices that are connected to OPC-UA servers.
 - **MQTT** connector to collect data that is published to external MQTT brokers. 
 - **Modbus** connector to collect data from Modbus servers and slaves.
 - **BLE** connector to collect data from BLE devices.
 - **Request** connector to collect data from HTTP API.
 - **Custom** connector to collect data from custom protocols.
 - **Persistence** of collected data to guarantee data delivery in case of network and hardware failures.
 - **Automatic reconnect** to Thingsboard cluster.
 - Simple yet powerful **mapping** of incoming data and messages **to unified format**.
  
### Architecture  

The IoT Gateway is built on top of **Python**, however is different from similar projects that leverage OSGi technology.
The idea is distantly similar to microservices architecture.  
The gateway supports custom connectors to connect to new devices or servers and custom converters for processing data from devices.  
Especially, when we are talking about language APIs and existing libraries to work with serial ports, GPIOs, I2C, and new modules and sensors that are released every day.  

The Gateway provides simple integration APIs, and encapsulates common Thingsboard related tasks: device provisioning, local data persistence and delivery, message converters and other.  
For processing data from devices you also can write custom converter, it will receive information from device and send it to converter to convert to unified format before sending it to the ThingsBoard cluster.  

## Support

 - [Community chat](https://gitter.im/thingsboard/chat)
 - [Q&A forum](https://groups.google.com/forum/#!forum/thingsboard)
 - [Stackoverflow](http://stackoverflow.com/questions/tagged/thingsboard)

## Licenses

This project is released under [Apache 2.0 License](./LICENSE).
>>>>>>> upstream/master
