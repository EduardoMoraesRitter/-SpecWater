[![License](https://img.shields.io/badge/License-Apache2-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0) [![Community](https://img.shields.io/badge/Join-Community-blue.svg)](https://developer.ibm.com/callforcode/solutions/projects/get-started/)

# SpecWater - Call for Code

Bringing Artificial Intelligence to monitor water quality and save lives.

## Description:

<p>Over 1.8 billion people on Earth do not have access to adequate sanitation. Therefore, over 10 million people, with the majority being children, die every year due to the lack of safe drinking water. This is a major problem plaguing humanity, targeting the poorest populations, whose only source of drinking water are rivers that can become polluted unbeknownst to the people who rely on them.

Today, while scientific advancements are made daily, analyzing water quality is not a simple task. Researchers must travel to the region and collect individual samples. After which, the samples must then be  transported to a qualified laboratory where testing can be performed. Each of these crucial steps increase the time and monetary value spent on the expedition making it more difficult to receive funding and consequently alert the population.
Taking all of this into account, we developed SpecWater, a solution that aims to facilitate this process and improve access to safer water sources in all regions and in real time, for all humanity.

SpecWater uses Artificial Intelligence that analyzes the spectrum of light within a water sample collected by an IoT (a small equipment installed in rivers and lakes). After the analysis, results will be made available on an easily accessible website. Expanded functions such as the ability to trigger an alert via SMS, will also available. When a water quality alert is sent, it will allow the population to be able to check the quality of the community source and view whether it has been contaminated, or if it’s safe to consume. Instructions regarding a separate source of drinking water will be provided if the community source tests confirm contamination thus, avoiding infant mortality, the human immunodeficiency virus, which is often found in contaminated water and several other serious health and nutrition problems. The responsible authorities will also be immediately alerted to take action and provide further assistance to the local population.</p>

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

### Spectrophotometry research:
It is a method used to measure how much a chemical substance absorbs light by measuring the intensity of when a beam of light passes through a sample, making it possible to measure the quantity of a known chemical substance

![spectrophotometer](/images/spectrophotometer.jpg)

### Arduino prototype:
We developed a spectrophotometry  prototype in Arduino which when installed in rivers, streams, wells, springs and treatment plants collects the water data and process them through cloud.

![Cooperation architecture diagram](/images/arduino_project.jpg)

### Collection in the river:
The Tietê river, born in Salesópolis, in the Serra do Mar, crosses the state of São Paulo, bathing 62 municipalities. The river is at the top of the ranking of the most polluted rivers in Brazil, as it receives domestic and industrial sewage in the stretch of the capital where less than half of this sewage is treated. The analyzed sample was collected in the western region of the city, after the river had crossed the entire state capital on the border with the municipality of Osasco.

![coleta](/gifs/coleta.gif)

### Creation of an Arduino collector for spectrophotometry testing:
Taken from the point where the water runs calmly with a strong sewage odor using a plastic container and transferred to the test body applying the method of analysis according to the variation of the light beam through the substance without decanting of organic material.

![arduino](/gifs/arduino.gif)

### Data analysis
With data collected from a sample of safe water and a sample of water  from the most polluted river in Brazil we carried out a comparison and proved the efficiency of the applied method and proved that the project is functionally applicable:

![data](/images/data_collect.jpg)

### Model algorithms, Auto AI 
We used a cognitive system applied in Watson Studio together with Watson ML to test different algorithms and compare the efficiency of the models, streamlining the analysis process between the collected samples, and in the future analyzing any changes or anomalies that will be noticed in the rivers.:

![AutoAI](/gifs/IBM_Watson_IA.gif)

### Web site 
Web site development so the local population can check water quality:

![website](/gifs/website.gif)


#### Thus creating a complete monitoring system through which we can observe changes in the physical, chemical and biological characteristics of water


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
