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
- **☀️ Acordou**: toque quando acordar. A soneca vai para a lista do dia, e o app mostra **o horário da próxima soneca**, calculado pela idade do Emanuel (nascido em 16/09/2026) e pela tabela de janelas de sono da NUK. O aviso fica verde quando chega a hora de dormir e laranja quando passa da janela.
  Para mudar o nome ou a data de nascimento: no `index.html`, linha `const BEBE = ...` (o mês começa em 0: setembro = 8).
- **⏸️ Despertou rapidinho (pausar)**: durante a soneca, se o bebê acordar um pouco, toque aqui. A contagem do sono para.
  - **🌙 Voltou a dormir**: retoma a contagem. Pode pausar quantas vezes precisar na mesma soneca.
  - **☀️ Acordou de vez**: se ele não voltar a dormir, a soneca termina no horário em que ele despertou, e a próxima soneca é calculada a partir daí.
  - A duração da soneca, o total do dia e o relatório da semana contam **só o sono real**, sem os despertares. A lista mostra quantos despertares houve e quanto tempo duraram. Ao tocar na soneca, dá para apagar os despertares, se tiver sido engano.
- **🍼 Registrar mamada**: escolha peito esquerdo, direito ou mamadeira. O app já sugere o peito do outro lado da última mamada. Dá para anotar quantos ml ele mamou em qualquer mamada (peito ou mamadeira); o resumo do dia mostra o total de ml e o relatório da semana mostra a média por dia. Duração, ml e observações são opcionais.
- **Corrigir ou anotar**: toque em qualquer item da lista para mudar os horários, escrever uma observação (ex.: "dormiu no colo") ou excluir.
- **Esqueceu de apertar?** Use "+ Soneca esquecida" ou "+ Mamada esquecida".
- **Dias anteriores**: use as setas ‹ › ao lado de "Hoje".
- No topo da lista: total de sono do dia, número de sonecas e de mamadas.
- **📊 Relatório da semana** (de segunda a domingo): gráfico com as horas de sono de cada dia, médias de sono, sonecas e mamadas por dia, soneca mais longa, total de ml de mamadeira e comparação com a semana anterior. As setas ‹ › mostram as semanas passadas. O dia de hoje aparece no gráfico, mas fica fora das médias até terminar.
  O botão **Compartilhar** gera uma imagem do relatório para mandar no WhatsApp ou mostrar ao pediatra.

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
