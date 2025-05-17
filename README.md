# Sistema de Simulação de Prevenção de Guerras

Este projeto demonstra a utilização de agentes baseados em modelos de linguagem para simular um cenário de conflito e negociação, com o objetivo de explorar a interação entre diferentes perspectivas e um agente diplomático neutro.

## Funcionalidades

- **Agente Estrategista Russo Invasor:** Simula um estrategista com o objetivo de invasão e apropriação de recursos, evitando acordos diplomáticos.
- **Agente Estrategista Ucraniano Agredido:** Simula um estrategista com o objetivo de defesa, minimizando perdas e buscando negociação.
- **Agente Diplomático Bilateral Neutro:** Analisa as posições dos agentes em conflito e fornece um veredicto ou sugestão para o fim do conflito.

## Pré-requisitos

- É necessário ter uma chave de API do Google Gemini.
- O código utiliza bibliotecas como `google-genai` e `google-adk`.

## Como executar

1. Clone este repositório (se estiver em um).
2. Abra o arquivo em um ambiente Google Colab ou Jupyter Notebook.
3. Certifique-se de configurar sua chave de API do Google Gemini na variável de ambiente `GOOGLE_API_KEY`. No Colab, você pode fazer isso usando `userdata.get('GOOGLE_API_KEY')`.
4. Execute as células do notebook em ordem.

## Código

O código está estruturado em células que:

- Instalam as bibliotecas necessárias.
- Configuram a chave de API e o cliente da SDK do Gemini.
- Definem funções auxiliares para chamar os agentes e formatar a saída.
- Definem os agentes Estrategista Russo, Estrategista Ucraniano e Diplomático.
- Executam a simulação chamando o agente diplomático.

## Estrutura do Código

- `call_agent(agent, message_text)`: Função para enviar uma mensagem para um agente e obter a resposta final.
- `to_markdown(text)`: Função auxiliar para formatar texto em Markdown para exibição no Colab.
- `agente_invasor(text)`: Define e chama o agente estrategista russo.
- `agente_invadido(text)`: Define e chama o agente estrategista ucraniano.
- `agente_diplomatico()`: Define e chama o agente diplomático, integrando as respostas dos outros agentes.

## Observações

- Este é um modelo de simulação simplificado e não reflete a complexidade real de conflitos e negociações.
- O desempenho e as respostas dos agentes podem variar dependendo do modelo de linguagem utilizado e das instruções fornecidas.

## Licença
[LICENSE](https://github.com/luizptm/desafio_alura_gemini_2025/blob/main/LICENSE)
