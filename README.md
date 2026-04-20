# 🎵 Nio Music Premium

![Banner](https://img.shields.io/badge/Status-Operacional-success?style=for-the-badge&logo=statuspage)
![Version](https://img.shields.io/badge/Versão-1.0.8-blue?style=for-the-badge)
![License](https://img.shields.io/badge/Licença-Premium-gold?style=for-the-badge)

O **Nio Music Premium** é um ecossistema completo para download e gerenciamento de músicas em alta fidelidade. Unindo uma interface inspirada no *Spotify* e *YouTube Music* com um motor de processamento robusto, ele oferece uma experiência desktop definitiva com sistema de licenciamento inteligente.

---

## 💎 Diferenciais & Funcionalidades

### 🚀 Motor de Download Nativo
* **Alta Fidelidade:** Extração de áudio em MP3 a 320kbps (Qualidade 0).
* **Processamento em Massa:** Adicione múltiplos vídeos ou playlists inteiras à fila e baixe tudo com um clique.
* **Compactação Inteligente:** Opção de extrair as faixas diretamente em um arquivo `.ZIP` organizado.
* **Tecnologia yt-dlp:** Utiliza o motor mais atualizado do mercado para evitar bloqueios e garantir velocidade máxima.

### 🎨 Interface Ultra-Moderna (Glassmorphism)
* **Design Translúcido:** UI baseada em transparências e desfoque de fundo (Frosted Glass).
* **Navegação Fluida:** Transições suaves entre as abas de Descobrir, Downloads e Conta.
* **Layout Adaptável:** Sidebar lateral colapsável e grid de músicas auto-ajustável.

### 🔐 Segurança & Licenciamento
* **Híbrido de Autenticação:** Login via Discord (OAuth2) e Google.
* **Trava de Hardware (HWID):** Chaves atreladas à placa-mãe do PC para evitar compartilhamento indevido.
* **Verificação de Servidor:** Benefício *Lifetime* automático para membros que estão no servidor oficial do Discord.
* **Chaves Universais:** Sistema de chaves promocionais para eventos (ex: NATAL-VIP) com data de expiração automática.

### 🛡️ Painel Administrativo Integrado
* **Dashboard Secreto:** Área restrita no app para Donos e Administradores.
* **Fábrica de Keys:** Geração de licenças temporárias ou permanentes em tempo real.
* **Gestão de Cargos:** O Dono pode promover membros a Administradores diretamente pela interface.

---

## 🛠️ Tecnologias Utilizadas

| Componente | Tecnologia |
| :--- | :--- |
| **Frontend** | React + Vite + TypeScript |
| **Backend (Bridge)** | Node.js (Express) |
| **Motor Desktop** | Electron |
| **Banco de Dados** | MongoDB |
| **Utilitários** | yt-dlp, FFmpeg, Adm-Zip |
| **Integração** | Discord.js + Discord RPC |

---

## 🏗️ Arquitetura do Sistema

O projeto funciona através de uma ponte segura entre o cliente e o servidor:

1.  **Frontend (App Electron):** Interface visual de alta performance.
2.  **Ponte API (Squareweb):** Processa as validações de segurança e gera chaves sem expor o banco de dados.
3.  **Banco de Dados (MongoDB):** Armazena de forma criptografada as licenças e permissões.
4.  **Servidor Discord:** Atua como o validador de acesso VIP em tempo real.

---
