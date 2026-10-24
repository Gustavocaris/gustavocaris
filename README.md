<!--<div align="center">
  <img width="70%" src="https://github.com/Gustavocaris/Data_Science/assets/149839159/7a11fecd-5bb6-4783-b0e0-2c106bfd317f"/>
</div>-->

[![Typing SVG](https://readme-typing-svg.herokuapp.com/?color=FF4b33&size=30&center=true&vCenter=true&width=1000&lines=Heyy+Welcomeee☕👨‍💻)](https://git.io/typing-svg)

<img align="right" height="150" src="https://media.tenor.com/dHk-LfzHrtwAAAAm/linux-computer.webp">

<p align="center"> My name is Gustavo, and I’m a technology professional passionate about smart solutions, automation, and continuous learning. Currently, I work in the cloud infrastructure team, dealing with migration projects, internal and external support, virtualized environments, and databases. I also have experience in web development, client support, and collaboration with engineering and product teams. Over the past few months, I’ve been deepening my knowledge in the following areas: Cloud Computing: fundamentals, architecture, and cloud providers such as Azure and AWS. DevOps: culture, agile practices, CI/CD, automation, and process integration. Containerization ande Databases.
</p>

<div align="center">
<img align="center" src="https://github.com/Harlocks/design/blob/main/assets/inkscape/separators/Line.png?raw=true">
</div>
 
<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=aws,azure,terraform,kubernetes,docker,githubactions,ansible,linux,ubuntu,windows,powershell,bash,nginx,go,py,js,html,css,react,nodejs,git,github,vscode&perline=12" />
  </a>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/Oracle_Cloud-F80000?style=for-the-badge&logo=oracle&logoColor=white">
  <img src="https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white">
  <img src="https://img.shields.io/badge/Zabbix-D40000?style=for-the-badge&logo=zabbix&logoColor=white">
</p>
<p align="center">
  🌎 <b>Português</b> (nativo) · <b>English</b> (intermediário) &nbsp;|&nbsp; 📋 Scrum/Kanban · ERP · CRM
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/gustavo-caris"><img src="https://img.shields.io/badge/LinkedIn-Gustavo_Caris-0A66C2?style=flat&logo=linkedin&logoColor=white"></a>
  <a href="https://github.com/Gustavocaris/DevOps-Alire-Cloud"><img src="https://img.shields.io/badge/repo-DevOps--Alire--Cloud-2088FF?style=flat&logo=github&logoColor=white"></a>
  <a href="https://github.com/Gustavocaris/Spotify-AWS-EC2"><img src="https://img.shields.io/badge/repo-Spotify--AWS--EC2-FF9900?style=flat&logo=github&logoColor=white"></a>
  <a href="https://github.com/Gustavocaris/netcheck"><img src="https://img.shields.io/badge/repo-NetCheck-28a745?style=flat&logo=github&logoColor=white"></a>
  <a href="https://ccmtecnologia.com.br/"><img src="https://img.shields.io/badge/trabalho-CCM_Tech-00838F?style=flat&logo=icloud&logoColor=white"></a>
  <a href="https://github.com/Desenvolvimentos-Inteligentes"><img src="https://img.shields.io/badge/org-Inteldev-6E40C9?style=flat&logo=github&logoColor=white"></a>
</p>


### 🗺️ Arquitetura dos Projetos

```mermaid
flowchart LR
    dev(["👨🏻‍💻 Gustavo"])

    subgraph GH["🐙 GitHub"]
        direction TB
        r1["📦 NetHealth"]
        r2["📦 backend-API"]
        r3["📦 terraform-pipeline"]
        r4["📦 Engineering-experiments"]
        r5["🔒 web-tondato"]
        r6["📦 Data-science"]
        r7["📦 DevOps-Aliare-Cloud"]
    end

    dev -- "git push" --> GH

    %% NetHealth: diagnóstico de rede
    r1 --> fe
    subgraph NH["🩺 NetHealth"]
        fe["⚛️ React + TS"] -- "REST" --> api["🟢 Node / Express"]
    end

    %% backend-API
    r2 --> bapi["🔌 REST API"] --> dk["🐳 Docker"]

    %% Pipeline de IaC
    r3 -- "push" --> fmt
    subgraph CI["⚙️ GitHub Actions"]
        direction LR
        fmt["✅ fmt · validate"] --> plan["📋 plan"] --> apply["🚀 apply"]
    end
    apply -- "🏗️ Terraform" --> cloud["☁️ Cloud"]

    %% Ambientes por branch (em estudo)
    subgraph K8S["☸️ Cluster Kubernetes · em estudo"]
        direction TB
        ns1["📁 dev"]
        ns2["📁 staging"]
        ns3["📁 prod"]
    end
    r4 -- "🌿 dev" --> ns1
    r4 -- "🌿 staging" --> ns2
    r4 -- "🌿 main" --> ns3

    %% web-tondato (privado)
    r5 --> site
    subgraph WT["🌐 web-tondato"]
        cms["📝 Sanity CMS"] -- "conteúdo" --> site["🖥️ Site"]
        cms -- "webhook" --> wapi["🔌 API"]
        site -- "formulário" --> wapi
        wapi -- "envio" --> rs["✉️ Resend"]
    end

    %% Estudos
    r6 --> ds["📊 ML · Probabilidade · Estatística"]

    %% Referência de CLI
    r7 --> cli["⌨️ Bash · PowerShell · Git"]

    classDef repo stroke:#58A6FF,stroke-width:2px
    classDef priv stroke:#8B949E,stroke-width:2px,stroke-dasharray:4 4
    class r1,r2,r3,r4,r6,r7 repo
    class r5 priv
    style K8S stroke-dasharray:5 5
```
