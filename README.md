# Phase-1-Code
The code for the phase 1 Project in case the replit is lost 
unit=input("Enter unit")
if unit =="Km":
  Km=int(input("Enter Km"))
  MPH=Km*.62 
  print(MPH)
elif unit=="Kg":
  Kg=int(input("Enter Kg"))
  LBS=Kg*.45
  print(LBS)
elif unit == "cel":
  cel=int(input("Enter cel"))
  fer=cel*32
  print(fer)
else:
  print("Please insert proper unit :( ")

import pygame 
Black=(0,0,0)
White=(255,255,255)
Red=(255,0,0)
Green=(0,255,0)
Blue=(0,0,255)
Grey=(150,150,150)
Purple=(102,0,102)
Yellow=(255,255,0)
pygame.display.set_mode(size=(0, 0), flags=0, depth=0, display=0)
scn_width=500
scn_height=640
screen=pygame.display.set_mode((scn_width,scn_height))
screen.fill(White)
pygame.draw.rect(screen,Yellow,[150,105,200,110],0)
pygame.draw.circle(screen,Purple,[20,20],100)
pygame.init()
print(pygame.font.get_fonts())
font = pygame.font.SysFont("freesans", 25, )
text = font.render("Your unit has been converted",True,Black)
tw = text.get_width()
th = text.get_height()
screen.blit(text, [0, 0])
screen.blit(text, [scn_width / 2 -tw / 2, scn_height / 2 -th / 2])
screen.blit(text, [scn_width -tw, scn_height -th])
pygame.display.flip()           

''''
import RPi.GPIO as GPIO
import time 
GPIO.setmode(GPIO.BCM)
GPIO.setwarnings(False)
GPIO.setup(19,GPIO.OUT)
for x in range (10):
    GPIO.output(19,GPIO.HIGH)
    time.sleep(1)
    GPIO.output(19,GPIO.LOW)
    time.sleep(1)
    '''
