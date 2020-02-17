# STUDIO TEST MEDICINA


import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as np


##BARI 2016

df_bari_2016 = pd.read_csv("Desktop/2016/bari_2016.csv", sep=" ", names = ['logica','cultura_generale',"biologia","chimica","fisica_matematica","Totale",""])
df_bari_2016.drop([''], axis='columns', inplace=True)
df_bari_2016.dropna(inplace=True)


#Inserimento colonna bari
bari_2016=[]
for i in range(len(df_bari_2016)):
    bari_2016.append("Bari")

df_bari_2016["Regione"]=bari_2016


#inserimento promosso

bari_2016_promosso =[]

for i in range(len(df_bari_2016)):
    try:
        if df_bari_2016["Totale"][i] > punteggio_min_bari_2016:
         bari_2016_promosso.append(1)
        else:
         bari_2016_promosso.append(0)
    except KeyError:
        print("index {} missing".format(i))
        pass

df_bari_2016["promosso"]=bari_2016_promosso

##BOLOGNA 2016

df_bologna_2016 = pd.read_csv("Desktop/2016/bologna_2016.csv", sep=" ", names = ['logica','cultura_generale',"biologia","chimica","fisica_matematica","Totale",""])
df_bologna_2016.drop([''], axis='columns', inplace=True)
df_bologna_2016.dropna(inplace=True)

print()

#Inserimento colonna bologna
bologna_2016=[]
for i in range(len(df_bologna_2016)):
    bologna_2016.append("Bologna")

df_bologna_2016["Regione"]=bologna_2016

#inserimento promosso

bologna_2016_promosso =[]

for i in range(len(df_bologna_2016)):
    try:
        if df_bologna_2016["Totale"][i] > punteggio_min_bologna_2016:
         bologna_2016_promosso.append(1)
        else:
         bologna_2016_promosso.append(0)
    except KeyError:
        print("index {} missing".format(i))
        pass

df_bologna_2016["promosso"]=bologna_2016_promosso


##BRESCIA 2016

df_brescia_2016 = pd.read_csv("Desktop/2016/Brescia_2016.csv", sep=" ", names = ['logica','cultura_generale',"biologia","chimica","fisica_matematica","Totale",""])
df_brescia_2016.drop([''], axis='columns', inplace=True)
df_brescia_2016.dropna(inplace=True)

print()

#Inserimento colonna brescia
brescia_2016=[]
for i in range(len(df_brescia_2016)):
    brescia_2016.append("Brescia")

df_brescia_2016["Regione"]=brescia_2016

#inserimento promosso

brescia_2016_promosso =[]

for i in range(len(df_brescia_2016)):
    try:
        if df_brescia_2016["Totale"][i] > punteggio_min_brescia_2016:
         brescia_2016_promosso.append(1)
        else:
         brescia_2016_promosso.append(0)
    except KeyError:
        print("index {} missing".format(i))
        pass

df_brescia_2016["promosso"]=brescia_2016_promosso


##CAGLIARI 2016

df_cagliari_2016 = pd.read_csv("Desktop/2016/Cagliari_2016.csv", sep=" ", names = ['logica','cultura_generale',"biologia","chimica","fisica_matematica","Totale",""])
df_cagliari_2016.drop([''], axis='columns', inplace=True)
df_cagliari_2016.dropna(inplace=True)

print()

#Inserimento colonna cagliari
cagliari_2016=[]
for i in range(len(df_cagliari_2016)):
    cagliari_2016.append("Cagliari")

df_cagliari_2016["Regione"]=cagliari_2016

#inserimento promosso

cagliari_2016_promosso =[]

for i in range(len(df_cagliari_2016)):
    try:
        if df_cagliari_2016["Totale"][i] > punteggio_min_cagliari_2016:
         cagliari_2016_promosso.append(1)
        else:
         cagliari_2016_promosso.append(0)
    except KeyError:
        print("index {} missing".format(i))
        pass

df_cagliari_2016["promosso"]=cagliari_2016_promosso



##CATANIA 2016

df_catania_2016 = pd.read_csv("Desktop/2016/Catania_2016.csv", sep=" ", names = ['logica','cultura_generale',"biologia","chimica","fisica_matematica","Totale",""])
df_catania_2016.drop([''], axis='columns', inplace=True)
df_catania_2016.dropna(inplace=True)

print()

#Inserimento colonna bologna
catania_2016=[]
for i in range(len(df_catania_2016)):
    catania_2016.append("Catania")

df_catania_2016["Regione"]=catania_2016

#inserimento promosso

catania_2016_promosso =[]

for i in range(len(df_catania_2016)):
    try:
        if df_catania_2016["Totale"][i] > punteggio_min_catania_2016:
         catania_2016_promosso.append(1)
        else:
         catania_2016_promosso.append(0)
    except KeyError:
        print("index {} missing".format(i))
        pass

df_catania_2016["promosso"]=catania_2016_promosso





