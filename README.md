# 🤖 RPA: Automação para Nomenclatura e Triagem de Arquivos

Este repositório documenta meu **primeiro protótipo de automação**, desenvolvido para resolver um desafio real de alta repetitividade que enfrentei no início da minha carreira.

## 📖 O Nascimento do Projeto (Contexto)
Este fluxo foi criado na época em que eu trabalhava no setor administrativo como **Jovem Aprendiz**. Minha rotina envolvia a renomeação manual de centenas de documentos, principalmente **contracheques**. Identifiquei que o tempo gasto nesta tarefa mecânica era um gargalo para o setor e decidi aplicar lógica computacional para otimizar o processo através de RPA.

## 📝 O Problema (Business Case)
A organização manual de documentos gerava impactos negativos na operação:
- **Volume:** Fluxo constante de centenas de arquivos semanais.
- **Tempo gasto:** Aproximadamente **4 horas semanais** dedicadas apenas à renomeação.
- **Risco:** Erros de digitação humanos que dificultavam auditorias e a localização posterior dos arquivos.

## 🚀 A Solução
Desenvolvi um fluxo de **RPA (Robotic Process Automation)** no **Microsoft Power Automate Desktop**. O robô realiza a leitura inteligente do conteúdo e a padronização automática dos arquivos.

### 🔍 Detalhamento Técnico do Fluxo
Conforme documentado no [print do fluxo](docs/fluxo-automacao.png), a automação executa as seguintes etapas:
1. **Mapeamento:** Obtém todos os arquivos brutos em uma pasta específica do OneDrive/SharePoint.
2. **Loop de Processamento:** Inicia um ciclo "For each" para tratar cada documento individualmente.
3. **Extração de Dados (OCR):** Extrai todo o conteúdo de texto do PDF para uma variável temporária.
4. **Tratamento de String:** Divide o texto extraído para isolar o nome do colaborador (index [0] da lista).
5. **Nomenclatura Padronizada:** Renomeia o arquivo original concatenando os dados extraídos.
   - **Estrutura de Nome:** `Contracheque_2025_` + `%NOME%`
   - **Exemplo Real:** `Contracheque_2025_LARISSA_MARQUES.pdf`

## 📊 Impacto e Resultados
- **Ganho de Eficiência:** Redução do tempo de execução de 4 horas para **menos de 5 minutos**.
- **Precisão:** Eliminação de 100% dos erros de digitação.
- **Localização:** Busca imediata de documentos através da taxonomia padronizada.

## 📂 Guia do Repositório
- **[docs/](docs/):** Evidência visual da lógica construída no Power Automate.
- **[samples/](samples/):** Modelos fictícios para demonstração do Input (Entrada) e Output (Saída esperada).

---
**Desenvolvido por Larissa Marques** *Foco em Eficiência Operacional e Automação de Processos.*
