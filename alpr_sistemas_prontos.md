## ALPR - Sistemas prontos

### UTFPR - An Efficient and Layout-Independent Automatic License Plate Recognition System Based on the YOLO Detector

* Aplicação usando Darknet
* Detecção de veículo com modelo baseado em YOLOv2
* Detecção da placa com rede modificada de Fast YOLOv2

* For example, all Brazilian LPs have seven characters: three letters and four digits (in that order)

* The models adapted are YOLOv2 [27], Fast-YOLOv2 and CR-NET [6], which is an architecture inspired by YOLO for character detection and recognition.

#### Vehicle detection

* YOLOv2 modificada em vez de Yolov3 devido ao custo computacional. Variantes do Fast YOLOv2 veículos parcialmente cobertos (oclusão).
* Input size de 416 x 416 para 448 x 288 após testes com tamanhos de 448 × 288 até 832 × 576 pixels. Imagens geralmente têm largura maior que altura.
* Número de classes = 2 (carros e motos)    A = 5   Filtros na última camada convolucional = 35 ((2 + 5) x 5))
* Resultados melhores para duas classes em vez de apenas uma.
* We exploit various data augmentation strategies, such as flipping, rescaling and shearing, to train our network.

* https://web.inf.ufpr.br/vri/publications/layout-independent-alpr
