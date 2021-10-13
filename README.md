# SignLanguageRecognition
Repository del mio progetto di Tesi Magistrale per l'Università Roma Tre.

In questo progetto vengono usate reti neurali deep per il riconoscimento della Lingua dei Segni. In particolare vengono usati due approcci: il primo utilizza un'architettura Convolutional Neural Network (CNN) combinata con un'architettura Recurrent Neural Network (RNN); il secondo utilizza un approccio hand pose estimation proposto dalla libreria MediaPipe di Google sempre utilizzando come modello CNN e RNN.

## Dataset 
Nella cartella **dataset** si trova il dataset utilizzato in questo progetto, l'alfabeto della lingua dei segni americana (ASL), già convertito in immagini. Ma è possibile applicare i modelli anche ad altri dataset come il [WLASL](https://github.com/dxli94/WLASL).

## Operazioni sui video
Nella cartella **input_functions** si trovano le funzioni ausiliari da sottoporre ai video in input. In particolare con **videos_to_frames** vengono trasformati tutti i video di input in immagini e con la funzione **split** le immagni vengono divise in train e test set (utili per il modello CNN-RNN).

## Modelli 
Vengono costruiti i due modelli, con tutte le operazioni preliminari sull'input, la costruzione, l'addestramento e la valutazione delle prestazioni.
