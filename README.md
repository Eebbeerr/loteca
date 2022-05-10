# Projeto Loteca
Este projeto simula uma loteria, onde o usuário 
escolhe seis numeros e sorteia outros seis numeros, 
que no final é verificado a quantidade de números iguais, 
contados como acertos

## Técnologias utilizadas
- **HTML**: Estrutura do site
- **CSS**: Estilização do site
- **_JS_**: Funções do site
- ~~BootStrap~~: Não foi utilizado

## Melhorias Possiveis
1. [X] Subir para GitHubPages
2. [ ] Alterar os Alerts
3. [ ] Utilizar BootStrap
4. [ ] Deixar responsivo

## Disponibilizado em
[GitHubPages](https://eebbeerr.github.io/loteca/)

## Print da tela

| ID | Primeira tela | Segunda tela |
|----|---------------|--------------|
| 1  | Loteca Limpa  | Loteca Preenchida |
| 2  |![tela_loteca_limpa](https://user-images.githubusercontent.com/100212316/161781675-dff634d7-6f2c-4095-8980-eb200265c9ce.png)|![tela_loteca_suja](https://user-images.githubusercontent.com/100212316/161782306-1374be7b-8ba3-40ae-a167-a3441c312762.png)|

## Função Principal
```js:
function sorteio() {
    if (numEsco.lenght == 6) {
        var cont = 0
        numSort = []

        while (cont < 6) {
            let num = Math.random() * 60
            num = Math.ceil(num)
            if (!numSort.includes(num)) {
                numSort[cont] = num
                console.log(numSort)
                cont++
            }
        }
        document.getElementById("sorteados").innerHTML = numSort
        contAcertos()
    }else{
        alert("Faltam número a serem colocados, preencha todos os seis campos.")
    }

}
```

## Comando git
para iniciar o projeto
```bash:
git init
```
