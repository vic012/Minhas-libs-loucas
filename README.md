# coding=utf-8

# nesse momento o jogador receberá as boas vindas!
print 'Olá, Seja bem-vindo ao jogo: MAD-LIBS!'
print '-' * 40
print '-' * 40

# os níveis disponíveis para o jogo.
niveis = ['iniciante', 'amador', 'profissional']

# as frases de cada nível.
frase_nivel_iniciante = "Água __0__ pedra __1__ tanto __2__ até que __3__."
frase_nivel_amador = "Em __0__ de cego __1__ tem __2__ é __3__."
frase_nivel_profissional = "De __0__ e de __1__ todo __2__ tem um __3__."

# as respostas corretas de cada nível.
reposta_iniciante = ['mole', 'dura', 'bate', 'fura']
resposta_amador = ['terra', 'quem', 'olho', 'rei']
resposta_profissional = ['medico', 'louco', 'mundo', 'pouco']

# Lista das frases definidas por nível.
frases = [frase_nivel_iniciante, frase_nivel_amador, frase_nivel_profissional]

# Lista das respostas definidas por nível.
respostas = [reposta_iniciante, resposta_amador, resposta_profissional]

# Números de erros para cada nível.
chances = ['5', '3', '1']

# O usuário vai escolher um nível nesse momento.
iniciante = frases[0]
amador = frases[1]
profissional = frases[2]
'''O nível será digitado pelo usuário, o programa deve esperar o
jogador digitar o nível que deseja jogar, após p jogador selecionar
um nivel válido o programa defe retornar a pergunta conforme o nível
selecionado, caso não, o programa deve mostrar uma mensagem
dizendo a ele que precisa informar um nivel válido'''

escolha_nivel = raw_input('Para iniciar, escolha uma faixa de dificuldade: ( iniciante | amador | profissional):').lower()

if escolha_nivel == niveis[0]:
    print iniciante
else:
    if escolha_nivel == niveis[1]:
        print amador
    else:
        if escolha_nivel == niveis[2]:
            print profissional
        else:
            print 'Insira um nivel válido!'
