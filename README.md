[![License](https://img.shields.io/badge/License-Apache2-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0) [![Community](https://img.shields.io/badge/Join-Community-blue.svg)](https://developer.ibm.com/callforcode/solutions/projects/get-started/)

# SpecWater - Call for Code

Bringing Artificial Intelligence to monitor water quality and save lives.

## Description:

<p>Over 1.8 billion people on Earth do not have access to adequate sanitation. Therefore, over 10 million people, on their majority kids, die every year due to the lack of safe water. This is a major problem that has been plaguing humanity, especially the poorest population, whose only source of drinking water are rivers that are polluted.</p>
<p>Nowadays, analyzing the water quality is not an easy task. It's necessary for researchers to travel to the region to collect samples and take them to the laboratory, bringing great costs and making it difficult to alert the population.</p>
<p>Taking that into account, we developed SpecWater, a solution that aims to facilitate this process and make the water quality available to all humanity, in its region and in real time.</p> 
<p>SpecWater uses Artificial Intelligence that analyzes the spectrum of light from the water sample collected by an IoT (a small equipment installed in rivers and lakes). After the analysis, the result will be made available on an easily accessible website, and triggering an alert via SMS to the population who will be able to check the quality of the water and whether it is contaminated or not, in addition to receiving instructions for another form of consumption of drinking water.</p>
<p>The responsible authorities will also be immediately alerted to take action and provide further assistance to the local population.</p>

## Contents

1. [Description](#Description)
2. [RoadMap](#RoadMap)
3. [Architecture](#Architecture)
5. [Development](#Development)
6. [Resources](#Resources)
7. [Solution developed by](#Solution-developed-by)
8. [License](#license)

## RoadMap

* Fase alfa foi desenvolvido em maio e junho, os não tinhamos ideai ainda que o projeto era possivel, entao desenvolvemos de forma rudimentar para teste uma hipotese;
* Fase beta dado o sucesso que tivemos com aplicação evoluimos o projeto de maneira que pode ser aplicado em mundo real e criamos um MVP minimo produto viavel;

![RoadMap](/images/roudmap.jpg)

## Architecture

1. Initial phase: Water collection through IoT where it can be placed in several rivers
1. Data transmission through MQTT protocol to Watson IoT platform;
1. The data management proccess for analysis and orquestration of steps;
1. Sent to Watson Studio where the data is treated and sent to Watson ML Engine;
1. The machine learning model is implemented and it is responsible to classify the quality of water;
1. After the data is classified, it is sent to a database;
1. The API consumes the data and makes it available for comsumption;
1. The website gathers the information and puts it on a map;
1. The local population can access the website and check the quality of the consumed water in real time

![Cooperation architecture](/images/architecture.jpg)


## Development

Creation of an Arduino collector for spectrophotometry testing:
![Cooperation architecture diagram](/images/arduino_project.jpg)

Water collection from a river:
<p align="center">
  <src="/gifs/agua.gif">
</p>
![Cooperation architecture diagram](/images/arduino_project.jpg)

Safe and contaminated water sample data analysis:
![Cooperation architecture diagram](/images/arduino_project.jpg)

Data processing and Machine Learning model creation:
![Cooperation architecture diagram](/images/arduino_project.jpg)

Web site development so the local population can check water quality:
![Cooperation architecture diagram](/images/arduino_project.jpg)

## Resources

- [IBM Cloud](https://www.ibm.com/cloud)
- [Watson Studio](https://www.ibm.com/cloud/watson-studio)
- [Watson Machine Learning](https://www.ibm.com/br-pt/cloud/machine-learning)
- [Watson IoT Cloud](https://www.ibm.com/cloud/internet-of-things)

## Solution developed by
* [Eduardo Ritter](https://github.com/EduardoMoraesRitter), Senior Software Engineer
* [Joana Ritter](https://github.com/JoanaRitter), UX/UI Designer
- Joel Pacheco
* [Matheus Moraes](https://github.com/mtsvi-moraes), Data Scientist
- Pedro Ivo

<p>
  <img src="https://contributors-img.web.app/image?repo=EduardoMoraesRitter/SpecWater" />
</p>

## License

This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details.
