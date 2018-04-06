# nibbas.gates

import pygame
import os
import pathlib
import join


from os import *
from pathlib import *
from join import *
from pygame import *




def main():
    escritorio = image.load(os.path.join('Wl.png'))

    pygame.init()
    tela = pygame.display.set_mode([1366, 768])
    pygame.display.set_caption("Vsg.select(funcionario)")
    relogio = pygame.time.Clock()

    ret = pygame.Rect(10, 10, 45, 45)

    sair = False

    while sair != True:
        for event in pygame.event.get():
            if event.type == pygame.QUIT:
                sair = True

            if event.type == pygame.MOUSEBUTTONDOWN:
                ret = ret.move(0, 10)

        tela.blit(escritorio, (0, 0))
        pygame.display.update()

    pygame.quit()


main()



