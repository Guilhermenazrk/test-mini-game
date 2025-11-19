# test-mini-game
É um mini game sobre escolha de numeros extremamente simples, apenas para prática.
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <script>

        alert("Bem-Vindo ao jogo de ESCOLHA QUALQUER NUMERO ENTRE 1000-10000")
        let round1 = parseInt(prompt("Digite a pontuação a sua primeira rodada"))
        let round2 = parseInt(prompt("Digite a pontuação a sua segunda rodada"))
        const bonus = 1500
        const penalty = 1500
        let totalScore = (round1 + round2) * 2;





        if (round1 < 1000 || round2 < 1000) {





            console.log("Não vale trapacear, apenas numeros entre 1000-10000! Atualize a página e tente novamente!")


        } else if (round1 > 10000 || round2 > 10000) {


            console.log("Não vale trapacear, apenas numeros entre 1000-10000! Atualize a página e tente novamente!")


        } else {

            console.log("VAMOS AOS JOGOS!")
            console.log("")






            if (round1 > 5000) {
                round1 = round1 + penalty
                console.log(`Rodada 1: O numero que você escolheu (${round1}) é muito alto, você foi punido!
                +${penalty}!`)
                console.log("")

            } else {

                round1 = round1 - bonus
                console.log(`Rodada 1: Você passou tranquilo nessa rodada! Recebeu um bonus! -${bonus}`)
                console.log("")
            }
            if (round2 > 5000) {
                round2 = round2 + penalty
                console.log(`Rodada 2: O numero que você escolheu (${round2}), é muito alto, você foi punido!
                +${penalty}!`)
                console.log("")

            } else {

                round2 = round2 - bonus
                console.log(`Rodada 2: Você passou tranquilo nessa rodada! Recebeu um bonus! -${bonus}`)
                console.log("")
            }

            if (totalScore > 10000) {


                console.log("Você falhou! Não pode ser maior que 10000! Tente novamente!")






            }

            else {

                console.log("Parabéns! Você ganhou o jogo!")



            }











        }
























    </script>

</body>

</html>
