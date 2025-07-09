# Projeto: Pipeline de Análise de Raios-X com Sistema Multiagente

![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google_Gemini-API-4285F4?style=for-the-badge&logo=google&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=black)

---

## 🎯 Sobre o Projeto

Este projeto é um estudo prático que demonstra como um **Sistema Multiagente de Inteligência Artificial** pode ser estruturado para auxiliar profissionais da saúde em tarefas de análise de imagens médicas.

O objetivo é explorar como a IA pode automatizar um fluxo de trabalho (pipeline) para otimizar o tempo e fornecer informações de suporte de maneira rápida e organizada. Para isso, foi criada uma "equipe" de 5 agentes de IA especializados, onde cada um executa uma etapa do processo: desde a análise inicial de um raio-x de tórax até a compilação de um relatório completo e enriquecido.

É uma demonstração do potencial da IA como ferramenta de apoio, visando reduzir a carga de trabalho repetitiva e permitir que os profissionais foquem naquilo que é mais crítico: o cuidado com o paciente.

### ✨ Principais Características

* **Pipeline com 5 Agentes Autônomos:** Demonstra uma arquitetura de IA modular e especializada.
* **Hibridismo de IAs:** Combina uma Rede Neural Convolucional (CNN) para análise de imagem com o poder dos Modelos de Linguagem Grandes (LLM) do Google Gemini para raciocínio, pesquisa e redação.
* **Uso de Ferramentas de IA:** Integra ferramentas externas como o **Google Search** e uma ferramenta customizada de data/hora para enriquecer a funcionalidade dos agentes.
* **Relevância com a Área da Saúde:** Aplica conceitos de Data Science e IA em um desafio real da área de Informática na Saúde.

---

## ⚙️ Como Funciona: O Pipeline Multiagente

O sistema funciona como uma linha de montagem, onde uma imagem de raio-x passa por 5 agentes especialistas em sequência. Cada agente realiza sua tarefa e passa o resultado para o próximo.

1.  **Agente 1: O Preparador**
    * **Função:** Recebe a imagem do raio-x e a prepara para análise, ajustando seu tamanho, formato e cores para o padrão que a IA analítica espera.

2.  **Agente 2: O Analista de IA (com CNN)**
    * **Função:** Utiliza o modelo de Machine Learning (treinado previamente) para classificar a imagem, identificando se há sinais característicos de pneumonia.

3.  **Agente 3: O Relator Clínico (com Gemini)**
    * **Função:** Recebe o diagnóstico do analista (ex: "PNEUMONIA") e sua confiança. Com base nisso, usa o Gemini para redigir um laudo técnico preliminar e estruturado.

4.  **Agente 4: O Pesquisador Web (com Gemini + Google Search)**
    * **Função:** Se o diagnóstico é positivo, este agente usa a ferramenta `Google Search` para buscar na internet uma explicação simples sobre a condição e links para fontes confiáveis, como a OMS ou a Mayo Clinic.

5.  **Agente 5: O Compilador Final (com Gemini + Ferramenta Customizada)**
    * **Função:** Recebe o laudo clínico e a pesquisa web. Utiliza uma ferramenta customizada para obter a data e hora atuais e, em seguida, compila todas as informações em um único documento final, coeso e bem formatado.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.11
* **Ambiente:** Google Colab
* **Machine Learning:** TensorFlow / Keras
* **Agentes e LLM:** Google Agent Development Kit (ADK) e API do Google Gemini (modelos Flash e Pro)
* **Ferramentas de IA:** Google Search API
* **Bibliotecas:** Pandas, NumPy, Matplotlib, Pytz

---

## 🚀 Como Executar o Projeto

Para executar este projeto em seu próprio ambiente, siga os passos abaixo.

### Pré-requisitos

* Uma conta Google para acessar o Colab.
* Uma conta Kaggle para obter a chave de API e baixar o dataset.
* Uma chave de API do **Google Gemini**, que pode ser obtida no [Google AI Studio](https://aistudio.google.com/app/apikey).

### Instruções

1.  **Clone o Repositório**
    ```bash
    git clone [https://github.com/Thiago-Alencar/Pipeline-de-An-lise-de-Raios-X-de-T-rax-com-Sistema-Multiagente]
    ```

2.  **Abra no Google Colab**
    * Faça o upload do arquivo `.ipynb` para o seu Google Drive e abra-o com o Google Colab.

3.  **Configure as Chaves de API**
    * **Google Gemini API Key:** No menu lateral esquerdo do Colab, clique no ícone de chave (Segredos) e crie um novo segredo com o nome `GEMINI_API_KEY`, colando a sua chave no campo de valor.
    * **Kaggle API Key:** Ao executar a célula de download do dataset pela primeira vez, o sistema pedirá que você faça o upload do seu arquivo `kaggle.json`.

4.  **Execute as Células**
    * Execute cada célula do notebook em ordem, de cima para baixo. O projeto foi estruturado para que a saída de cada etapa seja clara e compreensível.

---

## ⚠️ Aviso Importante

Este sistema é um **protótipo de estudo**, desenvolvido com o objetivo de pesquisar como a Inteligência Artificial pode servir de ferramenta de apoio para profissionais da saúde.

**Este sistema NÃO é uma ferramenta de diagnóstico médico.** As análises são geradas automaticamente e não possuem validação clínica. A responsabilidade por qualquer diagnóstico ou tratamento é exclusivamente de um profissional de saúde qualificado.

---

## 👨‍💻 Autor

Projeto desenvolvido por **Thiago Alencar Antonio**.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/thiago-alencar-antonio/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Thiago-Alencar/)
