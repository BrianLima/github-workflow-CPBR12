![Image of Yaktocat](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/git-and-git-hub-basics/work-with-the-git-hub-workflow/images/17cdcf6d5135213b505e04eb6c7be614_4-collaborate.png)

# GitHub Workflow - CPBR12
-------------------------------------

Bem vindo ao nosso workshop de [Github Workflow](https://guides.github.com/introduction/flow/) hoje vamos aprender na prática como funciona o fluxo colaborativo de trabalho em programação utilizando o github. 

## 00 - Instalando o Git na sua máquina. 

O passo 0 é instalar o git em sua máquina (caso ainda nao o tenha). É bem provavel que você usuario de **MAC** ou **Linux** não precise instalar pois o Git ja vem de fábrica na sua maquina, mas usuários **Windows** irão ter de baixa-lo. 

Nada tema é bem fácil de [instalar](https://git-scm.com/). 

## 01 - O que é GitHub Workflow ?

Imagine contribuir com um projeto grande, com colaboradores de todas as partes do mundo fazendo alterações (as vezes ao mesmo tempo) em um mesmo arquivo ? Se você ja conhece git sabe que isso causará provavelmente muitos conflitos que podem soar desesperadores e por vezes complicados de resolver. É ai que o Github workflow entra em ação ! \o/ 

O segredo para colaborar e gerir projetos grandes envolvendo código está nesses 3 procedimentos:

 - Branching
 - Pull Request
 - Merge
 

## 02 - 'Leave master alone'

Você provavelmente não quer enviar aquele código que você escreveu as 4:35 da manhã de uma segunda feira para a branch master. Duas coisas podem acontecer:
Você salva o dia, ou no dia seguinte nada funciona mais e você percebe que tudo quebrou ...  e foi **sua culpa**.

Deixa a master branch quieta! Em projetos grandes é preciso ter um monitoramento especial da branch master pois é la que se encontra o código que faz com que a aplicação funcione de forma plena, então se você deseja fazer uma alteração sem quebrar nada, **use branches**. 

#### Branches

Branches como o nome sugere é uma 'ramificação', uma espécie de desvio. Logo cria-se uma cópia do código contido na master em uma ramificação onde você pode fazer o que você desejar sem afetar o código contido la contido. 

Ento mãos a massa:

Inicie um repositório git em uma pasta em seu computador (`git init`) e em seguida baixe ou clone esse repositório:

```
git clone https://github.com/Perkles/github-workflow-CPBR12
```

Agora você tem o código contido na master bem ai na sua maquina. Vamos criar então propriamente a nossa branch.

```
git checkout -b umNomeSignificativo
```

## 03 - Fazendo alteraçes

Vamos todos editar o arquivo **cacilds.md** escolha uma frase randomica e troque algumas letras. 

Após as mudanças vamos commita-las.

```
git add cacilds.md
```

Para adicionar as alteraçes do arquivo ao seu commit

```
git commit -m "Uma mensagem cheia de significado e relevancia"
```

Para descrever as alteraçes feitas no arquivo.

```
git push origin umNomeSignificativo
```

Observe aqui que você esta enviando as alteraçes para a branch `umNomeSignificativo` e não para a `master`.


