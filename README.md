[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/tro2Z-6l)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=23170879&assignment_repo_type=AssignmentRepo)
# Lab 01: Lógica de Programação com Blockly 🐢

Bem-vindo(a) à sua atividade prática de Lógica Computacional! Siga os passos abaixo para completar o desafio.

**Nome do Aluno:** [Antonio Gabriel Reis do Valle Perez de Mello]
**Matrícula:** [20261100153]
---

## 🎯 Objetivo
Demonstrar capacidade de resolução de problemas algorítmicos completando o **Nível 10** do jogo da Tartaruga (Turtle). 

## 📝 Instruções

**Passo 1: Jogue e Resolva**

Acesse o jogo da Tartaruga no [Blockly Games](https://blockly.games/turtle) e complete as etapas até vencer o **nível 10**.

**Passo 2: Registre sua Solução**

Tire um screenshot (captura de tela) da sua solução final (mostrando os blocos que você usou para passar do nível 10). Faça o upload (envio) dessa imagem **dentro da pasta /imagens** que já existe neste repositório.

**Passo 3: Explique sua Estratégia**

Escreva um pequeno texto explicando qual foi a sua linha de raciocínio e a estratégia que você usou para resolver o nível 10.
*(Exemplo: "Criei uma função para desenhar uma estrela, depois usei um loop para repetir essa função 3 vezes girando 120 graus.")*

**Passo 4: Pergunta Desafio**

Olhando para os blocos que você usou para resolver o jogo no nível 10, imagine que o problema mudou. A sua nova missão agora é desenhar um **hexágono regular** (uma figura geométrica de 6 lados iguais) e repetir esse hexágono **4 vezes**, formando um padrão circular (como as pétalas de uma flor).

**Sem precisar montar os blocos** no jogo, responda por escrito:
* **A)** Quantas repetições o seu loop principal (que desenha o hexágono) precisaria ter e qual seria o ângulo (em graus) que a tartaruga deve virar a cada linha desenhada?
* **B)** Depois de desenhar um hexágono completo, qual deve ser o ângulo de giro (em graus) antes de começar a desenhar o próximo hexágono, para que os 4 fiquem distribuídos igualmente em um círculo completo?
* **C)** Explique brevemente qual foi a lógica (ou o cálculo) que você usou para descobrir os ângulos das questões A e B.

---

## ✍️ Suas Respostas

*(Edite este arquivo e escreva suas respostas dos Passos 3 e 4 aqui embaixo. Lembre-se de colocar a imagem do Passo 2 dentro da pasta **/imagens** deste repositório)*

## 2. Evidência Visual (Screenshot)
*Suba o screenshot da sua solução final (onde aparece "Você resolveu este nível!") para a pasta **/imagens** deste repositório.*

## 3. Estratégia Utilizada
*Explique com suas palavras como você resolveu o problema. Qual foi a lógica?*
> Eu comecei o código mudando a cor da tartaruga para amarelo, visto que as estrelas são amarelas. Em seguida, eu criei uma função repeat que contém a função de mover a tartaruga e mudar sua angulação, criando assim uma estrela ao final do ciclo desse loop. Esse repeat, de criar uma estrela, está dentro de um repeat maior, que repetirá a criação da estrela 3 vezes junto com a locomoção da tartaruga para as posições das outras 2 estrelas que devem ser desenhadas. Então, ao término das 3 estrelas o repeat maior terminará e o processo da criação da Lua crescente iniciará.
Primeiro, eu movi a tartaruga para o centro de onde seria a parte iluminada da lua (considerando o centro dela como o centro da circunferência original dela). Em seguida, Eu fiz um repeat de 360 vezes que fará a tartaruga desenhar um círculo branco. Após terminar o círculo branco, bastou fazer a parte escura da lua. Para isso, eu movi a tartaruga um pouco para cima e para a direita, posicionando ela para onde seria o centro do círculo preto imaginário que cria a sombra na lua. Por fim, bastou colocar na cor preta e utilizar o mesmo repeat de criação de um círculo, completando o nível.

*Extra: Nível 10 - criação livre (logo da CC UENF). Qual foi a minha lógica utilizada?*
> Primeiro, eu desenhei um grande fundo branco a partir da função "repeat n times", fazendo um grande círculo branco e preenchendo o fundo. Após isso, eu foquei em desenhar o "C" maior e o "C" menor de cores azuis presentes na logo. Logo, decidi fazer dois círculos, um maior e um menor, um dentro do outro. Junto a isso, fiz círculos brancos intermediários, criando um espaço entre os dois círculos azuis e os tornando circunferências. Eu criei os círculos a partir do conhecimento obtido dos níveis anteriores do jogo da tartaruga, através das funções básicas apresentadas (ou seja: "move", "turn", "pen", "set color to",...). Em seguida, decidi finalizar os dois "C" criando uma abertura do lado direito deles. Para isso, eu novamente utilizei a estratégia de usar a cor branca, como se eu estivesse apagando uma parte do desenho, mas na verdade, estou apenas pintando com a cor do fundo por cima. Para isso, eu utilizei a função "repeat n times" novamente, com a ideia similar de criar um círculo. No entanto, dessa vez eu defini esse looping com menos repetições para fazer esta pequena abertura nas circunferências. Agora, finalizado o "C" maior e o "C" menor, basta escrever as palavras da logo, no caso: "CIÊNCIA DA"; "COMPUTAÇÃO"; "UENF". Nessa situação, eu fui movendo a tartaruga para as regiões corretas e escrevi utilizando a função "print" (eu achei as regiões corretas através de tentativa e erro). Além disso, usei a função "font" para trocar a fonte e o tamanho das letras, tornando-as mais idênticas com as da logo.

## 4. Desafio:
**A)** O loop principal (que cria um hexágono) deve ter 6 repetições, visto que um hexágono possui 6 lados. E a tartaruga deve virar 60° para um dos lados.
  
**B)** Após desenhar um hexágono completo, o ângulo utilizado para criar um círculo de hexágonos (no padrão de uma flor) é o ângulo de 90° graus (para qualquer um dos lados).
  
**C)** A lógica que eu usei para achar o ângulo utilizado no item "A)" foi: a tartaruga deveria virar um ângulo de 60° a cada linha desenhada, pois, considerando um hexágono regular, cada ângulo interno possui 120°. A tartaruga indo reto é como se fosse 180°, e desviando 60° para um lado, cria-se entre as linhas um ângulo de 120° (180°-60°=120°).
Já a lógica utilizada para achar o ângulo do item "B)" foi: Visto que queremos formar um círculo de hexágonos, devemos fazer uma rotação de forma proporcional com a quantidade de hexágonos que desenharemos com o ângulo de uma circunferência (360°), formando um círculo. Logo, 360°/4 = 90°.

---
