# Sistema-de-Gestão-de-Pedidos-E-commerce-Simples

## Propósito do Projeto
Este projeto tem como objetivo demonstrar a implementação da pirâmide de testes em um sistema de gestão de pedidos, utilizando .NET (C#). Ele inclui testes unitários, de integração, de sistema e de aceitação, garantindo qualidade e confiabilidade no software.
## 🏷️ Entidades e Funcionalidades

### 1️⃣ Cliente  
- **ID do Cliente**  
- **Nome**  
- **E-mail**  
- **Lista de Pedidos associados**  

### 2️⃣ Pedido  
- **ID do Pedido**  
- **Cliente Associado**  
- **Data do Pedido**  
- **Lista de Itens**  
- **Status do Pedido**  
- **Cálculo do Valor Total do Pedido**  
## Funcionalidades
* Cadastro e consulta de clientes
* Cálculo automático do valor total do pedido
* Controle de status do pedido
## 📊 Cobertura de Código
O relatório de cobertura pode ser acessado [aqui](coverage/index.html).

# 🚀 Como Executar o Projeto Localmente
### 📌 Pré-requisitos  
- .NET 6+ instalado  
- Git instalado
## 🔧 Clonar o Repositório  
git clone https://github.com/Luumano/Sistema-E-commerce.git  
cd Sistema-Ecommerce-main  
## 🔨 Restaurar Dependências e Compilar  
dotnet restore  
dotnet build
## ▶️ Executar a Aplicação  
dotnet run  

## Como Rodar os Testes Automatizados
### Testes Unitários e de Integração
Execute os testes unitários e de integração com o seguinte comando:
* dotnet test

### Testes de Aceitação (SpecFlow)
Para rodar os testes de aceitação utilizando SpecFlow, execute:
* dotnet test --filter Category=AcceptanceTests

## 📊 Cobertura de Código  
O projeto utiliza **Coverlet** para medir a cobertura de código. Para gerar o relatório de cobertura, execute:  
* dotnet test /p:CollectCoverage=true /p:CoverletOutputFormat=lcov

### O relatório será gerado na pasta coverage/.
Para visualizar, utilize um visualizador de cobertura como o ReportGenerator:
* dotnet tool install --global dotnet-reportgenerator-globaltool
* reportgenerator -reports:coverage/*.xml -targetdir:coverageReport

Agora, abra coverageReport/index.html no navegador para ver os detalhes da cobertura! 📈
## 🛠️ Tecnologias Utilizadas  
- .NET 7+  
- xUnit para testes unitários  
- SpecFlow para testes de aceitação  
- Coverlet para análise de cobertura de código  
- FluentAssertions para validação de testes  
- Moq para mocks em testes de integração  
