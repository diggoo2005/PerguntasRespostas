# PerguntasRespostas
Base de um jogo de perguntas e respostas em Python utilizando a biblioteca Panda


import random

def fazer_perguntas (perguntas):
    perguntas - random.choice(perguntas)
    print (perguntas ['Pergunta'])
    resposta_jogador= input('Sue resposta').strip().lower()
    return resposta_jogador == perguntas['resposta'].lower()


perguntas = [
    {
        "pergunta": "Qual é a capital da França?",
        "resposta": "Paris"
    },
    {
        "pergunta": "Quem escreveu 'Romeu e Julieta'?",
        "resposta": "William Shakespeare"
    },
    {
        "pergunta": "Em que ano ocorreu e independencia do Brasil?",
        "resposta": "Em 1822"
    },
    {
        "pergunta": "Quem foi o primeiro presidente dos Estados Unidos?",
        "resposta": "George Washington"
    },
    {
        "pergunta": "Qual o maior planeta do sistema solar?",
        "resposta": "Jupter"
    },
    {
        "pergunta": "Quem foi o altor da pintura Mona Lisa?",
        "resposta": "Leornado Da Vinci"
    },
    {
        "pergunta": "Qual a maior montanha do mundo?",
        "resposra": "Monte Everest"
    },
    {
        "pergunta": "Em que ano a primeira guerra mundial começou?",
        "resposta": "Em 1918"
    },
    {
        "pergunta": "Quem é o autor da teoria da relatividadde?",
        "resposta": "Albert Einstein"
    },
    {
        "pergunta": "Qual o pais com a maior população do mundo?",
        "resposta": "China"
    }
]

while True:

    acertou = fazer_perguntas(perguntas)

    if acertou:
        print('Parabens, sua resposta está correta.')

    else: 
        print('Desculpa, sua resposta está incorreta')

    continuar = input('Deseja continuar jogando (s/n)').lower()

    if continuar != 's':
        break
