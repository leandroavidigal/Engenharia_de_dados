## Projetos de Engenharia de Dados

Bem-vindo(a) ao repositório **Projetos de Engenharia de Dados**!  
Aqui você encontrará soluções práticas e estudos de caso que envolvem desde a ingestão e transformação de dados em larga escala até testes, validação e governança de informações. Cada projeto descreve o uso de diferentes ferramentas e abordagens para lidar com os desafios de um ambiente de dados complexo.

---

### Objetivo do Repositório

Este repositório foi criado para **compartilhar conhecimento** e **demonstrar experiências** em Engenharia de Dados. Os projetos aqui abrangem diversas etapas típicas de pipelines de dados, como:

- **Coleta e Ingestão de Dados** (batch, streaming)  
- **Transformações e Limpeza** (tratamento de dados, normalização, deduplicação)  
- **Modelagem e Armazenamento** (Data Lakes, Data Warehouses, Data Lakehouses)  
- **Criação de Scripts de ETL/ELT**  
- **Boas Práticas de Governança** (LGPD, anonimização, gerenciamento de metadados)  
- **Monitoração e Observabilidade**  
- **Orquestração de Pipelines** (Airflow, Jenkins, etc.)

Ao longo do repositório, você encontrará explicações sobre as arquiteturas adotadas, scripts SQL, códigos em Python/Scala, ferramentas de orquestração e dicas de boas práticas para tornar os pipelines mais robustos, seguros e escaláveis.

---

### Projetos

1. **Migração de Dados entre Azure e GCP**  
   **Descrição:**  
   Este projeto mostra como lidar com discrepâncias de dados entre um ambiente _legacy_ (Azure) e um ambiente _modernized_ (GCP). Foram aplicadas técnicas de hash, mascaramento de dados (para conformidade com a LGPD) e funções de normalização (`lpad`). Após o ajuste de pipelines e transformações, foram realizados testes de validação para garantir equivalência entre as tabelas.  
   **Principais Etapas:**  
   - Análise de inconsistências de volume e formatação  
   - Aplicação de hashes (SHA-256) para dados sensíveis  
   - Padronização de campos de CPF/CNPJ  
   - Validação e comparação de dados entre _legacy_ e _modernized_ usando scripts SQL  
   **Resultados:**  
   A divergência foi eliminada e o processo de migração passou a garantir governança e segurança dos dados, servindo de referência para futuras integrações.  

2. *(Em breve...)* **Migração de dados entre componentes**

---

### Configuração e Ferramentas

A depender do projeto, podem ser utilizadas as seguintes tecnologias/bibliotecas:

- **Python 3.8+** e/ou **Scala**
- **Apache Spark**, **Databricks**, **Delta Lake**
- **Google Cloud Platform (GCP)**, **Microsoft Azure**, **AWS**
- **Airflow**, **Jenkins** ou outras ferramentas de orquestração
- **SQL** para consultas e transformações
- **Ferramentas de Observabilidade** (Prometheus, Grafana etc.)  
- **Docker** e **Kubernetes** (eventualmente, para containerização)

---

### Como Contribuir

1. **Faça um fork** deste repositório.  
2. **Crie uma branch** para suas alterações: `git checkout -b minha-branch`.  
3. **Implemente** suas funcionalidades ou correções.  
4. **Envie as alterações** para o seu fork: `git push origin minha-branch`.  
5. **Abra um Pull Request** descrevendo suas mudanças.

Fique à vontade para contribuir com correções de bugs, melhorias de documentação, novos exemplos de pipelines ou qualquer dica que possa enriquecer a discussão!

---

### Licença e Observações

- Os exemplos e dados utilizados são **fictícios ou anonimizados**, seguindo boas práticas de privacidade.  
- Sinta-se livre para **adaptar** o código ou as ideias às suas próprias necessidades.  
- Antes de adotar qualquer abordagem em **produção**, revise cuidadosamente os requisitos de segurança, governança de dados e conformidade com leis de privacidade.  

---

**Obrigado por visitar o repositório!**  
Qualquer dúvida ou sugestão, fique à vontade para abrir uma _issue_ ou entrar em contato.  
Bons estudos e boas análises de dados!
