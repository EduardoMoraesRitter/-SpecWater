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

* In the alpha stage of this project, a spectrometry study was made in order to understand the process of chemical analysis fluids that come into contact with water. As a result, we developed a prototype in Arduino to validate the hypothesis, even not knowing for certain if whether this solution would work or not.
* After the validation of the hypothesis we begined the Beta stage where, through the collected data, we elaborated a statistical analysis  to verify if the water in question would be contaminated or not. With the success we had, we created a MVP (minimum viable product) in order to be applied in the real world.


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

#### Spectrophotometry research:
It is a method used to measure how much a chemical substance absorbs light by measuring the intensity of when a beam of light passes through a sample, making it possible to measure the quantity of a known chemical substance

![spectrophotometer](/images/spectrophotometer.jpg)

Prototipo de arduino:

![Cooperation architecture diagram](/images/arduino_project.jpg)

#### Collection in the river:
The Tietê river, born in Salesópolis, in the Serra do Mar, crosses the state of São Paulo, bathing 62 municipalities. The river is at the top of the ranking of the most polluted rivers in Brazil, as it receives domestic and industrial sewage in the stretch of the capital where less than half of this sewage is treated. The analyzed sample was collected in the western region of the city, after the river had crossed the entire state capital on the border with the municipality of Osasco.

![coleta](/gifs/coleta.gif)

#### Creation of an Arduino collector for spectrophotometry testing:
Taken from the point where the water runs calmly with a strong sewage odor using a plastic container and transferred to the test body applying the method of analysis according to the variation of the light beam through the substance without decanting of organic material.

![amostra](/gifs/amostra.gif)

Data processing and Machine Learning model creation:

![Cooperation architecture diagram](/images/arduino_project.jpg)

Web site development so the local population can check water quality:

![website](/images/website.jpg)

## Resources

- [IBM Cloud](https://www.ibm.com/cloud)
- [Watson Studio](https://www.ibm.com/cloud/watson-studio)
- [Watson Machine Learning](https://www.ibm.com/br-pt/cloud/machine-learning)
- [Watson IoT Cloud](https://www.ibm.com/cloud/internet-of-things)

## Solution developed by
* [Eduardo Ritter](https://github.com/EduardoMoraesRitter), Senior Software Engineer
* [Joana Ritter](https://github.com/JoanaRitter), UX/UI Designer
* [Joel Pacheco](https://github.com/jpachecoaraujo), Chemist
* [Matheus Moraes](https://github.com/mtsvi-moraes), Data Scientist
* [Pedro Ivo](https://github.com/P-dro), IT Specialist

<p>
  <img src="https://contributors-img.web.app/image?repo=EduardoMoraesRitter/SpecWater" />
</p>

## License

This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details.
