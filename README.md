# 🤖 RPA: Automação para Nomenclatura e Triagem de Arquivos

Este repositório apresenta o meu **primeiro protótipo de automação**, desenvolvido para resolver um desafio real que enfrentei no início da minha trajetória profissional.

## 📖 O Nascimento do Projeto (Contexto)
Este fluxo foi criado na época em que eu trabalhava no setor administrativo como **Jovem Aprendiz**. Minha rotina envolvia a renomeação manual e constante de documentos, principalmente **contracheques**, para organização em pastas de rede. Percebi que o tempo gasto nessa tarefa mecânica poderia ser melhor aproveitado se utilizássemos a lógica computacional a nosso favor.

## 📝 O Problema (Business Case)
O processo manual de organização gerava um gargalo operacional significativo:
- **Volume:** Centenas de documentos processados semanalmente.
- **Tempo gasto:** Média de 4 horas semanais apenas para triagem e nomenclatura.
- **Risco:** Erros de digitação em nomes e CPFs, o que dificultava auditorias e a localização futura dos arquivos.

## 🚀 A Solução
Implementei uma solução de **RPA (Robotic Process Automation)** utilizando **Microsoft Power Automate** .

### Funcionalidades do Fluxo:
1. **Monitoramento Ativo:** O robô identifica novos arquivos em uma pasta de entrada.
2. **Extração via OCR:** Leitura automática do conteúdo dos PDFs para identificar campos variáveis.
3. **Padronização de Nomenclatura:** O fluxo foi programado para concatenar os dados e gerar um nome de arquivo padronizado: 
   - **Estrutura:** `[NOME DO COLABORADOR] + [TIPO DE DOCUMENTO] + [ANO]`

### Funcionalidades do Fluxo:
1. **Monitoramento Ativo:** O robô identifica novos arquivos em uma pasta de entrada.
2. **Extração via OCR:** Leitura automática do conteúdo dos PDFs para identificar campos variáveis (Nome, Data e Identificação).
3. **Lógica de String:** Tratamento dos dados extraídos para seguir um padrão rigoroso de nomenclatura.

## 📊 Impacto e Resultados
- **Produtividade:** Redução do tempo de execução de 4 horas para **menos de 5 minutos**.
- **Precisão:** Erro humano reduzido a 0%.
- **Padronização:** 100% dos arquivos organizados conforme as normas internas.

## 📂 Estrutura do Repositório
- `/docs`: Diagramas e capturas de tela do fluxo de lógica no Power Automate.
- `/samples`: Modelos de arquivos fictícios (Certificados) utilizados para demonstrar o funcionamento da lógica de extração.

---
**Desenvolvido por Larissa Marques** *Foco em Eficiência Operacional e Automação de Processos.*
