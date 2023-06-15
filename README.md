# Perceptron-Diagnóstico de doença cardíaca

## Diagnóstico de Problemas Cardíacos
### Introdução: 

Este projeto tem como objetivo desenvolver um modelo de diagnóstico médico para identificar a existência de problemas cardíacos em pacientes, utilizando uma base de dados médicos contendo informações de exames realizados. A análise desses dados pode auxiliar na detecção precoce de doenças cardíacas e na tomada de decisões médicas.

### Pré-processamento dos dados: 

Antes da construção do modelo, realizamos um pré-processamento dos dados. As seguintes etapas foram executadas:

1. Transformação em one-hot encoding: Para melhor processamento dos dados categóricos, utilizamos a técnica de one-hot encoding.
    
2. Normalização: Realizamos a normalização das seguintes variáveis: 'idade', 'pressão', 'colesterol', 'freq_crd_max' e 'depressão ST'. Essa etapa é importante para garantir que as variáveis estejam na mesma escala e facilitar o treinamento do modelo.
    
### Construção do modelo: 

Desenvolvemos uma rede neural utilizando um perceptron implementado do zero, sem o uso de bibliotecas específicas, devido à natureza acadêmica do projeto. A rede foi treinada com os dados pré-processados e ajustada com base em uma determinada métrica.

### Implementação do Callback: 

Criamos um Callback para capturar o melhor conjunto de pesos (weights) e bias durante o treinamento. Esse Callback nos permitiu monitorar a métrica escolhida e guardar os melhores valores obtidos.

##Avaliação do modelo:

Realizamos a avaliação do modelo utilizando três métricas: F1-score, Recall e Acurácia. Essas métricas fornecem insights sobre o desempenho do modelo em diferentes aspectos.

### Conclusão:   

Os modelos avaliados com acurácia e F1-score apresentaram desempenho semelhante, com acurácia = 0.9135 e F1-score = 0.8888. No entanto, considerando a natureza do problema de diagnóstico médico, a minimização de falsos negativos é essencial para evitar que pacientes doentes sejam erroneamente classificados como saudáveis.
Nesse sentido, o modelo avaliado com a métrica Recall obteve um valor de 0.9444, identificando corretamente 94,44% dos pacientes doentes. 
Trabalho acadêmico re4alizado em parceria com João Pedro Brito


