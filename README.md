# Procuradoria da Mulher 🛡️

![Status](https://img.shields.io/badge/Status-Em_Produção-success?style=for-the-badge) ![Impact](https://img.shields.io/badge/Impacto-Social_Crítico-purple?style=for-the-badge) ![Tech](https://img.shields.io/badge/Tech-Flutter_|_GetX-blue?style=for-the-badge)

> **Nota:** Este repositório é um **estudo de caso** de um software proprietário desenvolvido por mim na [IntellGest](https://www.linkedin.com/company/intellgest/). Ele serve como demonstração de portfólio técnico e **não contém o código-fonte original**.

---

## 📱 Sobre o Projeto

O aplicativo da **Procuradoria da Mulher** é uma plataforma vital que oferece informações, serviços de assistência jurídica e orientações sobre direitos da mulher. Além de conteúdos educativos e políticas públicas para igualdade de gênero, o app serve como uma ferramenta de **apoio e proteção imediata** contra a violência de gênero.

O projeto exigiu rigorosos padrões de segurança de dados, anonimato e performance, visto que a falha no funcionamento ou lentidão poderia colocar vidas em risco.

## 👨‍💻 Meu Papel: Desenvolvimento End-To-End

Atuei como **Líder Técnico Mobile**, responsável pela arquitetura da solução, escolha da stack tecnológica e desenvolvimento das funcionalidades críticas de segurança e comunicação em tempo real.

* **Desafio:** Garantir que o pedido de socorro funcionasse mesmo em redes instáveis e que a interface fosse acessível e fluida em dispositivos de entrada.
* **Solução:** Implementação de uma arquitetura reativa leve com **GetX** e estratégia de persistência local **offline-first** com ObjectBox.

## 🚀 Engenharia e Funcionalidades Críticas

### 1. Botão de Pânico com Geolocalização (Background) 📍
A funcionalidade mais crítica do sistema. Ao ser acionado, o app captura silenciosamente as coordenadas GPS exatas do dispositivo e envia um alerta prioritário para a central.
* **Engenharia:** Utilização de **Dart Isolates** para processar a localização em threads separadas, garantindo que a UI nunca trave durante uma emergência, independente da carga do processador.

### 2. Videoconferência Integrada (Telemedicina Jurídica) 📹
Integração nativa com a API do **Jitsi Meet**. Desenvolvi um módulo que permite às vítimas realizarem atendimentos psicológicos ou jurídicos via vídeo diretamente no app, garantindo um ambiente criptografado e seguro sem expor o usuário a links externos.

### 3. Denúncia Anônima e Gestão de Mídia 🔒
Sistema robusto para envio de evidências (fotos, vídeos e áudio) com total anonimato.
* **Segurança:** O app gerencia permissões de hardware sensíveis e realiza compressão inteligente de mídia antes do upload, otimizando o envio em conexões móveis 3G/4G.

## 🛠️ Tech Stack

* **Linguagem:** Dart
* **Framework:** Flutter
* **Gerência de Estado:** GetX (Performance e Injeção de Dependências)
* **Persistência:** ObjectBox (NoSQL de alta performance)
* **Backend Services:** Firebase (Auth & Push Notifications)
* **Integrações:** Jitsi SDK, Google Maps API, Image Picker
