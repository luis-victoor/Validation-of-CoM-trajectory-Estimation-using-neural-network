# Validação de sistema de cálculo de trajetória de centro de massa corporal utilizando BlazePose

Projeto em desenvolvimento utilizando dados de IMUs do banco de dados [MoVi: A Large Multipurpose Motion and Video Dataset](https://dataverse.scholarsportal.info/dataset.xhtml?persistentId=doi:10.5683/SP2/JRHDRN) para realizar a análise e classificação do movimento de sentar e levantar utilizando dados de aceleração das IMUs. Para a separação dos dados de aceleração referentes apenas ao movimento de sentar e levantar, utilizou-se os dados de vídeo como referência visual para os dados das IMUs que foram sincronizados. A imagem a seguir demonstra alguns exemplos de voluntários sentados, utilizando diferentes assentos. 

O centro de massa corporal é um parâmetro bastante útil para o estudo do movimento humano. Sua trajetória reflete a interação dos diferentes segmentos corporais na hora de gerar movimento. Existem na literatura vários métodos para estimativa da trajetória do centro de massa corporal e dependendo da natureza dos dados utilizados no cálculo, é necessário um conjunto de equipamentos de alto custo, como câmeras de visão computacional, sistemas de captura de movimento e marcadores corporais, cujo uso é mais apropriado dentro de ambientes laboratoriais. Pensando nas limitações de custo e na complexidade da aplicação dos equipamentos, este trabalho propõe uma abordagem capaz de realizar a estimativa da trajetória do centro de massa automaticamente através da técnica de segmentação corporal, utilizando apenas uma câmera simples e o sistema baseado em rede neural BlazePose.

Referências: 

- [On-device, Real-time Body Pose Tracking with MediaPipe BlazePose] (https://ai.googleblog.com/2020/08/on-device-real-time-body-pose-tracking.html)
- [MoVi: A Large Multipurpose Motion and Video Dataset](https://dataverse.scholarsportal.info/dataset.xhtml?persistentId=doi:10.5683/SP2/JRHDRN)
