# The Legend of Zelda — Port nativo para Mega Drive

[English](README.md) · [FAQ](FAQ.md) · [Ajuda](HELP.md) · [Compilação](BUILD.md) · [Histórico](CHANGELOG.md) · [Roadmap](ROADMAP.md)

## Sobre o meu projeto

Comecei este projeto com o objetivo de trazer o The Legend of Zelda original de NES, lançado em 1986, para o Mega Drive / Genesis. Quero preservar a experiência e a jogabilidade do original, adaptando o jogo à arquitetura do console de 16 bits da Sega, sem utilizar um emulador de NES.

O jogo executa código 68000 nativamente. Utilizo tradução estática do código PRG0 e rotinas específicas para vídeo, controles e outros recursos do Mega Drive. O áudio utiliza PSG, YM2612 e Z80 para os efeitos DMC reservados, com aproximações do comportamento da APU original.

## Estado atual

Minha versão de referência reúne melhorias de movimentação, rolagem de cenários, renderização das dungeons, áudio, título e correções do menu de pausa. Ainda estou trabalhando na validação completa das duas quests, dos saves, do desempenho e do equilíbrio sonoro.

## Testes em hardware real

Testei o port no meu Mega Drive 1 japonês original (NTSC-J), utilizando um EverDrive V3 Pro. Também utilizo o BlastEm durante o desenvolvimento. Pretendo ampliar os testes para outros modelos, regiões e configurações. Ainda não considero a compatibilidade integral certificada.

## Conversor web

Meu [conversor web](https://sa-m-be.github.io/Zelda-1-MegaDrive-Converter/) foi desenvolvido para gerar o port localmente a partir de uma ROM original compatível de NES, sem instalação de programas ou SDK. Validei o motor de conversão direta fora do navegador comparando o resultado com minha ROM de referência. Ainda falta validar a integração completa no navegador e revisar a distribuição. Quando estiver pronto para uso, selecione a ROM de NES, clique em **Generate Mega Drive ROM** e depois em **Download PORT**.

## Como ajudar

Se encontrar algum problema, abra uma Issue com a versão, o ambiente de teste e os passos para reproduzir o erro. Sugestões e contribuições técnicas são bem-vindas.

## Créditos e direitos autorais

Mantenho este projeto independente pela conta [sa-m-be](https://github.com/sa-m-be). Consulte [CREDITS.md](CREDITS.md). O projeto não possui vínculo com a Nintendo ou a Sega. Os direitos do jogo original pertencem aos respectivos titulares. Não disponibilizo ROMs completas neste repositório de documentação e estou revisando os direitos de distribuição dos fontes e patches.
