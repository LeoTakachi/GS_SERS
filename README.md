# Global Solution 1 - Soluções em Energias Renováveis e Sustentáveis

##  Integrantes
* **Giovane Salazar Fioravante** - RM: 570396
* **Leonardo Basile Takachi** - RM: 569066

## 🚀 Sistema Inteligente de Monitoramento de Energias Renováveis para Missões Espaciais

## 📖 Descrição

Este projeto consiste em uma interface web desenvolvida em HTML, CSS e JavaScript que simula uma plataforma funcional de monitoramento e análise operacional para uma missão espacial. O sistema permite ao usuário inserir informações como temperatura, nível de energia e status da comunicação da nave. Com base nesses dados, o sistema realiza uma análise automática das condições operacionais, identificando possíveis riscos e gerando alertas que auxiliam no acompanhamento da situação atual da missão.

---

## ⚙️ Funcionamento do Sistema

O usuário informa três parâmetros principais:

🌡️ **Temperatura**

Representa a temperatura da nave.

⚡ **Energia**

Representa o percentual de energia disponível no sistema.

📡 **Comunicação**

Indica se a comunicação com a base está ativa ou inativa.

Após clicar em "Iniciar Sessão", os dados são processados e armazenados em um histórico de leituras.

---

## 🧠 Lógica do Sistema

O sistema utiliza estruturas condicionais (if/else) para analisar diferentes cenários operacionais.

### Caso 1 - Superaquecimento

Se:

* Temperatura > 80°C 
* Energia > 20% 
* Comunicação ativa 

Resultado:⚠️ Alerta de superaquecimento!

---

### Caso 2 - Baixa Energia

Se:

* Temperatura ≤ 80°C
* Energia < 20%
* Comunicação ativa
  
Resultado:🔋 Modo de Economia de energia ligado!

---

### Caso 3 - Falha de Comunicação

Se:

* Temperatura ≤ 80°C
* Energia > 20%
* Comunicação inativa
  
Resultado:📡 Falha na Comunicação!

---

### Casos Combinados

O sistema também identifica situações em que múltiplos problemas acontecem simultaneamente:

* Superaquecimento + Baixa Energia
* Superaquecimento + Falha de Comunicação
* Baixa Energia + Falha de Comunicação
* Superaquecimento + Baixa Energia + Falha de Comunicação

Essas combinações geram alertas mais completos para o operador.

---

## 📊 Histórico de Leituras

Todas as leituras realizadas são armazenadas em um vetor JavaScript chamado: historicoLeituras

Com isso, o histórico permite acompanhar a evolução dos parâmetros monitorados durante a missão.

---

## 🔄 Reinicialização

A função de reinicialização:

* Limpa o histórico;
* Limpa os campos do formulário;
* Remove os resultados exibidos;
* Retorna a interface ao estado inicial.

---

## 🎬 Demonstração

Vídeo de demonstração prática do sistema: https://youtu.be/0vVOuCI32kA

---

## 📌 Conclusão

O principal objetivo do sistema é mostrar que através da análise automática dos parâmetros da missão, é possível identificar situações críticas, gerar alertas e auxiliar na tomada de decisão, simulando cenários reais encontrados em operações espaciais e sistemas embarcados.

---
