# Glossary
Glossário de termos para auxiliar no aprendizado

# Maven
O que é: Uma ferramenta de gerenciamento de projetos e automação de build, principalmente para projetos Java.
 - Principais Funcionalidades:
   
    Gerenciamento de dependências.
    Automação do processo de build (compilação, testes, empacotamento).
    Organização de projetos seguindo uma estrutura padrão.
    Suporte a plugins para estender funcionalidades.
# Spring Boot
 - O que é: É um framework Java baseado no Spring Framework que simplifica o desenvolvimento de aplicativos, especialmente web, permitindo criar aplicações prontas para produção com configuração mínima.
 - Principais recursos do Spring Boot:
   
   Configuração Automática: Ajusta automaticamente muitos aspectos do aplicativo, reduzindo a necessidade de configuração manual.
   Standalone: Permite que as aplicações sejam executadas de forma independente, sem precisar de um servidor de aplicativos separado.
   Maven/Gradle: Suporta construção de projetos com Maven ou Gradle, facilitando o gerenciamento de dependências.
   Facilidade de Testes: Oferece ferramentas para testes de integração e unitários.
   Segurança: Integra facilmente com o Spring Security para autenticação e autorização.

# Spring Boot Actuator
 - O que é: Um módulo do Spring Boot que adiciona funcionalidades de monitoramento e gerenciamento para aplicações.
 - Principais Funcionalidades:
   
    Exposição de métricas, informações de sistema, e endpoints de gerenciamento (como /health, /metrics, etc.).
    Facilidade de integração com ferramentas de monitoramento e gerenciamento.
# Micrometer
 - O que é: Uma biblioteca de instrumentação para monitoramento de métricas de aplicações, agnóstica de backend.
 - Principais Funcionalidades:
   
    Coleção e exposição de métricas (como contadores, temporizadores, etc.).
    Suporte a múltiplos sistemas de monitoramento e gerenciamento, como Prometheus, Graphite, e outros.
    Integração direta com Spring Boot via Actuator para exposição das métricas.
# Prometheus
 - O que é: Uma plataforma de monitoramento e alerta orientada a séries temporais, usada para coletar e consultar métricas de sistemas e serviços.
 - Principais Funcionalidades:
   
    Coleção de métricas através de scraping de endpoints (geralmente no formato /metrics).
    Armazenamento de métricas como séries temporais.
    Sistema de alertas baseado em regras definidas.
    Possui uma linguagem de consulta própria (PromQL) para analisar e visualizar métricas.

# Relação entre Maven, Actuator, Micrometer e Prometheus
   _Maven_ é usado para gerenciar o projeto e suas dependências, incluindo as bibliotecas Spring Boot, Actuator e Micrometer.
   
   _Actuator_ expõe endpoints de gerenciamento e métricas de uma aplicação Spring Boot, facilitando o monitoramento.
   
   _Micrometer_ serve como uma camada de instrumentação que coleta métricas e as fornece para sistemas de monitoramento como o Prometheus.
   
   _Prometheus_ coleta as métricas expostas pela aplicação (via Actuator e Micrometer) para monitoramento e análise.
   
Essas ferramentas juntas formam uma stack poderosa para o desenvolvimento, gerenciamento, e monitoramento de aplicações Java, especialmente no ecossistema Spring.
