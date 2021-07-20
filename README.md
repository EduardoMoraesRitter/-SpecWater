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

1. Etapa de coleta a água através do IoT onde pode ser colocado em diversos rio.
1. Transmissão dos dados através de protocolo MQTT para a plataforma do watson iot plataforma;
1. O gerenciamento dos processo dos dados para análises e orquestração das etapas;
1. Enviado para o watson studio onde são os dados são tratados e envia pra watson ml engine;
1. O modelo de machine learning está implementado e responsável para classificar a qualidade da água;
1. Depois que os foram classificados são enviadas para um banco de dados;
1. A api consome os dados e deixa disponível para consumo;
1. O website consome as informações e colocas as informações em um mapa;
1. A população pode acessar o site verificaram a qualidade da água que consome em tempo real;

![Cooperation architecture](/images/architecture.jpg)


## Development

Criação de uma coletor feito em arduino para teste de um espectrofotometria:
![Cooperation architecture diagram](/images/arduino_project.jpg)

Coleta de agua de uma Rio:
![Cooperation architecture diagram](/images/arduino_project.jpg)

Analise de dados, de amostra de agua potavel e agua contaminada:
![Cooperation architecture diagram](/images/arduino_project.jpg)

Tratamento dos dados e criação de um modelo de machine learning:
![Cooperation architecture diagram](/images/arduino_project.jpg)

Desenvolvimento do web site para acesso da população a qualidade da agua:
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
* [Matheus Moraes](https://github.com/mtsvi-moraes), Data Science
- Pedro Ivo

<p>
  <img src="https://contributors-img.web.app/image?repo=EduardoMoraesRitter/SpecWater" />
</p>

## License

This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details.
