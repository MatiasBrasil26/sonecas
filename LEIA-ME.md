# App Sonecas 🌙

App simples para acompanhar as sonecas e as mamadas do bebê no iPhone.

**Endereço do app:** https://matiasbrasil26.github.io/sonecas/

## Como instalar no iPhone (uma vez só)

1. No iPhone, abra o **Safari** (precisa ser o Safari, não o Chrome nem o Instagram).
2. Digite o endereço acima e abra.
3. Toque no botão **Compartilhar** (o quadrado com a seta para cima, embaixo da tela).
4. Role a lista e toque em **Adicionar à Tela de Início**.
5. Confirme o nome "Sonecas" e toque em **Adicionar**.

Pronto: o ícone da lua aparece na tela de início e o app abre em tela cheia, como qualquer outro app. Depois da primeira vez, abre até sem internet.

> Sempre abrir pelo **ícone da tela de início**. Os registros feitos pelo ícone ficam separados dos feitos no Safari.

## Como usar

- **🌙 Dormiu**: toque quando o bebê dormir. O relógio mostra há quanto tempo está dormindo.
- **☀️ Acordou**: toque quando acordar. A soneca vai para a lista do dia.
- **🍼 Registrar mamada**: escolha peito esquerdo, direito ou mamadeira. O app já sugere o peito do outro lado da última mamada. Duração, ml e observações são opcionais.
- **Corrigir ou anotar**: toque em qualquer item da lista para mudar os horários, escrever uma observação (ex.: "dormiu no colo") ou excluir.
- **Esqueceu de apertar?** Use "+ Soneca esquecida" ou "+ Mamada esquecida".
- **Dias anteriores**: use as setas ‹ › ao lado de "Hoje".
- No topo da lista: total de sono do dia, número de sonecas e de mamadas.

## Onde ficam os dados

Os registros ficam guardados **só no iPhone dela** (nada vai para a internet).
Se o app for apagado da tela de início, ou se o iPhone for trocado, os registros se perdem.
Por isso, de vez em quando, toque em **Cópia de segurança → Salvar cópia** e guarde o arquivo
(no app Arquivos/iCloud ou mandando para si mesma pelo WhatsApp).
Para recuperar: **Cópia de segurança → Restaurar de uma cópia**.

## Para quem for mexer no código

- `index.html`: o app inteiro (tela, estilo e lógica).
- `sw.js`: faz o app abrir sem internet.
- `manifest.json`, `icon-*.png`, `icon.svg`: nome e ícone.
- Publicado pelo GitHub Pages (repositório `MatiasBrasil26/sonecas`). Para atualizar: alterar os arquivos, `git commit` e `git push`; o iPhone pega a versão nova na próxima vez que abrir com internet.
