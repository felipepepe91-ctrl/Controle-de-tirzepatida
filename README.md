# 💉 Controle & Previsão de Estoque de Tirzepatida

Sistema web moderno, responsivo e intuitivo desenvolvido para o gerenciamento de estoque, cálculo de dosagens em Unidades Internacionais (UI), acompanhamento de peso de pacientes, projeção temporal de esgotamento e sincronização em tempo real com o Google Drive (Google Apps Script).

---

## 🚀 Principais Funcionalidades

- **📊 Dashboard Interativo:** Visão geral com cartões de status, contagem de seringas/ampolas e projeção de consumo baseada na rotina semanal dos pacientes.
- **🚨 Alerta de Estoque Crítico:** Sistema de aviso inteligente que sinaliza quando o estoque de seringas ou ampolas atinge o limite de segurança das **últimas 3 aplicações**, prevenindo que alguém fique sem tomar.
- **📐 Simulador Visual de Seringa:** Desenho interativo de seringa (50 UI e 100 UI) com marcação exata da dosagem em miligramas (`mg`) e conversão automática para Unidades Internacionais (`UI`), além de suporte a diferentes concentrações de frascos.
- **👥 Gestão de Perfis:** Cadastro de pacientes/usuários com definição de dose semanal e dia de aplicação.
- **⚖️ Evolução de Peso:** Acompanhamento gráfico e em tabela da variação de peso registrada a cada aplicação.
- **📦 Gestão de Estoque e Entradas:** Controle detalhado do saldo de ampolas (`mg` restantes) e seringas por tipo, com histórico completo de abastecimentos.
- **☁️ Sincronização em Nuvem (Google Drive):** Conexão via API do Google Apps Script para manter dados sincronizados entre múltiplos dispositivos em tempo real. Possui botão flutuante exclusivo para administradores no canto superior direito com indicador da última sincronização.
- **📄 Exportação de Relatórios:** Exportação imediata de dados para planilhas do Excel (`.xlsx`) e relatórios em PDF.
- **🔒 Modo Administrador & Usuário:** Alternância segura de perfis protegida por senha para impedir alterações acidentais por usuários comuns.

---

## 💻 Tecnologias Utilizadas

Este projeto foi construído em **arquivo único (HTML/JS/CSS)** utilizando bibliotecas via CDN, facilitando a hospedagem estática (como GitHub Pages) sem necessidade de servidores complexos:

- **[Tailwind CSS](https://tailwindcss.com/)** – Estilização moderna e responsiva.
- **[Chart.js](https://www.chartjs.org/)** – Gráficos interativos de projeção de estoque e evolução de peso.
- **[SheetJS (XLSX)](https://sheetjs.com/)** – Exportação de dados para Excel.
- **[jsPDF & autoTable](https://github.com/parallax/jsPDF)** – Geração de relatórios em PDF.

---

## 🔧 Como Usar / Instalar

1. Clone o repositório ou faça o download do arquivo `index.html`.
2. Abra o arquivo `index.html` em qualquer navegador web moderno.
3. Para gerenciar estoque e cadastros, clique no botão **"Login Admin"** no cabeçalho e digite a senha padrão:
   - **Senha Admin:** `admin123` *(Você pode alterá-la diretamente no código JavaScript)*.

---

## ☁️ Configuração da Nuvem (Google Drive / Apps Script)

Para habilitar a persistência e compartilhamento em nuvem:
1. Crie um projeto no [Google Apps Script](https://script.google.com/).
2. Cole o script de manipulação de requisições POST/GET conectado a uma planilha do Google Sheets.
3. Insira a URL gerada do Web App na configuração do sistema (via modal de configuração do Drive ou diretamente na constante `DEFAULT_DRIVE_URL` no código).

---

## 👤 Autor

Desenvolvido por **Felipe Lima dos Santos**.
