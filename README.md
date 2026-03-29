❄️ Bot Especialista em Garantia - RR Climatização
Este projeto foi desenvolvido como parte da disciplina de Inteligência Artificial no curso de Análise e Desenvolvimento de Sistemas da FATEC Praia Grande.

O objetivo é a criação de um assistente virtual de domínio restrito para suporte sobre políticas de garantia de ar-condicionado, utilizando técnicas de Prompt Engineering para evitar alucinações e garantir a conformidade com as regras de negócio.

🚀 Funcionalidades e Regras de Negócio
Domínio Restrito: O bot é um especialista exclusivo em prazos e condições de garantia da RR Climatização.

Políticas de Garantia:

1 Ano: Para instalações realizadas por técnicos NÃO credenciados.

2 Anos: Para instalações realizadas por técnicos credenciados.

Obrigatoriedade: Exigência de Nota Fiscal para qualquer atendimento.

Controle de Alucinação: - temperature=0.1: Garante respostas factuais e consistentes.

top_p=0.95 e top_k=10: Filtram a geração de texto para manter o foco técnico.

Fluxo Controlado: Sistema de interação em 3 turnos. Na última resposta, o bot consolida os pontos discutidos em um resumo final.

🛠️ Tecnologias e Modelos
Linguagem: Python (Ambiente Google Colab)

SDK: google-genai (v1.0+)                                                                                                                                                                                                                                                                                                                                                                                                                                  ## 📋 Passo a Passo para Reprodução

Siga as etapas abaixo para executar o projeto em seu ambiente:

1. *Obter Chave de API:*
   - Acesse o [Google AI Studio](https://aistudio.google.com/) e gere sua chave de API.
2. *Configuração no Google Colab:*
   - Abra o arquivo .ipynb deste repositório no Google Colab.
   - No menu lateral, clique no ícone de chave (*Secrets*) e adicione uma nova chave com o nome exato: GOOGLE_API_KEY.
3. *Execução das Células:*
   - *Célula 1:* Instalação e importação das bibliotecas necessárias.
   - *Célula 2:* Definição das System Instructions (Personalidade e Conhecimento) e configuração dos parâmetros top_p e top_k.
   - *Célula 3:* Execução do chatbot em loop de 3 perguntas com geração de resumo final.
   - Desenvolvido por: Stefany Karoline Instituição: FATEC Praia Grande - 2026
