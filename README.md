# Validação de sistema de cálculo de trajetória de centro de massa corporal utilizando BlazePose

O centro de massa corporal é um parâmetro bastante útil para o estudo do movimento humano. Sua trajetória reflete a interação dos diferentes segmentos corporais na hora de gerar movimento. Existem na literatura vários métodos para estimativa da trajetória do centro de massa corporal e dependendo da natureza dos dados utilizados no cálculo, é necessário um conjunto de equipamentos de alto custo, como câmeras de visão computacional, sistemas de captura de movimento e marcadores corporais, cujo uso é mais apropriado dentro de ambientes laboratoriais. 

Pensando nas limitações de custo e na complexidade da aplicação dos equipamentos, este trabalho em desenvolvimento propõe uma abordagem capaz de realizar a estimativa da trajetória do centro de massa automaticamente através da técnica de segmentação corporal, utilizando apenas uma câmera simples e o sistema baseado em rede neural Blaze Pose.

A imagem a seguir demonstra alguns exemplos da rede neural atuando na estimativa de pose usando imagens simples:

<p align="center">
  <img src="https://github.com/gustavomontoli/Validation-of-CoM-trajectory-Estimation-using-neural-network/blob/main/imagens/imagem1.JPG" alt="Exemplos de imagens com rede neural"/>
</p>

<p align="center">
  <img src="https://github.com/gustavomontoli/Validation-of-CoM-trajectory-Estimation-using-neural-network/blob/main/imagens/imagem3.JPG" alt="Exemplos de imagens com rede neural"/>
</p>

A segunda etapa deste trabalho está relacionada à comparação entre a estimativa do CoM calculada com o método proposto e aquela obtida a partir de sistemas de captura de movimento (MoCap) mais sofisticados considerados o padrão ouro para este tipo de medição. A imagem abaixo demonstra a comparação preliminar entre os dois sistemas utilizando o algoritmo Dynamic Time Warping.

<p align="center">
  <img src="https://github.com/gustavomontoli/Validation-of-CoM-trajectory-Estimation-using-neural-network/blob/main/imagens/imagem2.JPG" alt="Exemplos de imagens com rede neural"/>
</p>

Referências: 

- [On-device, Real-time Body Pose Tracking with MediaPipe BlazePose] (https://ai.googleblog.com/2020/08/on-device-real-time-body-pose-tracking.html)
- [MoVi: A Large Multipurpose Motion and Video Dataset](https://dataverse.scholarsportal.info/dataset.xhtml?persistentId=doi:10.5683/SP2/JRHDRN)

# Dependências 

Abaixo está o comando para baixar as dependências deste projeto.

~~~Python
pip install -r requirements.txt
~~~

É possível também criar um [ambiente virtual](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/).

- Numpy (pip install numpy)
- Pandas (pip install pandas)
- Matplotlib (pip install matplotlib)
- Opencv (pip install opencv-python)
- Math (pip install math)
- Scipy (pip install scipy)
- Pathlib (pip install pathlib)
- Os (pip install os)
- Sys (pip install sys)
- Collections (pip install collections)
- Re (pip install re)
- Fastdtw (pip install fastdtw)
- Dtw (pip install dtw)
- Seaborn (pip install seaborn)
- Mediapipe (pip install mediapipe)

