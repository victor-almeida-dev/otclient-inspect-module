# UI Inspector (OTClient)

Tutorial rapido para usar o modulo `client_ui_inspector` no OTClient.

## O que ele faz
- Ao passar o mouse sobre um widget, mostra um tooltip com o caminho do widget
  e o `id`.
- Aplica um contorno temporario no widget enquanto o inspector esta ativo.

## Como usar
1) Inicie o cliente normalmente.
2) Ative o inspector pelo botao no top menu (icone de debug) chamado
   "UI Inspector".
3) Passe o mouse sobre qualquer widget.

Exemplo de tooltip:
```text
MainWindow > Button > Label
id: submit
```

## Atalho
- `Ctrl+Alt+I` para ligar/desligar o inspector.

## Desativar
- Clique no botao "UI Inspector" novamente ou use o atalho.

## Personalizacao
No arquivo `modules/client_ui_inspector/ui_inspector.lua`:
- `HIGHLIGHT_COLOR` controla a cor do contorno.
- `HIGHLIGHT_WIDTH` controla a espessura do contorno.

## Observacoes
- O contorno original do widget e restaurado automaticamente ao mudar o hover
  ou desativar o inspector.
