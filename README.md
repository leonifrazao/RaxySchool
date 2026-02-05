<a id="readme-top"></a>

<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![License][license-shield]][license-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/leonifrazao/RaxySchool">
    <img src="itens/logo.png" alt="Logo" width="200" height="200">
  </a>

  <h3 align="center">RaxySchool</h3>

  <p align="center">
    Sistema de Análise de Faltas Escolares da Rede Estadual de São Paulo
    <br />
    <a href="https://github.com/leonifrazao/RaxySchool"><strong>Explore a documentação »</strong></a>
    <br />
    <br />
    <a href="https://github.com/leonifrazao/RaxySchool/releases">Ver Releases</a>
    ·
    <a href="https://github.com/leonifrazao/RaxySchool/issues/new?labels=bug&template=bug-report---.md">Reportar Bug</a>
    ·
    <a href="https://github.com/leonifrazao/RaxySchool/issues/new?labels=enhancement&template=feature-request---.md">Solicitar Funcionalidade</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Índice</summary>
  <ol>
    <li>
      <a href="#sobre-o-projeto">Sobre o Projeto</a>
      <ul>
        <li><a href="#construído-com">Construído Com</a></li>
      </ul>
    </li>
    <li>
      <a href="#começando">Começando</a>
      <ul>
        <li><a href="#pré-requisitos">Pré-requisitos</a></li>
        <li><a href="#instalação">Instalação</a></li>
      </ul>
    </li>
    <li><a href="#uso">Uso</a></li>
    <li><a href="#funcionalidades">Funcionalidades</a></li>
    <li><a href="#exemplos-de-análises">Exemplos de Análises</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contribuindo">Contribuindo</a></li>
    <li><a href="#licença">Licença</a></li>
    <li><a href="#contato">Contato</a></li>
    <li><a href="#agradecimentos">Agradecimentos</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## Sobre o Projeto

[![RaxySchool Screen Shot][product-screenshot]](https://github.com/leonifrazao/RaxySchool)

O **RaxySchool** é uma ferramenta completa para análise de faltas de alunos da rede estadual de ensino de São Paulo, utilizando dados fornecidos pela **Secretaria de Educação do Estado de São Paulo (SED)**. O sistema permite que gestores escolares, coordenadores pedagógicos e educadores identifiquem padrões de ausências e tomem decisões baseadas em dados para melhorar a frequência e o desempenho escolar.

### Por que usar RaxySchool?

* 📊 **Análise Detalhada**: Visualize padrões de faltas por período, escola, sala e região
* 📧 **Notificações Automatizadas**: Envie mensagens automáticas para pais sobre as ausências
* 📈 **Relatórios Visuais**: Gráficos e relatórios intuitivos para facilitar a tomada de decisões
* 🎯 **Identificação de Riscos**: Detecte alunos em situação de risco de evasão escolar
* ⚡ **Interface Amigável**: Interface gráfica moderna e fácil de usar

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

### Construído Com

* [![Python][Python.py]][Python-url]
* [![Pandas][Pandas]][Pandas-url]
* [![Tkinter][Tkinter]][Tkinter-url]
* [![Selenium][Selenium]][Selenium-url]

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

<!-- GETTING STARTED -->
## Começando

Para começar a usar o RaxySchool, siga estas etapas simples de instalação.

### Pré-requisitos

Antes de começar, certifique-se de ter os seguintes requisitos:

* **Python**: Versão 3.7 ou superior
  ```sh
  python --version
  ```
* **Google Chrome**: Navegador atualizado (para automação com Selenium)
* **Acesso à SED**: Credenciais válidas para acesso ao sistema da Secretaria de Educação

### Instalação

1. Clone o repositório
   ```sh
   git clone https://github.com/leonifrazao/RaxySchool.git
   ```

2. Navegue até o diretório do projeto
   ```sh
   cd RaxySchool
   ```

3. Instale as dependências necessárias
   ```sh
   pip install -r requirements.txt
   ```

4. Configure suas credenciais de acesso à SED (se necessário)
   ```python
   # Edite as configurações no arquivo de configuração
   ```

5. Execute a aplicação
   ```sh
   python RaxySchool.py
   ```

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

<!-- USAGE -->
## Uso

### Interface Principal

A interface do RaxySchool foi desenvolvida com **CustomTkinter** para proporcionar uma experiência moderna e intuitiva:

1. **Login no Sistema**: Insira suas credenciais da SED
2. **Seleção de Período**: Escolha o período letivo que deseja analisar
3. **Visualização de Dados**: Veja relatórios e gráficos em tempo real
4. **Exportação**: Exporte relatórios em formato PDF ou Excel

### Exemplos de Comandos

```python
# Carregar dados de uma escola específica
from RaxySchool import DataAnalyzer

analyzer = DataAnalyzer()
analyzer.load_school_data(school_id="123456")

# Gerar relatório de faltas
report = analyzer.generate_absence_report()
report.export_to_pdf()
```

_Para mais exemplos e documentação detalhada, consulte a [Wiki](https://github.com/leonifrazao/RaxySchool/wiki)_

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

<!-- FEATURES -->
## Funcionalidades

- [x] 📊 **Coleta Automática de Dados**: Extração de dados diretamente da SED
- [x] 📈 **Análise de Padrões**: Identificação de tendências de ausências
- [x] 📧 **Notificações para Pais**: Sistema automatizado de alertas
- [x] 🎨 **Interface Gráfica Moderna**: Desenvolvida com CustomTkinter
- [x] 📉 **Gráficos Interativos**: Visualizações dinâmicas de dados
- [x] 📄 **Geração de Relatórios**: Exportação em PDF e Excel
- [x] 🔍 **Análise por Período**: Comparação de dados entre bimestres/trimestres
- [x] 🏫 **Análise por Escola/Sala**: Detalhamento por unidade escolar
- [ ] 📱 Versão Mobile (em desenvolvimento)
- [ ] 🤖 Integração com WhatsApp API
- [ ] 📊 Dashboard Web Interativo
- [ ] 🔔 Sistema de Alertas em Tempo Real

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

<!-- EXAMPLES -->
## Exemplos de Análises

### 1. 📅 Distribuição de Faltas por Período

Análise temporal que identifica períodos críticos com altos índices de ausências ao longo do ano letivo, permitindo ações preventivas em momentos estratégicos.

### 2. 📧 Mensagens Automatizadas

Sistema de envio automático de notificações para responsáveis sobre as ausências dos alunos, promovendo maior engajamento familiar na vida escolar.

### 3. 🎓 Faltas por Sala

Comparação detalhada das ausências entre diferentes séries e ciclos escolares, auxiliando na identificação de turmas que necessitam de intervenções específicas.

### 4. 📊 Impacto no Desempenho Escolar

Análise cruzada entre padrões de faltas e desempenho acadêmico dos alunos, revelando a correlação entre frequência e aproveitamento escolar.

### 5. 🗺️ Análise Geográfica

Mapeamento das ausências por região, escola e distrito, permitindo identificar áreas que necessitam de atenção especial.

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

<!-- ROADMAP -->
## Roadmap

- [x] Sistema de coleta de dados da SED
- [x] Interface gráfica com CustomTkinter
- [x] Geração de relatórios básicos
- [x] Sistema de notificações por e-mail
- [ ] Implementar dashboard web
- [ ] Integração com WhatsApp Business API
- [ ] Sistema de predição de evasão escolar usando ML
- [ ] Aplicativo mobile (iOS/Android)
- [ ] API REST para integração com outros sistemas
- [ ] Sistema de backup automático
- [ ] Suporte multi-idioma
- [ ] Modo offline para análise de dados

Veja as [issues abertas](https://github.com/leonifrazao/RaxySchool/issues) para uma lista completa de funcionalidades propostas e problemas conhecidos.

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

<!-- CONTRIBUTING -->
## Contribuindo

As contribuições são o que tornam a comunidade open source um lugar incrível para aprender, inspirar e criar. Qualquer contribuição que você fizer será **muito apreciada**.

Se você tiver uma sugestão para melhorar o projeto, faça um fork do repositório e crie um pull request. Você também pode simplesmente abrir uma issue com a tag "enhancement".
Não se esqueça de dar uma estrela ao projeto! Obrigado novamente!

1. Faça um Fork do Projeto
2. Crie sua Branch de Funcionalidade (`git checkout -b feature/NovaFuncionalidade`)
3. Commit suas Mudanças (`git commit -m 'Adiciona NovaFuncionalidade'`)
4. Push para a Branch (`git push origin feature/NovaFuncionalidade`)
5. Abra um Pull Request

### Principais Contribuidores

<a href="https://github.com/leonifrazao/RaxySchool/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=leonifrazao/RaxySchool" alt="contrib.rocks image" />
</a>

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

<!-- LICENSE -->
## Licença

Distribuído sob a Licença MIT. Veja `LICENSE` para mais informações.

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

<!-- CONTACT -->
## Contato

Leoni Frazão - [@leonifrazao](https://github.com/leonifrazao)

Link do Projeto: [https://github.com/leonifrazao/RaxySchool](https://github.com/leonifrazao/RaxySchool)

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Agradecimentos

Recursos e ferramentas que tornaram este projeto possível:

* [Python Documentation](https://docs.python.org/)
* [Pandas Documentation](https://pandas.pydata.org/)
* [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)
* [Selenium WebDriver](https://www.selenium.dev/)
* [Secretaria de Educação do Estado de São Paulo](https://www.educacao.sp.gov.br/)
* [Choose an Open Source License](https://choosealicense.com)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

---

<div align="center">

### 🎓 Desenvolvido com foco na educação

*Ajudando escolas a melhorar a frequência e o desempenho dos alunos através de dados*

**[⬆ Voltar ao topo](#readme-top)**

</div>

<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/leonifrazao/RaxySchool.svg?style=for-the-badge
[contributors-url]: https://github.com/leonifrazao/RaxySchool/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/leonifrazao/RaxySchool.svg?style=for-the-badge
[forks-url]: https://github.com/leonifrazao/RaxySchool/network/members
[stars-shield]: https://img.shields.io/github/stars/leonifrazao/RaxySchool.svg?style=for-the-badge
[stars-url]: https://github.com/leonifrazao/RaxySchool/stargazers
[issues-shield]: https://img.shields.io/github/issues/leonifrazao/RaxySchool.svg?style=for-the-badge
[issues-url]: https://github.com/leonifrazao/RaxySchool/issues
[license-shield]: https://img.shields.io/github/license/leonifrazao/RaxySchool.svg?style=for-the-badge
[license-url]: https://github.com/leonifrazao/RaxySchool/blob/master/LICENSE
[product-screenshot]: itens/logo.png
[Python.py]: https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white
[Python-url]: https://www.python.org/
[Pandas]: https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white
[Pandas-url]: https://pandas.pydata.org/
[Tkinter]: https://img.shields.io/badge/Tkinter-3776AB?style=for-the-badge&logo=python&logoColor=white
[Tkinter-url]: https://docs.python.org/3/library/tkinter.html
[Selenium]: https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white
[Selenium-url]: https://www.selenium.dev/
