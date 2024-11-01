# **JDUber - InfinityTech**🚜

<p align="center">
<img src="scr/assets/Infinity-Apresentação.png" alt="InfinityTech">
</p>

### Autores 👥
- Agatha Cassari Benedicto
- Arthur Gouvea
- Felipe Chiozzotto Gozzani 
- `Juliana Barbosa Sandes` 
- Raissa Yukari Senoi

## Introdução 📃

* **Principal problema:** <br>
  O principal problema da John Deere é a dificuldade na localização e monitoramento eficiente dos rebocadores e carrinhos, impactando negativamente o fluxo de trabalho e a        produtividade. A falta de um sistema que identifique se os carrinhos estão vazios ou carregados gera atrasos na logística interna e desperdício de tempo. Isso resulta em        custos operacionais elevados e gargalos na movimentação de materiais, comprometendo a eficiência geral das operações.
 
* **Objetivos:** <br>
  Nosso objetivo é facilitar a localização e utilização dos carrinhos, reduzindo o tempo gasto pelos usuários. Vamos desenvolver um sistema integrado com sensores e               microcontroladores Arduino para monitorar continuamente o estado dos carrinhos. Isso permitirá que os operadores saibam imediatamente quando um carrinho está vazio,         
  aumentando a eficiência operacional e a produtividade geral. O sistema aprimorado garantirá uma resposta mais ágil e coordenada nas operações.

<p align="center">
<img src="scr/assets/JB-img.png" alt="JohnDeere">
</p>

## Desenvolvimento 💻
- Estamos utilizando o Node-RED para o site e o programa que gerencia o sensor de peso e a localização dos carrinhos. A WiFi.h conecta o ESP32 ao Wi-Fi e escaneia redes, enquanto a PubSubClient.h envia dados ao broker MQTT (Mosquitto). A HX711.h configura a balança e a ArduinoJson.h converte os dados para JSON, compatível com o Node-RED. Essas bibliotecas garantem uma integração eficiente entre hardware e software.
  
<p align="center">
<img src="scr/assets/Diagrama.png" alt="Diagrama">
</p>

### Solução IoT do ESP32 🌐

<p align="center">
<img src="scr/assets/NodeRed.png" alt="Node-red">
</p>

## Resultados ✅
- Estamos desenvolvendo um site para facilitar a visualização dos carrinhos de forma eficiente. Implementamos um programa que utiliza um sensor de peso para indicar se a balança está vazia ou ocupada. Além disso, o site também exibe a localização dos carrinhos, utilizando a conectividade Wi-Fi para determinar a posição exata de cada um. Dessa forma, conseguimos monitorar tanto o estado de carga quanto a localização em tempo real, proporcionando uma melhor gestão e controle dos carrinhos no ambiente.

<p align="center">
<img src="scr/assets/Hardware.jpeg" alt="Hardware">
</p>

<p align="center">
<img src="scr/assets/Site.png" alt="Site">
</p>

## Testes de Desempenho 📈

### Teste de Precisão de localização 📍

**a-) Definição da Ferramenta de Teste:** Nessa seção o grupo deve descrever o que ela faz e como faz; <br>
- O ESP32 faz uma leitura de todas as redes wifis disponíveis próximas, pega as 3 mais fortes/mais perto e compara com o que seria a localização divididas em 3 roteadores, exemplo:
  
<p align="center"><br>
1 local : redes A,B e C<br>
2 local: redes B,C e D
</p>
<br>

**b-) Evidências de Testes:** Nessa seção precisa evidenciar o está sendo realizado, como prints da sua tela demonstrando os resultados; <br>

<p align="center">
<img src="scr/assets/Teste1.jpeg" alt="Teste1">
</p>

**c-) Discussão dos Resultados:** Nessa seção o grupo deve descrever se o teste foi satisfatório ou não;<br>
- Não foi satisfatório, a leitura das redes ficou muito volátil, o que causa confusão na hora de comparar com os locais.

**d-) Soluções Futuras:** Nessa seção, o que grupo faria para melhorar seus testes (não precisa implementar essas propostas de melhorias).<br>
- Uma possibilidade seria a instalação de uma antena para melhorar a precisão da leitura
  
<br>

### Teste de Capacidade Multidispositivo Simultâneos ⚡

**a-) Definição da Ferramenta de Teste:** Nessa seção o grupo deve descrever o que ela faz e como faz; <br>
- Utilizamos 2 baterias para energizar tanto o ESP32 quanto o sensor HX711.

**b-) Evidências de Testes:** Nessa seção precisa evidenciar o está sendo realizado, como prints da sua tela demonstrando os resultados; <br>

<p align="center">
<img src="scr/assets/Teste2.jpeg" alt="Teste2">
</p>

**c-) Discussão dos Resultados:** Nessa seção o grupo deve descrever se o teste foi satisfatório ou não;<br>
- A duração da bateria não foi ideal e a necessidade do uso de duas baterias atrapalha a praticidade do sistema.

**d-) Soluções Futuras:** Nessa seção, o que grupo faria para melhorar seus testes (não precisa implementar essas propostas de melhorias).<br>
- A substituição das baterias por outro modelo com voltagem e duração corretas.

<br>

Clique aqui para acessar **toda a visualização da Apresentação** de nosso projeto: [Apresentação](https://www.canva.com/design/DAGFS6GM3Aw/0-2xlqHYrZxdfv8g3aQgjA/edit?utm_content=DAGFS6GM3Aw&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton). 👈 <br>

Clique aqui para acessar **o video Explicativo** de nosso projeto: [Video](https://youtu.be/_0JSFxbW1Z4?si=JQcMbvTRka8SGTjX). 👈 <br>
