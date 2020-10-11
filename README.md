# PANDA_projekt
Projektarbete i deep learning

Koden är för PANDA, med syftet att kunna ange ISUP-gradering genom att analysera biopsibilder.

PANDA_DataProcessing.ipynb innehåller dataprocessing-delen, där bilderna läses in från .tiff-bilderna, nya bilder bestående av N sub-bilder genereras, och pixelvärderna sparas
som 32-bitars flytttal och normeras så att de skall passa ResNetV2.

PANDA_GeneratorTraining_Small är träningskoden för bilderna med N=16. Denna innehåller fem modeller samt resultaten för varje träningsepok, samt en utvärdering mot testsettet för 
den modell som gav bäst utvärderingsmått mot valideringssettet.

PANDA_GeneratorTraining_Large är träningskoden för bilderna med N=100. Denna innehåller sex modeller samt resultaten för varje träningsepok, samt en utvärdering mot testsettet för 
den modell som gav bäst utvärderingsmått mot valideringssettet.
