# Taggy Green

![GitHub repo size](https://img.shields.io/github/repo-size/iuricode/README-template?style=for-the-badge)
![GitHub language count](https://img.shields.io/github/languages/count/iuricode/README-template?style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/iuricode/README-template?style=for-the-badge)
![Bitbucket open issues](https://img.shields.io/bitbucket/issues/iuricode/README-template?style=for-the-badge)
![Bitbucket open pull requests](https://img.shields.io/bitbucket/pr-raw/iuricode/README-template?style=for-the-badge)

<img src="https://drive.google.com/uc?export=view&id=1T2Cs60Ibutkhd6T8ysN7QuDXxoeoIKZW" alt="Exemplo imagem">

> Print do Trello.

### Ajustes e melhorias

O projeto ainda está em desenvolvimento e as próximas atualizações serão voltadas para as seguintes tarefas:

- [x] Definição das User Stories (Padrão 3Cs)
- [x] Priorização do Backlog (Alta, Média, Baixa)
- [ ] Implementação do motor de cálculo de CO2 (Fatores oficiais)
- [ ] Desenvolvimento do Dashboard B2C (Tempo ganho vs. CO2)
- [ ] Exportação de relatórios PDF/CSV para gestão de RH

## 📋 Histórias de Usuário (Backlog)
Legenda de Prioridades:

🔴 Vermelho: Alta Prioridade (Essential/Core)

🟡 Amarelo: Média Prioridade (Growth/Engagement)

🟢 Verde: Baixa Prioridade (Value-Add/Optimization)

##

### 🔴 ID 01: Conversor de Carbono B2B
[![Trello Card](https://img.shields.io/badge/Trello-Abrir_Card-0079BF?style=for-the-badge&logo=trello&logoColor=white)](https://trello.com/c/fAlMfpd4)

> **User Story:** Como Gestor de Sustentabilidade, quero converter passagens de pedágio em dados de CO2​ evitados, para gerar relatórios auditáveis.

```mermaid
graph TD
    Gestor[Gestor] -->|Solicita Relatório| Taggy[Sistema Taggy]
    Taggy --> Coleta[Coleta Passagens]
    Coleta --> Verifica[Verifica Tipo Veículo]
    Verifica -->|Leve| FatorLeve[Aplica Fator Leve]
    Verifica -->|Pesado| FatorPesado[Aplica Fator Pesado]
    FatorLeve --> Calc[Calcula CO2]
    FatorPesado --> Calc
    Calc --> Gera[Gera Relatório]
    Gera -->|Download| Gestor
```
### 🔴 ID 02: Dashboard de Impacto B2C
[![Trello Card](https://img.shields.io/badge/Trello-Abrir_Card-0079BF?style=for-the-badge&logo=trello&logoColor=white)](https://trello.com/c/EwGh5ie4)

> **User Story:** Como usuário B2C, quero visualizar o impacto ambiental positivo das minhas viagens no app, para sentir que minha conveniência contribui para o planeta.

```mermaid
graph TD
    User[Usuário B2C] -->|Abre App| Dash[Dashboard]
    Dash --> Hist[Processa Histórico]
    Hist --> Tempo[Calcula Tempo Ganho]
    Hist --> CO2[Calcula CO2 Evitado]
    Tempo --> Comp[Monta Comparativo]
    CO2 --> Comp
    Comp -->|Exibe Dados| User
```

### 🔴 ID 03: Relatório de ROI Ambiental
[![Trello Card](https://img.shields.io/badge/Trello-Abrir_Card-0079BF?style=for-the-badge&logo=trello&logoColor=white)](https://trello.com/c/DsOkxX0S)

> **User Story:** Como Gerente de RH, quero um relatório de sustentabilidade da frota/benefícios, para justificar o ROI ambiental do serviço para a diretoria.

```mermaid
graph TD
    RH[Gerente RH] -->|Acessa Portal| Sol[Solicita Relatório]
    Sol --> Agrupa[Agrupa Dados Uso]
    Agrupa --> Cons[Consolida Impacto]
    Cons --> Def[Define Formato]
    Def -->|PDF| PDF[Gera PDF]
    Def -->|CSV| CSV[Gera CSV]
    PDF --> RH
    CSV --> RH
```


### 🟡 ID 04: Calculadora Parametrizada
[![Trello Card](https://img.shields.io/badge/Trello-Abrir_Card-0079BF?style=for-the-badge&logo=trello&logoColor=white)](https://trello.com/c/CN29d01o)

> **User Story:** Como Gestor de Sustentabilidade, quero uma calculadora parametrizada no portal, para facilitar meu trabalho de reporte mensal.

```mermaid
graph TD
    Gestor[Gestor] -->|Acessa Portal| Calc[Calculadora]
    Calc -->|Insere Inputs| Proc[Processa Cálculo]
    Proc -->|Integra Dados Tag| Res[Exibe Resultado]
    Res -->|Facilita Reporte| Gestor
```

### 🟡 ID 05: Notificações "Zero Papel"
[![Trello Card](https://img.shields.io/badge/Trello-Abrir_Card-0079BF?style=for-the-badge&logo=trello&logoColor=white)](https://trello.com/c/yY600Kbt)

> **User Story:** Como usuário B2C, quero receber notificações sobre a redução de uso de plástico e papel (tags vs. tickets), para validar meu desejo de ser "mais sustentável".

```mermaid
graph TD
    Rotina[Rotina Mensal] --> Conta[Contabiliza Uso]
    Conta --> Papel[Soma Papel Evitado]
    Conta --> Plastico[Soma Plástico Evitado]
    Papel --> Notif[Gera Notificação]
    Plastico --> Notif
    Notif -->|Envia Push| User[Usuário B2C]
```


### 🟡 ID 06: Kit de Endomarketing ESG
[![Trello Card](https://img.shields.io/badge/Trello-Abrir_Card-0079BF?style=for-the-badge&logo=trello&logoColor=white)](hhttps://trello.com/c/FCMLB8p3)

> **User Story:** Como Gerente de RH, quero comunicar a redução de poluentes aos colaboradores, para aumentar a satisfação e retenção com o benefício.

```mermaid
graph TD
    RH[Gerente RH] -->|Acessa Portal| Temp[Seleciona Template]
    Temp --> Dados[Puxa Dados Reais]
    Dados --> Preenche[Preenche Template]
    Preenche -->|Dispara E-mail| Colab[Colaboradores]
```

### 🟡 ID 07: Rede de Parceiros Verdes
[![Trello Card](https://img.shields.io/badge/Trello-Abrir_Card-0079BF?style=for-the-badge&logo=trello&logoColor=white)](https://trello.com/c/TR6VuAKr)

> **User Story:** Como usuário B2C, quero que o app mostre selos de sustentabilidade parceiros, para consumir de marcas que compartilham meus valores.

```mermaid
graph TD
    User[Usuário B2C] -->|Abre App| Sec[Seção Parceiros]
    Sec --> Lista[Carrega Lista]
    Lista -->|Exibe Selos| User
```

### 🟢 ID 08: Portal de Transparência
[![Trello Card](https://img.shields.io/badge/Trello-Abrir_Card-0079BF?style=for-the-badge&logo=trello&logoColor=white)](https://trello.com/c/osK0bU03)

> **User Story:** Como Gestor de Sustentabilidade, quero acesso a metodologias baseadas em dados públicos, para garantir que os cálculos não sejam questionados.

```mermaid
graph TD
    Gestor[Gestor] -->|Acessa Portal| Menu[Menu Transparência]
    Menu --> Metod[Exibe Metodologia]
    Metod -->|Links Fontes Públicas| Gestor
```

### 🟢 ID 09: Mapa de Cobertura Total
[![Trello Card](https://img.shields.io/badge/Trello-Abrir_Card-0079BF?style=for-the-badge&logo=trello&logoColor=white)](https://trello.com/c/N2CXUdB1)

> **User Story:** Como usuário B2C, quero integrar minha Taggy a 1.000+ estacionamentos e shoppings, para otimizar meu tempo no dia a dia.

```mermaid
graph TD
    User[Usuário B2C] -->|Abre Mapa| API[Chama API Mapa]
    API -->|Carrega 1000+ Pontos| Exibe[Exibe Cobertura]
    Exibe -->|Traça Rota| User
```

### 🟢 ID 10: Fluxo Contínuo RFID
[![Trello Card](https://img.shields.io/badge/Trello-Abrir_Card-0079BF?style=for-the-badge&logo=trello&logoColor=white)](https://trello.com/c/PgU9pfGn)

> **User Story:** Como Gerente de RH, quero uma solução que simplifique a locomoção (RFID), para eliminar filas e estresse para os funcionários.

```mermaid
graph TD
    Carro[Carro Aproxima] -->|Leitura RFID| Cancela[Cancela Abre]
    Cancela -->|Passagem Direta| Log[Registra Log]
    Log -->|Tempo Espera Zero| RH[Gerente RH]
```

## 🤝 Participantes

Agradecemos às seguintes pessoas que contribuíram para este projeto:

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/RenatoCamara99" title="Github do integrante">
        <img src="https://avatars.githubusercontent.com/u/209717695" width="100px;" alt="Foto de Renato Câmara no GitHub"/><br>
        <sub>
          <b>Renato Câmara</b>
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/joaofdurao" title="Github do integrante">
        <img src="https://avatars.githubusercontent.com/u/120042358" width="100px;" alt="Foto de João Durão"/><br>
        <sub>
          <b>João Durão</b>
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/Henrique-Veloso" title="Github do integrante">
        <img src="https://avatars.githubusercontent.com/u/178965096" width="100px;" alt="Foto de Henrique Veloso"/><br>
        <sub>
          <b>Henrique Veloso</b>
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/caiqueassuncao" title="Github do integrante">
        <img src="https://avatars.githubusercontent.com/u/203854341" width="100px;" alt="Foto de Caique Assunção"/><br>
        <sub>
          <b>Caique Assunção</b>
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/phbag-bit" title="Github do integrante">
        <img src="https://avatars.githubusercontent.com/u/226612392" width="100px;" alt="Foto de Pedro Barreiras"/><br>
        <sub>
          <b>Pedro Barreiras</b>
        </sub>
      </a>
    </td>
        <td align="center">
      <a href="https://github.com/FelixCavalcanti" title="Github do integrante">
        <img src="https://avatars.githubusercontent.com/u/222039714" width="100px;" alt="Foto de Luis Felix"/><br>
        <sub>
          <b>Luis Felix</b>
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/aabsm-cesar" title="Github do integrante">
        <img src="https://avatars.githubusercontent.com/u/265135054" width="100px;" alt="Foto de Antonio Sandes"/><br>
        <sub>
          <b>Antonio Sandes</b>
        </sub>
      </a>
    </td>
  </tr>
  <tr>
    <td align="center">
      <sub>
        BACKEND
      </sub>
    </td>
    <td align="center">
      <sub>
        SCRUM MASTER
      </sub>
    </td>
    <td align="center">
      <sub>
        PO
      </sub>
    </td>
    <td align="center">
      <sub>
        FRONTEND
      </sub>
    </td>
    <td align="center">
      <sub>
        BACKEND
      </sub>
    </td>
    <td align="center">
      <sub>
        FRONTEND
      </sub>
    </td>
    <td align="center">
      <sub>
        DB
      </sub>
    </td>
  </tr>
</table>
