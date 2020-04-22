### Regras do Sistema Especialista V2

#### Regra 1
  
    SE NÃO nAmostras = Menos de 50 amostras
    E  p1 = Não
    E  p2 = Sim
    ENTÃO Tipo de algoritmo = Regression  CNF 100%

#### Regra 2
  
    SE NÃO nAmostras = Menos de 50 amostras
    E  p1 = Sim
    E  p4 = Sim
    ENTÃO Tipo de algoritmo = Classification CNF 100%

#### Regra 3
  
    SE NÃO nAmostras = Menos de 50 amostras
    E  p1 = Sim
    E  p4 = Não
    E  p5 = Sim
    ENTÃO Tipo de algoritmo = Clustering com numero de categorias conhecida CNF 100%

#### Regra 4
  
    SE NÃO nAmostras = Menos de 50 amostras
    E  p1 = Sim
    E  p4 = Não
    E  p5 = Não
    ENTÃO Tipo de algoritmo = Clustering com numero de categorias desconhecida CNF 100%

#### Regra 5
  
    SE NÃO nAmostras = Menos de 50 amostras
    E  p1 = Não
    E  p2 = Não
    E  p3 = Sim
    ENTÃO Tipo de algoritmo = Dimensionality reduction CNF 100%

#### Regra 6
  
    SE NÃO nAmostras = Menos de 50 amostras
    E  p1 = Não
    E  p2 = Não
    E  p3 = Não
    ENTÃO Tipo de algoritmo = Dimensionality reduction CNF 100%

#### Regra 7
  
    SE nAmostras = Menos de 50 amostras
    OU nAmostras = DESCONHECIDO
    ENTÃO Algoritmo(s) recomendado(s) = Consiga mais dados  CNF 100%

#### Regra 8
  
    SE Tipo de algoritmo = Classification
    E  nAmostras = Mais de 100 mil amostras
    E  p10 = Não
    ENTÃO Algoritmo(s) recomendado(s) = SGD Classifier CNF 100%

#### Regra 9
  
    SE Tipo de algoritmo = Classification
    E  nAmostras = Mais de 100 mil amostras
    E  p10 = Sim
    OU Tipo de algoritmo = Dimensionality reduction
    E  nAmostras = Entre 50 e 10 mil amostras
    E  p15 = Sim
    ENTÃO Algoritmo(s) recomendado(s) = Kernel Approximation  CNF 100%

#### Regra 10
  
    SE Tipo de algoritmo = Classification
    E  nAmostras = Mais de 100 mil amostras
    E  p11 = Não
    ENTÃO Algoritmo(s) recomendado(s) = Linear SVC CNF 100%

#### Regra 11
  
    SE Tipo de algoritmo = Classification
    E  nAmostras = Mais de 100 mil amostras
    E  p11 = Sim
    E  p12 = Não
    E  p13 = Não
    ENTÃO Algoritmo(s) recomendado(s) = KNeighbors Classifier CNF 100%

#### Regra 12
  
    SE Tipo de algoritmo = Classification
    E  nAmostras = Mais de 100 mil amostras
    E  p11 = Sim
    E  p12 = Não
    E  p13 = Sim
    ENTÃO Algoritmo(s) recomendado(s) = SVC CNF 100%
          Algoritmo(s) recomendado(s) = Ensemble Classifiers CNF 100%

#### Regra 13
  
    SE Tipo de algoritmo = Classification
    E  nAmostras = Mais de 100 mil amostras
    E  p11 = Sim
    E  p12 = Sim
    ENTÃO Algoritmo(s) recomendado(s) = Naive Bayes CNF 100%

#### Regra 14
  
    SE Tipo de algoritmo = Clustering com numero de categorias conhecida
    E  nAmostras = Entre 50 e 10 mil amostras
    E  p14 = Não
    ENTÃO Algoritmo(s) recomendado(s) = KMeans CNF 100%

#### Regra 15
  
    SE Tipo de algoritmo = Clustering com numero de categorias conhecida
    E  nAmostras = Entre 50 e 10 mil amostras
    E  p14 = Sim
    ENTÃO Algoritmo(s) recomendado(s) = Spectral Clustering CNF 100%
          Algoritmo(s) recomendado(s) = GMM CNF 100%

#### Regra 16
  
    SE Tipo de algoritmo = Clustering com numero de categorias conhecida
    E  nAmostras = Entre 50 e 10 mil amostras
    ENTÃO Algoritmo(s) recomendado(s) = MiniBatch KMeans CNF 100%

#### Regra 17
  
    SE Tipo de algoritmo = Clustering com numero de categorias desconhecida
    E  nAmostras = Entre 50 e 10 mil amostras
    ENTÃO Algoritmo(s) recomendado(s) = Mean Shift CNF 100%
          Algoritmo(s) recomendado(s) = VBGMM CNF 100%

#### Regra 18
  
    SE Tipo de algoritmo = Regression 
    E  nAmostras = Mais de 100 mil amostras
    ENTÃO Algoritmo(s) recomendado(s) = SGD Regressor  CNF 100%

#### Regra 19
  
    SE Tipo de algoritmo = Regression 
    E  nAmostras = Mais de 100 mil amostras
    E  p18 = Sim
    ENTÃO Algoritmo(s) recomendado(s) = Lasso CNF 100%
          Algoritmo(s) recomendado(s) = ElasticNet CNF 100%

#### Regra 20
  
    SE Tipo de algoritmo = Regression 
    E  nAmostras = Mais de 100 mil amostras
    E  p18 = Não
    E  p19 = Não
    ENTÃO Algoritmo(s) recomendado(s) = SVR(kernel='linear') CNF 100%

#### Regra 21
  
    SE Tipo de algoritmo = Regression 
    E  nAmostras = Mais de 100 mil amostras
    E  p18 = Não
    E  p20 = Não
    ENTÃO Algoritmo(s) recomendado(s) = RidgeRegression CNF 100%

#### Regra 22
  
    SE Tipo de algoritmo = Regression 
    E  nAmostras = Mais de 100 mil amostras
    E  p18 = Não
    E  p19 = Sim
    E  p20 = Sim
    ENTÃO Algoritmo(s) recomendado(s) = EnsembleRegressors  CNF 100%
          Algoritmo(s) recomendado(s) = SVR(kernel='rbf')  CNF 100%

#### Regra 23
  
    SE Tipo de algoritmo = Dimensionality reduction
    E  p15 = Não
    ENTÃO Algoritmo(s) recomendado(s) = Randomized PCA CNF 100%

#### Regra 24
  
    SE Tipo de algoritmo = Dimensionality reduction
    E  nAmostras = Entre 50 e 10 mil amostras
    E  p15 = Sim
    E  p16 = Não
    ENTÃO Algoritmo(s) recomendado(s) = Isomap CNF 100%

#### Regra 25
  
    SE Tipo de algoritmo = Dimensionality reduction
    E  nAmostras = Entre 50 e 10 mil amostras
    E  p15 = Sim
    E  p17 = Não
    ENTÃO Algoritmo(s) recomendado(s) = Spectral Embedding CNF 100%

#### Regra 26
  
    SE Tipo de algoritmo = Dimensionality reduction
    E  nAmostras = Entre 50 e 10 mil amostras
    E  p15 = Sim
    E  p16 = Sim
    E  p17 = Sim
    ENTÃO Algoritmo(s) recomendado(s) = LLE CNF 100%

 #### Regra 27
  
    SE Tipo de algoritmo = Nenhum tipo de algoritmo
    OU Tipo de algoritmo = Clustering com numero de categorias desconhecida
    E  nAmostras = Entre 50 e 10 mil amostras
    ENTÃO Algoritmo(s) recomendado(s) = Infelizmente nenhum algoritmo do Scikit-Learn se encaixa nessas opções :( CNF 100%
