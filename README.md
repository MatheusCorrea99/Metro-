# MetrôBot SP 2.0 (Linhas 1, 2 e 3)
🚇 MetrôBot SP 2.0
Disciplina: Inteligência Artificial e Machine Learning

Integrantes: Daniel Santiago, Eduardo Carotenuto, Everton Tiburcio, Fauzer Ribeiro e Matheus Diorio

Status: Projeto Acadêmico / Concluído

📖 Sobre o Projeto
O MetrôBot SP 2.0 é a evolução de um sistema inteligente desenvolvido para simular e otimizar rotas no transporte metropolitano. Unindo conceitos fundamentais de Inteligência Artificial — como busca em grafos, lógica formal, motores de inferência e Modelos de Linguagem (LLMs) —, esta versão expande a abrangência para cobrir 52 estações integradas através das principais linhas do Metrô de São Paulo:

Linha 1-Azul

Linha 2-Verde

Linha 3-Vermelha

O sistema lida com cenários complexos do mundo real (simulados), como baldeações, acessibilidade, estações bloqueadas e paralisações completas de linhas.

🧠 Principais Funcionalidades e Conceitos
Algoritmos de Busca: Utiliza BFS (Busca em Largura) e DFS (Busca em Profundidade) para encontrar rotas, permitindo comparar o esforço computacional de cada algoritmo através do número de estações visitadas.

Motor de Inferência e Lógica:

Emprega lógica proposicional e de primeira ordem.

Regra R6: Identifica automaticamente as integrações e baldeações entre as linhas, sem necessidade de cadastro manual.

Regra R7 (Nova): Desenvolvida pelo grupo para simular a paralisação de uma linha inteira, bloqueando automaticamente todas as suas estações durante a busca de rotas.

Intérprete e Narrador com IA (Llama):

Quando habilitado, o intérprete traduz comandos em linguagem natural escritos pelo usuário em dados estruturados.

O narrador apresenta o itinerário final (incluindo baldeações) de forma fluida e natural. (Nota: A lógica de decisão da rota permanece estritamente sob o controle dos algoritmos de busca e regras formais).

Interface Gráfica Interativa (ipywidgets): Painel visual completo para configurar origem, destino, algoritmo, acessibilidade, estações fechadas, elevadores em manutenção e linhas paralisadas.

🛠️ Como Executar
O projeto foi estruturado para ser executado diretamente no ambiente do Google Colab.

Abra o arquivo Desafio_MetroBot_SP_2.0.ipynb no Google Colab.

Execute as células em ordem (de cima para baixo) ou utilize a opção Executar tudo / Run All.

Configuração de Provedores de IA (PROVEDOR na Célula 2):
Modo Offline (Padrão): PROVEDOR = "offline" — Funciona totalmente sem internet e sem necessidade de chaves de API.

Via Groq (Llama): PROVEDOR = "groq" — Requer a configuração da variável GROQ_API_KEY nos Secrets do Colab ou em um arquivo .env.

Via Ollama: PROVEDOR = "ollama" — Para execução utilizando um modelo local.

🧪 Bateria de Testes
O notebook inclui uma função automatizada e um painel de validação:

Função rodar_testes(): Executa os 6 casos obrigatórios do desafio e mais 4 casos adicionais criados pelo grupo.

Cenários testados: Validação de quantidade de paradas, eficiência de baldeações, desvios na rede e contornos de estações bloqueadas ou linhas paralisadas.

⚠️ Aviso Legal: Este projeto possui fins estritamente acadêmicos. Informações sobre tempos de viagem, manutenções, estações fechadas e paralisações são cenários simulados para fins de demonstração técnica dos algoritmos de IA.
