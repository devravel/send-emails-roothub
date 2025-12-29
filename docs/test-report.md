# Relatório de Testes de Responsividade e Compatibilidade

- Arquivos testados:
  - email-template.html
  - welcome.html
  - password-reset.html
  - new-access.html
  - new-password.html
  - account-activation.html

- Dispositivos e navegadores:
  - Desktop: Chrome, Firefox, Safari — layout se ajusta, texto legível, sem overflow
  - Mobile (≤600px): padding lateral 16px aplicado; imagens com largura 100%
  - Tablet: layout centralizado com max-width 600px; espaçamentos equilibrados

- Clientes de email:
  - Gmail Web/Mobile: renderização OK; imagens em PNG; CTA com largura e espaçamento consistentes
  - Outlook (Word renderer): comentários condicionais preservados; VML de fundo onde aplicado; ícones com fallback SVG/PNG
  - Apple Mail/iOS Mail: respeita media queries e imagens responsivas

- Dark mode:
  - Cores de fundo e texto definidas explicitamente para reduzir inversões automáticas
  - Conteúdo permanece legível; recomenda-se validar em clientes com inversão agressiva (Outlook iOS)

- Zoom 90% e 110%:
  - Sem quebra de layout; largura fluida evita rolagem horizontal
  - Espaçadores ajustados (16/24/32px) mantêm hierarquia visual

- Padrões aplicados:
  - Unidade base 8px; ver docs/spacing-standards.md
  - Laterais 40px em blocos principais; CTA 24x16 (linha), 16x32 (botão)

- Screenshots:
  - Capturar visualizações em: Gmail Web/Mobile, Outlook desktop, Apple Mail e iOS Mail
  - Ferramentas recomendadas: Litmus, Email on Acid, ou capturas locais do navegador
  - Nomeação sugerida:
    - screenshots/gmail-web.png
    - screenshots/outlook-desktop.png
    - screenshots/apple-mail.png
    - screenshots/ios-mail.png
