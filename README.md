# MiniGuia-Notebooklm-QA
#Conteúdo e Objetivo
Este projeto tem como objetivo usar o Notebooklm como base de estudos de testes 
automatizados utilizando Cypress.

#Proposto:
* Conteúdo
* Engenharia de prompt
* Organização de conteúdo
* Pensamento crítico com auxílio da IA

#Fontes:
* Documentação oficial do Cypress (tradução PT-BR)
* Introduction to Cypress App
* Cypress API: Table of Contents
* Best Practices - Cypress Documentation
* Continuous Integration with Cypress
* Comparação: Cypress vs Selenium vs Playwright
* Cypress com BDD/Cucumber
* React Component Testing
* Vídeos sobre instalação e autenticação SSO

#Engenharia de prompt e aprendizagem

* Cypress API: Table of Contents
* Best Practices - Cypress Documentation
* Continuous Integration with Cypress
* Comparação: Cypress vs Selenium vs Playwright
* Cypress com BDD/Cucumber
* React Component Testing
* Vídeos sobre instalação e autenticação SSO

#Engenharia de Prompts e Aprendizados

#Prompt 1
#Pergunta: O que são testes automatizados?
Resumo da resposta:
Testes automatizados utilizam scripts para simular ações do usuário e validar o funcionamento da aplicação. Seguem três etapas: configuração, ação e validação.
#Dificuldade:
Resposta inicial muito ampla.
#Ajuste:
Refinei pedindo exemplos práticos com Cypress.

#Prompt 2
#Pergunta: Como instalar e configurar o Cypress do zero?
Resumo da resposta:
* Instalar Node.js
* Rodar `npm init -y`
* Instalar Cypress
* Executar `npx cypress open`
* Criar primeiros testes
#Dificuldade:
Muitos detalhes técnicos.
#Ajuste:
Pedi versão simplificada para iniciantes.

#Prompt 3
#Pergunta: O Cypress é a melhor ferramenta para testes automatizados?
Resumo da resposta:
Depende do projeto, mas se destaca por:
* Espera automática
* Debug fácil
* Execução no navegador
#Dificuldade:
Comparação superficial.
#Ajuste:
Solicitei comparação com outras ferramentas.

#Prompt 4
#Pergunta: Como usar cy.intercept?
Resumo da resposta:
Permite simular respostas de API (mock), testar erros e controlar dados sem backend real.
#Dificuldade:
Entender aplicação prática.
#Ajuste:
Pedi exemplos reais.

#Exemplos Práticos
✔ Teste simples

javascript
describe('Teste básico', () => {
  it('Visita e valida página', () => {
    cy.visit('https://example.cypress.io')
    cy.contains('type').click()
    cy.url().should('include', '/commands/actions')
  })
})

✔ Interceptação de API

javascript
cy.intercept('GET', '/api/dados', {
  statusCode: 500,
  body: { message: 'Erro no servidor' }
}).as('erro')

cy.wait('@erro')

#Conclusão
O uso do NotebookLM facilitou a organização do conteúdo e tornou o aprendizado mais fácil de compreender.
Além de aprender conteúdos sobre Cypress, foi possível desenvolver habilidades importantes como:
* Análise crítica
* Escrita técnica
* Interação com IA
  

