# The Legend of Zelda — Port nativo para Mega Drive

[English](README.md) · [FAQ](FAQ.md) · [Ajuda](HELP.md) · [Compilação](BUILD.md) · [Histórico](CHANGELOG.md) · [Roadmap](ROADMAP.md)

## Sobre o meu projeto

Comecei este projeto com o objetivo de trazer o The Legend of Zelda original de NES, lançado em 1986, para o Mega Drive / Genesis. Quero preservar a experiência e a jogabilidade do original, adaptando o jogo à arquitetura do console de 16 bits da Sega, sem utilizar um emulador de NES.

O jogo executa código 68000 nativamente. Utilizo tradução estática do código PRG0 e rotinas específicas para vídeo, controles e outros recursos do Mega Drive. O áudio utiliza PSG, YM2612 e Z80 para os efeitos DMC reservados, com aproximações do comportamento da APU original.

## Estado atual

Minha versão de referência é a **MD35**. Ela reúne melhorias de movimentação, rolagem de cenários, renderização das dungeons, áudio, título e correções do menu de pausa. Ainda estou trabalhando na validação completa das duas quests, dos saves, do desempenho e do equilíbrio sonoro.

## Testes em hardware real

Testei o port no meu Mega Drive 1 japonês original (NTSC-J), utilizando um EverDrive V3 Pro. Também utilizo o BlastEm durante o desenvolvimento. Pretendo ampliar os testes para outros modelos, regiões e configurações. Ainda não considero a compatibilidade integral certificada.

## Conversor web

Estou desenvolvendo um conversor para que seja possível selecionar a própria ROM original do NES e gerar a versão de Mega Drive diretamente no navegador, sem instalar programas. O protótipo atual valida a ROM de NES e atualiza uma base MD13 existente para MD35. A compilação completa a partir do NES ainda está em desenvolvimento.

## Como ajudar

Se encontrar algum problema, abra uma Issue com a versão, o ambiente de teste e os passos para reproduzir o erro. Sugestões e contribuições técnicas são bem-vindas.

## Créditos e direitos autorais

Mantenho este projeto independente pela conta [sa-m-be](https://github.com/sa-m-be). Consulte [CREDITS.md](CREDITS.md). O projeto não possui vínculo com a Nintendo ou a Sega. Os direitos do jogo original pertencem aos respectivos titulares. Não disponibilizo ROMs completas neste repositório de documentação e estou revisando os direitos de distribuição dos fontes e patches.
