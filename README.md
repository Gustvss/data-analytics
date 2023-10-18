# data-analytics
classDiagram
  class "API de Detecção de Fraude" {
    + monitorarTransacaoEmTempoReal()
    + detectarPadroesSuspeitos()
    + gerarAlerta()
    + sugerirAcoesProativas()
    + integrarDadosExternos()
    + gerarRelatoriosEAuditoria()
    + permitirMelhoriasContinuas()
    + garantirSegurancaEPrivacidade()
  }
  class "Aprendizado de Máquina" {
    + criarModelosDeDeteccaoDeFraude()
  }
  class "Serviços da AWS" {
    + EC2
    + RDS
    + S3
    + SNS
    + CloudWatch
    + IAM
  }
  class "Linguagens de Programação" {
    + Java
    + Python
  }
  class "Banco de Dados" {
    + MySQL
    + PostgreSQL
  }
  class "Bibliotecas de Aprendizado de Máquina" {
    + TensorFlow
    + scikit-learn
  }
  class "Serviços de Fila" {
    + AWS SQS
  }
  class "Ferramentas de Pré-processamento de Dados" {
    + Pandas
    + NumPy
  }
  class "Ferramentas de Desenvolvimento" {
    + IDEs Java
    + IDEs Python
    + Git
  }
  class "Ferramentas de Documentação" {
    + Markdown
    + Swagger
  }

  "API de Detecção de Fraude" --o "Aprendizado de Máquina" : Usa
  "API de Detecção de Fraude" --o "Serviços da AWS" : Usa
  "API de Detecção de Fraude" --o "Linguagens de Programação" : Usa
  "API de Detecção de Fraude" --o "Banco de Dados" : Usa
  "API de Detecção de Fraude" --o "Serviços de Fila" : Usa
  "API de Detecção de Fraude" --o "Ferramentas de Pré-processamento de Dados" : Usa
  "API de Detecção de Fraude" --o "Ferramentas de Desenvolvimento" : Usa
  "API de Detecção de Fraude" --o "Ferramentas de Documentação" : Usa

  "API de Detecção de Fraude" --|> "Aprendizado de Máquina" : Utiliza
  "API de Detecção de Fraude" --|> "Banco de Dados" : Armazena Dados
  "API de Detecção de Fraude" --|> "Serviços de Fila" : Processa Transações
  "API de Detecção de Fraude" --|> "Ferramentas de Pré-processamento de Dados" : Pré-processa Dados
  "API de Detecção de Fraude" --|> "Ferramentas de Desenvolvimento" : Implementa
  "API de Detecção de Fraude" --|> "Ferramentas de Documentação" : Documenta
