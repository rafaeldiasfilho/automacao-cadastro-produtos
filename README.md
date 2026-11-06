# Automação de cadastro de produtos

Script em Python que lê uma planilha de produtos e cadastra cada um em um sistema web, controlando o mouse e o teclado como se fosse uma pessoa digitando.

## Como funciona

1. Lê o arquivo `produtos_ficticios.xlsx`
2. Para cada produto, copia cada campo (nome, descrição, categoria, código, peso etc.)
3. Clica no campo certo da tela, cola o valor com `pyautogui` e salva o cadastro

## Atenção

Os cliques usam coordenadas fixas da tela onde o script foi feito. Para rodar em outro computador, é preciso trocar as coordenadas no `app.py` pelas posições dos campos na sua tela. Dá para descobri-las com `pyautogui.position()`.

## Como rodar

```bash
pip install -r requirements.txt
python app.py
```
