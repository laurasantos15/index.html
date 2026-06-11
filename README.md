<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
* {
    box-sizing: border-box;
}
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #f8eeee;
    color: #3
let tamanho = 18;
function aumentarTexto() {
    tamanho += 2;
    document.body.style.fontSize = tamanho + "px";
}
function diminuirTexto() {
    if (tamanho > 12) {
        tamanho -= 2;    document.body.style.fontSize = tamanho + "px";
    }
}
function ativarContraste() {
  document.body.classList.toggle("contraste");
}