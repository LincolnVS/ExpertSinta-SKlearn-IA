### Regras do Sistema Especialista V1

#### Regra 1
    
    SE P1 = Não
    ENTÃO Resposta = Consiga mais dados CNF 100%

#### Regra 2
  
    SE P1 = Sim
    E  P2 = Sim
    E  P3 = Sim
    E  P4 = Não
    E  P5 = Não
    ENTÃO Resposta = SGD Classifier CNF 100%

#### Regra 3
  
    SE P1 = Sim
    E  P2 = Sim
    E  P3 = Sim
    E  P4 = Não
    E  P5 = Sim
    ENTÃO Resposta = Kernel Approximation CNF 100%

#### Regra 4
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Não
    E  P16 = Sim
    E  P17 = Sim
    E  P18 = Não
    ENTÃO Resposta = Kernel Approximation CNF 100%

#### Regra 5
  
    SE P1 = Sim
    E  P2 = Sim
    E  P3 = Sim
    E  P4 = Sim
    E  P6 = Não
    ENTÃO Resposta = Linear SVC CNF 100%

#### Regra 6
  
    SE P1 = Sim
    E  P2 = Sim
    E  P3 = Sim
    E  P4 = Sim
    E  P6 = Sim
    E  P7 = Não
    E  P8 = Não
    ENTÃO Resposta = KNeighbors Classifier CNF 100%

#### Regra 7
  
    SE P1 = Sim
    E  P2 = Sim
    E  P3 = Sim
    E  P4 = Sim
    E  P6 = Sim
    E  P7 = Não
    E  P8 = Sim
    ENTÃO Resposta = Ensemble Classifiers CNF 100%
          Resposta = SVC CNF 100%

#### Regra 8
  
    SE P1 = Sim
    E  P2 = Sim
    E  P3 = Sim
    E  P4 = Sim
    E  P6 = Sim
    E  P7 = Sim
    ENTÃO Resposta = Naive Bayes CNF 100%

#### Regra 9
  
    SE P1 = Sim
    E  P2 = Sim
    E  P3 = Não
    E  P9 = Sim
    E  P10 = Sim
    E  P11 = Não
    ENTÃO Resposta = KMeans CNF 100%

#### Regra 10
 
    SE P1 = Sim
    E  P2 = Sim
    E  P3 = Não
    E  P9 = Sim
    E  P10 = Sim
    E  P11 = Sim
    ENTÃO Resposta = GMM CNF 100%
          Resposta = Spectral Clustering CNF 100%

#### Regra 11
  
    SE P1 = Sim
    E  P2 = Sim
    E  P3 = Não
    E  P9 = Sim
    E  P10 = Não
    ENTÃO Resposta = MiniBatch KMeans CNF 100%

#### Regra 12
  
    SE P1 = Sim
    E  P2 = Sim
    E  P3 = Não
    E  P9 = Não
    E  P10 = Sim
    ENTÃO Resposta = Mean Shift CNF 100%
          Resposta = VBGMM CNF 100%

#### Regra 13
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Sim
    E  P4 = Não
    ENTÃO Resposta = SGD Regressor  CNF 100%

#### Regra 14
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Sim
    E  P4 = Sim
    E  P13 = Sim
    ENTÃO Resposta = Lasso CNF 100%
          Resposta = ElasticNet CNF 100%

#### Regra 15
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Sim
    E  P4 = Sim
    E  P13 = Não
    E  P14 = Não
    E  P15 = Sim
    ENTÃO Resposta = SVR(kernel='rbf') CNF 100%

#### Regra 16
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Sim
    E  P4 = Sim
    E  P13 = Não
    E  P14 = Sim
    E  P15 = Não
    ENTÃO Resposta = RidgeRegression CNF 100%

#### Regra 17
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Sim
    E  P4 = Sim
    E  P13 = Não
    E  P14 = Não
    E  P15 = Não
    ENTÃO Resposta = SVR(kernel='rbf') CNF 100%
          Resposta = RidgeRegression CNF 100%

#### Regra 18
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Sim
    E  P4 = Sim
    E  P13 = Não
    E  P14 = Sim
    E  P15 = Sim
    ENTÃO Resposta = SVR(kernel='linear') CNF 100%
          Resposta = EnsembleRegressors CNF 100%

#### Regra 19
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Não
    E  P16 = Sim
    E  P17 = Não
    ENTÃO Resposta = Randomized PCA CNF 100%

#### Regra 20
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Não
    E  P16 = Sim
    E  P17 = Sim
    E  P18 = Sim
    E  P19 = Não
    E  P20 = Sim
    ENTÃO Resposta = Isomap CNF 100%

#### Regra 21
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Não
    E  P16 = Sim
    E  P17 = Sim
    E  P18 = Sim
    E  P19 = Sim
    E  P20 = Não
    ENTÃO Resposta = Spectral Embedding CNF 100%

#### Regra 22
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Não
    E  P16 = Sim
    E  P17 = Sim
    E  P18 = Sim
    E  P19 = Não
    E  P20 = Não
    ENTÃO Resposta = Isomap CNF 100%
          Resposta = Spectral Embedding CNF 100%

#### Regra 23
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Não
    E  P16 = Sim
    E  P17 = Sim
    E  P18 = Sim
    E  P19 = Sim
    E  P20 = Sim
    ENTÃO Resposta = LLE CNF 100%

#### Regra 24
  
    SE P1 = Sim
    E  P2 = Não
    E  P12 = Não
    E  P16 = Não
    ENTÃO Resposta = Infelizmente nenhum algoritmo do Scikit-Learn se encaixa nessas opções :( CNF 100%

#### Regra 25
  
    SE P1 = Sim
    E  P2 = Sim
    E  P3 = Não
    E  P9 = Não
    E  P10 = Não
    ENTÃO Resposta = Infelizmente nenhum algoritmo do Scikit-Learn se encaixa nessas opções :( CNF 100%

